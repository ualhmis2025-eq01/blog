---
layout: page
title: "Contacto"
permalink: /contacto/
---

<h2 style="text-align: center;">📬 Formulario de Contacto</h2>

<form action="https://formspree.io/f/meoaqpdz" method="POST" style="max-width: 500px; margin: auto; padding: 20px; border-radius: 8px; background-color: #f9f9f9; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  
  <label for="name" style="display: block; margin-bottom: 5px; font-weight: bold;">Nombre:</label>
  <input type="text" id="name" name="name" required style="width: 100%; padding: 10px; margin-bottom: 15px; border: 1px solid #ccc; border-radius: 4px;">

  <label for="email" style="display: block; margin-bottom: 5px; font-weight: bold;">Correo Electrónico:</label>
  <input type="email" id="email" name="email" required style="width: 100%; padding: 10px; margin-bottom: 15px; border: 1px solid #ccc; border-radius: 4px;">

  <label for="asunto" style="display: block; margin-bottom: 5px; font-weight: bold;">Asunto:</label>
  <input type="text" id="asunto" name="asunto" required style="width: 100%; padding: 10px; margin-bottom: 15px; border: 1px solid #ccc; border-radius: 4px;">

  <label for="message" style="display: block; margin-bottom: 5px; font-weight: bold;">Mensaje:</label>
  <textarea id="message" name="message" rows="4" required style="width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 4px;"></textarea>

  <button type="submit" style="margin-top: 15px; width: 100%; padding: 10px; background-color: #007acc; color: #fff; border: none; border-radius: 4px; cursor: pointer;">Enviar ✉️</button>
</form>
