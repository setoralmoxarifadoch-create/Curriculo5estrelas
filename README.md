<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gerador de Currículos - Petrópolis RJ</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
</head>
<body class="bg-gray-100 font-sans text-gray-800 p-4 md:p-8">

    <div class="max-w-4xl mx-auto bg-white rounded-2xl shadow-xl overflow-hidden border border-gray-200">
        <div class="bg-emerald-800 text-white p-6 text-center">
            <h1 class="text-2xl font-bold">📝 Criador de Currículo Oficial</h1>
            <p class="text-emerald-200 text-xs mt-1">Preencha os dados abaixo para gerar o seu PDF formatado</p>
        </div>

        <form id="form-curriculo" class="p-6 md:p-10 space-y-6">
            
            <div class="border-b pb-6">
                <h2 class="text-lg font-bold text-emerald-800 mb-4">1. Dados Pessoais</h2>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                    
                    <div class="flex flex-col items-center justify-center border-2 border-dashed rounded-xl p-4 bg-gray-50">
                        <label class="cursor-pointer text-center">
                            <span class="text-xs text-gray-500 font-medium block mb-2">📸 Foto de Perfil</span>
                            <input type="file" id="foto" accept="image/*" onchange="carregarFoto(event)" class="hidden">
                            <img id="preview-foto" src="https://via.placeholder.com/100" class="w-24 h-24 object-cover rounded-full border-2 border-emerald-600 hidden">
                            <span id="txt-upload" class="bg-emerald-50 text-emerald-700 text-xs px-3 py-1.5 rounded-lg font-bold hover:bg-emerald-100">Selecionar Foto</span>
                        </label>
                    </div>

                    <div class="md:col-span-2 space-y-3">
                        <div>
                            <label class="block text-xs font-semibold text-gray-600">Nome Completo</label>
                            <input type="text" id="nome" required class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-emerald-600 outline-none">
                        </div>
                        <div class="grid grid-cols-2 gap-2">
                            <div>
                                <label class="block text-xs font-semibold text-gray-600">E-mail</label>
                                <input type="email" id="email" required class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-emerald-600 outline-none">
                            </div>
                            <div>
                                <label class="block text-xs font-semibold text-gray-600">Telefone / WhatsApp</label>
                                <input type="text" id="telefone" placeholder="(24) 99999-9999" required class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-emerald-600 outline-none">
                            </div>
                        </div>
                    </div>
                </div>
