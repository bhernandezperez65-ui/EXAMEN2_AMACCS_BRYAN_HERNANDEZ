<template>
    <form class="cine-formulario">
        <label>
            Nombre:
            <input type="text" name="nombre" required />
        </label>

        <label>
            Correo electrónico:
            <input type="email" name="correo" required />
        </label>

        <label>
            Película:
            <select name="pelicula" required>
                <option value="">Selecciona una película</option>
                <option value="pelicula1">Toy Story</option>
                <option value="pelicula2">Spiderman 3</option>
                <option value="pelicula3">Avengers</option>
                <option value="pelicula3">Sonic 2</option>
                <option value="pelicula3">Thunderbolts</option>
                <option value="pelicula3">TRON ARES</option>
            </select>
        </label>

        <label>
            Cantidad de entradas:
            <input type="number" name="entradas" min="1" max="10" required />
        </label>

        <label>
            Horario:
            <select name="horario" required>
                <option value="">Selecciona un horario</option>
                <option value="14:00">14:00</option>
                <option value="17:00">17:00</option>
                <option value="20:00">20:00</option>
                <option value="20:00">21:00</option>
                <option value="20:00">22:00</option>
                <option value="20:00">23:00</option>
            </select>
        </label>

        <button type="submit">Reservar</button>
    </form>
</template>

<style scoped>
.cine-formulario {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    max-width: 400px;
    margin: auto;
    padding: 1.5rem;
    background: #f8f8f8;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

label {
    display: flex;
    flex-direction: column;
    font-weight: 600;
    color: #333;
}

input,
select {
    padding: 0.6rem;
    border: 1px solid #ccc;
    border-radius: 8px;
    font-size: 1rem;
}

button {
    padding: 0.8rem;
    background-color: #e50914;
    color: white;
    font-weight: bold;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.2s ease;
}

button:hover {
    background-color: #b00610;
}
</style>
