// Tableaux des caractéristiques possibles
const races = ['Humain', 'Elfe', 'Nain', 'Halfelin', 'Demi-elfe'];
const classes = ['Barbare', 'Bard', 'Clerc', 'Druide', 'Guerrier', 'Magicien', 'Paladin', 'Rôdeur', 'Sorcier'];
const genders = ['Homme', 'Femme', 'Non-binaire'];
const alignments = ['Loyal bon', 'Neutre bon', 'Chaotique bon', 'Loyal neutre', 'Neutre', 'Chaotique neutre', 'Loyal mauvais', 'Neutre mauvais', 'Chaotique mauvais'];

// Fonction pour choisir une valeur aléatoire dans un tableau
function getRandomValue(array) {
  const randomIndex = Math.floor(Math.random() * array.length);
  return array[randomIndex];
}

// Création du personnage
const character = {
  race: getRandomValue(races),
  class: getRandomValue(classes),
  gender: getRandomValue(genders),
  alignment: getRandomValue(alignments),
  level: Math.floor(Math.random() * 20) + 1,
  hitPoints: Math.floor(Math.random() * 100) + 1,
  strength: Math.floor(Math.random() * 20) + 1,
  dexterity: Math.floor(Math.random() * 20) + 1,
  constitution: Math.floor(Math.random() * 20) + 1,
  intelligence: Math.floor(Math.random() * 20) + 1,
  wisdom: Math.floor(Math.random() * 20) + 1,
  charisma: Math.floor(Math.random() * 20) + 1
};

console.log(character);

