var buttonTimeout;
var messageTimeout;

function giveAnswer(answer) {
  var responseDiv = document.getElementById('response');
  if (answer === 'Tak') {
    responseDiv.innerText = "W takim razie zabieram Cię w środę na walentynki!";
    showHeart();
  } else {
    responseDiv.innerText = "Błędna odpowiedź, spróbuj jeszcze raz";
  }
}

function showHeart() {
  var heart = document.getElementById('heart');
  heart.classList.remove('hidden');
}

function hideButtonAndShowMessage() {
  var button = document.getElementById('noButton');
  var message = document.getElementById('message');

  button.style.visibility = 'hidden';
  message.classList.remove('hidden');

  clearTimeout(buttonTimeout);
}

function showButtonAndHideMessage() {
  var button = document.getElementById('noButton');
  var message = document.getElementById('message');

  messageTimeout = setTimeout(function() {
    message.classList.add('hidden');
  }, 1000);

  buttonTimeout = setTimeout(function() {
    button.style.visibility = 'visible';
  }, 500);
}
