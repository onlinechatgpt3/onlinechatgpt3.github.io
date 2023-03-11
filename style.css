const OPENAI_API_KEY = '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';

function getResponse() {
    const prompt = document.getElementById('prompt').value;
    fetch('https://api.openai.com/v1/completions', {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
            'Authorization': `Bearer ${OPENAI_API_KEY}`
        },
        body: JSON.stringify({
            'model': 'text-davinci-002',
            'prompt': prompt,
            'temperature': 0.5,
            'max_tokens': 50,
            'n': 1,
            'stop': null
        })
    })
    .then(response => response.json())
    .then(data => {
        const response = data.choices[0].text;
        document.getElementById('response').textContent = response;
    })
    .catch(error => console.error(error));
}
