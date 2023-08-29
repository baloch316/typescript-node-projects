import inquirer from "inquirer";

async function askQuestion() {
  var answers = await inquirer.prompt([
    {
      type: "list",
      name: "operator",
      message: "what type of calculation do you want to perform? \n",
      choices: ["Addition", "Subtraction", "Multiplication", "Division"],
    },
    {
      type: "number",
      name: "num1",
      message:"Enter number 1;"
    },
    {
        type: "number",
        name: "num2",
        message:"Enter number 2;"
      },
  ]);
  if (answers.operator === "Addition") {
    console.log(`${answers.num1} + ${answers.num2} = ${answers.num1 + answers.num2}`);
  } else if (answers.operator === "Subtraction") {
    console.log(`${answers.num1} - ${answers.num2} = ${answers.num1 - answers.num2}`);
  } else if (answers.operator === "Multiplication") {
    console.log(`${answers.num1} * ${answers.num2} = ${answers.num1 * answers.num2}`);
  } else if (answers.operator === "Division") {
    console.log(`${answers.num1} / ${answers.num2} = ${answers.num1 / answers.num2}`);
  }
}
async function startAgain() {
    do{
        await askQuestion();
        var again = await inquirer
        .prompt({
            type:
            
            "input",
            name:"restart",
            message:"Do You Want To Continue Press Y or N"
        })
