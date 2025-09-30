<template>
  <div class="form-container">
    <h2>Formulario de Datos Personales</h2>
    <form>
      <div class="form-group">
        <label for="name">Nombre completo</label>
        <input type="text" id="name" name="name" required />
      </div>

      <div class="form-group">
        <label for="email">Correo electrónico</label>
        <input type="email" id="email" name="email" required />
      </div>

      <div class="form-group">
        <label for="phone">Teléfono</label>
        <input type="tel" id="phone" name="phone" />
      </div>

      <div class="form-group">
        <label for="birthdate">Fecha de nacimiento</label>
        <input type="date" id="birthdate" name="birthdate" />
      </div>

      <div class="form-group">
        <label for="address">Dirección</label>
        <textarea id="address" name="address" rows="3"></textarea>
      </div>

      <button type="submit">Enviar</button>
    </form>
  </div>
</template>

<script>
export default{
    name: 'formUno'
};
</script>

<style>
    .form-container {
      max-width: 600px;
      margin: 50px auto;
      background-color: #fff;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    .form-container h2 {
      margin-bottom: 20px;
      font-size: 24px;
      color: #333;
      text-align: center;
    }

    .form-group {
      margin-bottom: 15px;
    }

    label {
      display: block;
      margin-bottom: 6px;
      font-weight: 600;
      color: #555;
    }

    input,
    textarea {
      width: 90%;
      padding: 10px 12px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 16px;
      transition: border-color 0.3s ease;
    }

    input:focus,
    textarea:focus {
      border-color: #007bff;
      outline: none;
    }

    button {
      width: 100%;
      padding: 12px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #0056b3;
    }
</style>
