Создайте функцию truncate(str, maxlength), которая проверяет длину строки str и, если она превосходит maxlength, заменяет конец str на "…", так, чтобы её длина стала равна maxlength.

Результатом функции должна быть та же строка, если усечение не требуется, либо, если необходимо, усечённая строка.

function truncate(str, maxlength) {
	if (maxlength < str.length) {
		let startOfString = str.substr(0,maxlength - 1);
		let endOfString = str.slice(maxlength - 1);
		endOfString = '…'
    
		return startOfString + endOfString;
	} 
  else return str;
}
