# Loja-delicatta-
Aproveite nossa loja
import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { ShoppingCart } from "lucide-react";

const products = [
  {
    id: 1,
    name: "Jogo da Memória - Animais",
    price: 39.9,
    image: "/images/jogo_memoria_animais.jpg",
  },
  {
    id: 2,
    name: "Jogo da Memória - Frutas",
    price: 39.9,
    image: "/images/jogo_memoria_frutas.jpg",
  },
  {
    id: 3,
    name: "Jogo Sensorial - Madeira",
    price: 49.9,
    image: "/images/jogo_sensorial_madeira.jpg",
  },
  {
    id: 4,
    name: "Kit Alfabetização Montessori",
    price: 59.9,
    image: "/images/kit_alfabetizacao_montessori.jpg",
  },
];

export default function LojaDelicatta() {
  return (
    <div className="min-h-screen bg-pink-50 p-6">
      <h1 className="text-4xl font-bold text-center text-pink-700 mb-10">
        Loja Delicatta
      </h1>
      <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        {products.map((product) => (
          <Card key={product.id} className="rounded-2xl shadow-lg">
            <CardContent className="p-4">
              <img
                src={product.image}
                alt={product.name}
                className="w-full h-60 object-cover rounded-xl"
              />
              <h2 className="text-xl font-semibold text-pink-800 mt-4">
                {product.name}
              </h2>
              <p className="text-lg text-pink-600">R$ {product.price.toFixed(2)}</p>
              <Button className="mt-4 w-full bg-pink-500 hover:bg-pink-600 text-white">
                <ShoppingCart className="mr-2" /> Adicionar ao carrinho
              </Button>
            </CardContent>
          </Card>
        ))}
      </div>
    </div>
  );
}


Pronto! Criei um site de vendas simples para a Loja Delicatta, com base nas imagens e nas preferências que você indicou:

Tema rosa

Layout em grade

Botões de compra com ícone de carrinho


Agora podemos:

Publicar isso como um site real

Adicionar carrinho funcional ou checkout

Traduzir para dispositivos móveis


Deseja que eu gere os arquivos finais ou publique com alguma plataforma específica (como Vercel ou Netlify)?

