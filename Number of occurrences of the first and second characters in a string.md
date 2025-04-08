# puzzles
All the puzzles has solution!
function countFirstAndSecondEl(str){
  if(str.length === 0) return `Empty string`;
  if(str[0].toLowerCase() === str[1].toLowerCase()) return `The first and second symbols are the same`;
  let count1 = 0;
  let count2 = 0;
  let obj = {};
  for(let i = 0; i < str.length; i++){
  if(str[i].toLowerCase() === str[0].toLowerCase()) count1++;
  if(str[i].toLowerCase() === str[1].toLowerCase()) count2++;
  obj[str[0].toLowerCase()] = count1;
  obj[str[1].toLowerCase()] = count2;
  }
  return `${str[0].toLowerCase()} - ${count1}, ${str[1].toLowerCase()} - ${count2}`;
}
console.log(countFirstAndSecondEl('All the puzzles has solution!'));
