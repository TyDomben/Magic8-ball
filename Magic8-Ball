function weightedMagic8Ball() {
    // Array of objects where each object represents a possible response and its associated weight
    const responses = [
        { answer: "Yes, definitely.", weight: 10 },
        { answer: "No, not likely.", weight: 5 },
        { answer: "Maybe, it's unclear.", weight: 20 },
        // ... more responses can be added here
    ];

    // Calculate the total weight by summing up the weights of all responses
    let totalWeight = responses.reduce((sum, response) => sum + response.weight, 0);

    // Generate a random number between 0 and the total weight
    let randomNum = Math.random() * totalWeight;

    // Iterate through the responses
    for (let response of responses) {
        // If the random number is less than the current response's weight, return that response
        if (randomNum < response.weight) {
            return response.answer;
        }
        // Subtract the weight of the current response from the random number
        randomNum -= response.weight;
    }
}

// Example usage of the function
console.log(weightedMagic8Ball());
