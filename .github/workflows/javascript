// Inicializar el mapa y establecer la vista en Bogotá
var map = L.map('map').setView([4.7110, -74.0721], 12);

// Añadir una capa de mapa base de OpenStreetMap
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
}).addTo(map);

// Añadir ríos de Bogotá (simplificado para este ejemplo)
var rios = [
    {name: "Río Bogotá", coords: [[4.643, -74.121], [4.730, -74.085], [4.800, -74.070]]},
    {name: "Río Tunjuelo", coords: [[4.620, -74.147], [4.600, -74.100], [4.580, -74.080]]}
];

rios.forEach(function(rio) {
    L.polyline(rio.coords, {color: 'blue'}).addTo(map).bindPopup(rio.name);
});

// Añadir marcadores de obras
var obras = [
    {name: "Obra 1", coords: [4.676, -74.047]},
    {name: "Obra 2", coords: [4.641, -74.091]},
    {name: "Obra 3", coords: [4.689, -74.092]}
];

obras.forEach(function(obra) {
    L.marker(obra.coords).addTo(map).bindPopup(obra.name);
});
