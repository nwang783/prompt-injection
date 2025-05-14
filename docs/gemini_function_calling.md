[Skip to main content](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#main-content)

[![Google AI for Developers](https://www.gstatic.com/devrel-devsite/prod/ve761bca974e16662f27aa8810df6d144acde5bdbeeca0dfd50e25f86621eaa19/googledevai/images/lockup-new.svg)](https://ai.google.dev/)

`/`

- [English](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting)
- [Deutsch](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=de)
- [Español – América Latina](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=es-419)
- [Français](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=fr)
- [Indonesia](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=id)
- [Italiano](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=it)
- [Polski](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=pl)
- [Português – Brasil](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=pt-br)
- [Shqip](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=sq)
- [Tiếng Việt](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=vi)
- [Türkçe](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=tr)
- [Русский](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=ru)
- [עברית](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=he)
- [العربيّة](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=ar)
- [فارسی](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=fa)
- [हिंदी](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=hi)
- [বাংলা](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=bn)
- [ภาษาไทย](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=th)
- [中文 – 简体](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=zh-cn)
- [中文 – 繁體](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=zh-tw)
- [日本語](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=ja)
- [한국어](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting&hl=ko)

[Sign in](https://ai.google.dev/_d/signin?continue=https%3A%2F%2Fai.google.dev%2Fgemini-api%2Fdocs%2Ffunction-calling%3Fexample%3Dmeeting&prompt=select_account)

- On this page
- [How Function Calling Works](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#how_function_calling_works)
  - [Step 1: Define Function Declaration](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_1_define_function_declaration)
  - [Step 2: Call the model with function declarations](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_2_call_the_model_with_function_declarations)
  - [Step 3: Execute set\_light\_values function code](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_3_execute_set_light_values_function_code)
  - [Step 4: Create User friendly response with function result and call the model again](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_4_create_user_friendly_response_with_function_result_and_call_the_model_again)
- [Function declarations](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#function_declarations)
- [Parallel Function Calling](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#parallel_function_calling)
- [Compositional Function Calling](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#compositional_function_calling)
- [Function calling modes](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#function_calling_modes)
- [Automatic Function Calling (Python Only)](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#automatic_function_calling_python_only)
  - [Automatic Function schema declaration](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#automatic_function_schema_declaration)
- [Multi-tool use: Combine Native Tools with Function Calling](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#multi-tool_use_combine_native_tools_with_function_calling)
- [Use Model Context Protocol (MCP)](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#use_model_context_protocol_mcp)
- [Supported Models](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#supported_models)
- [Best Practices](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#best_practices)
- [Notes and Limitations](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#notes_and_limitations)

Introducing Gemini 2.5 Flash, Veo 2, and updates to the Live API [Learn more](https://developers.googleblog.com/en/gemini-2-5-flash-pro-live-api-veo-2-gemini-api/)

- [Home](https://ai.google.dev/)
- [Gemini API](https://ai.google.dev/gemini-api)
- [Models](https://ai.google.dev/gemini-api/docs)

Was this helpful?



 Send feedback



# Function Calling with the Gemini API

- On this page
- [How Function Calling Works](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#how_function_calling_works)
  - [Step 1: Define Function Declaration](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_1_define_function_declaration)
  - [Step 2: Call the model with function declarations](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_2_call_the_model_with_function_declarations)
  - [Step 3: Execute set\_light\_values function code](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_3_execute_set_light_values_function_code)
  - [Step 4: Create User friendly response with function result and call the model again](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#step_4_create_user_friendly_response_with_function_result_and_call_the_model_again)
- [Function declarations](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#function_declarations)
- [Parallel Function Calling](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#parallel_function_calling)
- [Compositional Function Calling](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#compositional_function_calling)
- [Function calling modes](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#function_calling_modes)
- [Automatic Function Calling (Python Only)](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#automatic_function_calling_python_only)
  - [Automatic Function schema declaration](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#automatic_function_schema_declaration)
- [Multi-tool use: Combine Native Tools with Function Calling](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#multi-tool_use_combine_native_tools_with_function_calling)
- [Use Model Context Protocol (MCP)](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#use_model_context_protocol_mcp)
- [Supported Models](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#supported_models)
- [Best Practices](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#best_practices)
- [Notes and Limitations](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#notes_and_limitations)

Function calling lets you connect models to external tools and APIs.
Instead of generating text responses, the model understands when to call specific
functions and provides the necessary parameters to execute real-world actions.
This allows the model to act as a bridge between natural language and real-world
actions and data. Function calling has 3 primary use cases:

- **Augment Knowledge:** Access information from external sources like databases, APIs, and knowledge bases.
- **Extend Capabilities:** Use external tools to perform computations and extend the limitations of the model, such as using a calculator or creating charts.
- **Take Actions:** Interact with external systems using APIs, such as scheduling appointments, creating invoices, sending emails, or controlling smart home devices

Get WeatherSchedule MeetingCreate Chart

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)[REST](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#rest)More

```
 from google import genai
 from google.genai import types

 # Define the function declaration for the model
 schedule_meeting_function = {
     "name": "schedule_meeting",
     "description": "Schedules a meeting with specified attendees at a given time and date.",
     "parameters": {
         "type": "object",
         "properties": {
             "attendees": {
                 "type": "array",
                 "items": {"type": "string"},
                 "description": "List of people attending the meeting.",
             },
             "date": {
                 "type": "string",
                 "description": "Date of the meeting (e.g., '2024-07-29')",
             },
             "time": {
                 "type": "string",
                 "description": "Time of the meeting (e.g., '15:00')",
             },
             "topic": {
                 "type": "string",
                 "description": "The subject or topic of the meeting.",
             },
         },
         "required": ["attendees", "date", "time", "topic"],
     },
 }

 # Configure the client and tools
 client = genai.Client(api_key=os.getenv("GEMINI_API_KEY"))
 tools = types.Tool(function_declarations=[schedule_meeting_function])
 config = types.GenerateContentConfig(tools=[tools])

 # Send request with function declarations
 response = client.models.generate_content(
     model="gemini-2.0-flash",
     contents="Schedule a meeting with Bob and Alice for 03/14/2025 at 10:00 AM about the Q3 planning.",
     config=config,
 )

 # Check for a function call
 if response.candidates[0].content.parts[0].function_call:
     function_call = response.candidates[0].content.parts[0].function_call
     print(f"Function to call: {function_call.name}")
     print(f"Arguments: {function_call.args}")
     #  In a real app, you would call your function here:
     #  result = schedule_meeting(**function_call.args)
 else:
     print("No function call found in the response.")
     print(response.text)

```

```
import { GoogleGenAI, Type } from '@google/genai';

// Configure the client
const ai = new GoogleGenAI({ apiKey: process.env.GEMINI_API_KEY });

// Define the function declaration for the model
const scheduleMeetingFunctionDeclaration = {
  name: 'schedule_meeting',
  description: 'Schedules a meeting with specified attendees at a given time and date.',
  parameters: {
    type: Type.OBJECT,
    properties: {
      attendees: {
        type: Type.ARRAY,
        items: { type: Type.STRING },
        description: 'List of people attending the meeting.',
      },
      date: {
        type: Type.STRING,
        description: 'Date of the meeting (e.g., "2024-07-29")',
      },
      time: {
        type: Type.STRING,
        description: 'Time of the meeting (e.g., "15:00")',
      },
      topic: {
        type: Type.STRING,
        description: 'The subject or topic of the meeting.',
      },
    },
    required: ['attendees', 'date', 'time', 'topic'],
  },
};

// Send request with function declarations
const response = await ai.models.generateContent({
  model: 'gemini-2.0-flash',
  contents: 'Schedule a meeting with Bob and Alice for 03/27/2025 at 10:00 AM about the Q3 planning.',
  config: {
    tools: [{\
      functionDeclarations: [scheduleMeetingFunctionDeclaration]\
    }],
  },
});

// Check for function calls in the response
if (response.functionCalls && response.functionCalls.length > 0) {
  const functionCall = response.functionCalls[0]; // Assuming one function call
  console.log(`Function to call: ${functionCall.name}`);
  console.log(`Arguments: ${JSON.stringify(functionCall.args)}`);
  // In a real app, you would call your actual function here:
  // const result = await scheduleMeeting(functionCall.args);
} else {
  console.log("No function call found in the response.");
  console.log(response.text);
}

```

```
curl "https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=$GEMINI_API_KEY" \
  -H 'Content-Type: application/json' \
  -X POST \
  -d '{
    "contents": [\
      {\
        "role": "user",\
        "parts": [\
          {\
            "text": "Schedule a meeting with Bob and Alice for 03/27/2025 at 10:00 AM about the Q3 planning."\
          }\
        ]\
      }\
    ],
    "tools": [\
      {\
        "functionDeclarations": [\
          {\
            "name": "schedule_meeting",\
            "description": "Schedules a meeting with specified attendees at a given time and date.",\
            "parameters": {\
              "type": "object",\
              "properties": {\
                "attendees": {\
                  "type": "array",\
                  "items": {"type": "string"},\
                  "description": "List of people attending the meeting."\
                },\
                "date": {\
                  "type": "string",\
                  "description": "Date of the meeting (e.g., '2024-07-29')"\
                },\
                "time": {\
                  "type": "string",\
                  "description": "Time of the meeting (e.g., '15:00')"\
                },\
                "topic": {\
                  "type": "string",\
                  "description": "The subject or topic of the meeting."\
                }\
              },\
              "required": ["attendees", "date", "time", "topic"]\
            }\
          }\
        ]\
      }\
    ]
  }'

```

## How Function Calling Works

![function calling overview](https://ai.google.dev/static/gemini-api/docs/images/function-calling-overview.png)

Function calling involves a structured interaction between your application,
the model, and external functions. Here's a breakdown of the process:

1. **Define Function Declaration:** Define the function declaration in your
application code. Function Declarations describe the function's name,
parameters, and purpose to the model.
2. **Call LLM with function declarations:** Send user prompt along with the
function declaration(s) to the model. It analyzes the request and
determines if a function call would be helpful. If so, it responds with a
structured JSON object.
3. **Execute Function Code (Your Responsibility):** The Model _does not_
execute the function itself. It's your application's responsibility to
process the response and check for Function Call, if

   - **Yes**: Extract the name and args of the function and execute the
     corresponding function in your application.
   - **No:** The model has provided a direct text response to the prompt (this
     flow is less emphasized in the example but is a possible outcome).
4. **Create User friendly response:** If a function was executed, capture the
result and send it back to the model in a subsequent turn of the conversation.
It will use the result to generate a final, user-friendly response that
incorporates the information from the function call.

This process can be repeated over multiple turns, allowing for complex
interactions and workflows. The model also supports calling multiple functions in a
single turn ( [parallel function calling](https://ai.google.dev/gemini-api/docs/function-calling#parallel_function_calling)) and in sequence ( [compositional function\\
calling](https://ai.google.dev/gemini-api/docs/function-calling#compositional_function_calling)).

### Step 1: Define Function Declaration

Define a function and its declaration within your application code that allows
users to set light values and make an API request. This function could call
external services or APIs.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
from google.genai import types

# Define a function that the model can call to control smart lights
set_light_values_declaration = {
    "name": "set_light_values",
    "description": "Sets the brightness and color temperature of a light.",
    "parameters": {
        "type": "object",
        "properties": {
            "brightness": {
                "type": "integer",
                "description": "Light level from 0 to 100. Zero is off and 100 is full brightness",
            },
            "color_temp": {
                "type": "string",
                "enum": ["daylight", "cool", "warm"],
                "description": "Color temperature of the light fixture, which can be `daylight`, `cool` or `warm`.",
            },
        },
        "required": ["brightness", "color_temp"],
    },
}

# This is the actual function that would be called based on the model's suggestion
def set_light_values(brightness: int, color_temp: str) -> dict[str, int | str]:
    """Set the brightness and color temperature of a room light. (mock API).

    Args:
        brightness: Light level from 0 to 100. Zero is off and 100 is full brightness
        color_temp: Color temperature of the light fixture, which can be `daylight`, `cool` or `warm`.

    Returns:
        A dictionary containing the set brightness and color temperature.
    """
    return {"brightness": brightness, "colorTemperature": color_temp}

```

```
import { Type } from '@google/genai';

// Define a function that the model can call to control smart lights
const setLightValuesFunctionDeclaration = {
  name: 'set_light_values',
  description: 'Sets the brightness and color temperature of a light.',
  parameters: {
    type: Type.OBJECT,
    properties: {
      brightness: {
        type: Type.NUMBER,
        description: 'Light level from 0 to 100. Zero is off and 100 is full brightness',
      },
      color_temp: {
        type: Type.STRING,
        enum: ['daylight', 'cool', 'warm'],
        description: 'Color temperature of the light fixture, which can be `daylight`, `cool` or `warm`.',
      },
    },
    required: ['brightness', 'color_temp'],
  },
};

/**
* Set the brightness and color temperature of a room light. (mock API)
* @param {number} brightness - Light level from 0 to 100. Zero is off and 100 is full brightness
* @param {string} color_temp - Color temperature of the light fixture, which can be `daylight`, `cool` or `warm`.
* @return {Object} A dictionary containing the set brightness and color temperature.
*/
function setLightValues(brightness, color_temp) {
  return {
    brightness: brightness,
    colorTemperature: color_temp
  };
}

```

### Step 2: Call the model with function declarations

Once you have defined your function declarations, you can prompt the model to use
the function. It analyzes the prompt and function declarations and decides
to respond directly or to call a function. If a function is called the response
object will contain a function call suggestion.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
from google import genai

# Generation Config with Function Declaration
tools = types.Tool(function_declarations=[set_light_values_declaration])
config = types.GenerateContentConfig(tools=[tools])

# Configure the client
client = genai.Client(api_key=os.getenv("GEMINI_API_KEY"))

# Define user prompt
contents = [\
    types.Content(\
        role="user", parts=[types.Part(text="Turn the lights down to a romantic level")]\
    )\
]

# Send request with function declarations
response = client.models.generate_content(
    model="gemini-2.0-flash", config=config, contents=contents
)

print(response.candidates[0].content.parts[0].function_call)

```

```
import { GoogleGenAI } from '@google/genai';

// Generation Config with Function Declaration
const config = {
  tools: [{\
    functionDeclarations: [setLightValuesFunctionDeclaration]\
  }]
};

// Configure the client
const ai = new GoogleGenAI({ apiKey: process.env.GEMINI_API_KEY });

// Define user prompt
const contents = [\
  {\
    role: 'user',\
    parts: [{ text: 'Turn the lights down to a romantic level' }]\
  }\
];

// Send request with function declarations
const response = await ai.models.generateContent({
  model: 'gemini-2.0-flash',
  contents: contents,
  config: config
});

console.log(response.functionCalls[0]);

```

The model then returns a `functionCall` object in an OpenAPI compatible
schema specifying how to call one or more of the declared functions in order to
respond to the user's question.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
id=None args={'color_temp': 'warm', 'brightness': 25} name='set_light_values'

```

```
{
  name: 'set_light_values',
  args: { brightness: 25, color_temp: 'warm' }
}

```

### Step 3: Execute set\_light\_values function code

Extract the function call details from the model's response, parse the arguments
, and execute the `set_light_values` function in our code.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
# Extract tool call details
tool_call = response.candidates[0].content.parts[0].function_call

if tool_call.name == "set_light_values":
    result = set_light_values(**tool_call.args)
    print(f"Function execution result: {result}")

```

```
// Extract tool call details
const tool_call = response.functionCalls[0]

let result;
if (tool_call.name === 'set_light_values') {
  result = setLightValues(tool_call.args.brightness, tool_call.args.color_temp);
  console.log(`Function execution result: ${JSON.stringify(result)}`);
}

```

### Step 4: Create User friendly response with function result and call the model again

Finally, send the result of the function execution back to the model so it can incorporate this information into its final response to the user.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
# Create a function response part
function_response_part = types.Part.from_function_response(
    name=tool_call.name,
    response={"result": result},
)

# Append function call and result of the function execution to contents
contents.append(types.Content(role="model", parts=[types.Part(function_call=tool_call)])) # Append the model's function call message
contents.append(types.Content(role="user", parts=[function_response_part])) # Append the function response

final_response = client.models.generate_content(
    model="gemini-2.0-flash",
    config=config,
    contents=contents,
)

print(final_response.text)

```

```
// Create a function response part
const function_response_part = {
  name: tool_call.name,
  response: { result }
}

// Append function call and result of the function execution to contents
contents.push({ role: 'model', parts: [{ functionCall: tool_call }] });
contents.push({ role: 'user', parts: [{ functionResponse: function_response_part }] });

// Get the final response from the model
const final_response = await ai.models.generateContent({
  model: 'gemini-2.0-flash',
  contents: contents,
  config: config
});

console.log(final_response.text);

```

This completes the function calling flow. The Model successfully used the `set_light_values` function to perform the request action of the user.

## Function declarations

When you implement function calling in a prompt, you create a `tools` object, which contains one or more _`function declarations`_. You define functions using JSON, specifically with a [select subset](https://ai.google.dev/api/caching#Schema) of the [OpenAPI schema](https://spec.openapis.org/oas/v3.0.3#schemawr) format. A single function declaration can include the following parameters:

- `name` (string): A unique name for the function ( `get_weather_forecast`, `send_email`). Use descriptive names without spaces or special characters (use underscores or camelCase).
- `description` (string): A clear and detailed explanation of the function's purpose and capabilities. This is crucial for the model to understand when to use the function. Be specific and provide examples if helpful ("Finds theaters based on location and optionally movie title which is currently playing in theaters.").
- `parameters` (object): Defines the input parameters the function expects.

  - `type` (string): Specifies the overall data type, such as `object`.
  - `properties` (object): Lists individual parameters, each with:

    - `type` (string): The data type of the parameter, such as `string`, `integer`, `boolean, array`.
    - `description` (string): A description of the parameter's purpose and format. Provide examples and constraints ("The city and state, e.g., 'San Francisco, CA' or a zip code e.g., '95616'.").
    - `enum` (array, optional): If the parameter values are from a fixed set, use "enum" to list the allowed values instead of just describing them in the description. This improves accuracy ("enum": \["daylight", "cool", "warm"\]).
  - `required` (array): An array of strings listing the parameter names that are mandatory for the function to operate.

## Parallel Function Calling

In addition to single turn function calling, you can also call multiple
functions at once. Parallel function calling lets you execute multiple
functions at once and is used when the functions are not dependent on each
other. This is useful in scenarios like gathering data from multiple
independent sources, such as retrieving customer details from different
databases or checking inventory levels across various warehouses or performing
multiple actions such as converting your apartment into a disco.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
power_disco_ball = {
    "name": "power_disco_ball",
    "description": "Powers the spinning disco ball.",
    "parameters": {
        "type": "object",
        "properties": {
            "power": {
                "type": "boolean",
                "description": "Whether to turn the disco ball on or off.",
            }
        },
        "required": ["power"],
    },
}

start_music = {
    "name": "start_music",
    "description": "Play some music matching the specified parameters.",
    "parameters": {
        "type": "object",
        "properties": {
            "energetic": {
                "type": "boolean",
                "description": "Whether the music is energetic or not.",
            },
            "loud": {
                "type": "boolean",
                "description": "Whether the music is loud or not.",
            },
        },
        "required": ["energetic", "loud"],
    },
}

dim_lights = {
    "name": "dim_lights",
    "description": "Dim the lights.",
    "parameters": {
        "type": "object",
        "properties": {
            "brightness": {
                "type": "number",
                "description": "The brightness of the lights, 0.0 is off, 1.0 is full.",
            }
        },
        "required": ["brightness"],
    },
}

```

```
import { Type } from '@google/genai';

const powerDiscoBall = {
  name: 'power_disco_ball',
  description: 'Powers the spinning disco ball.',
  parameters: {
    type: Type.OBJECT,
    properties: {
      power: {
        type: Type.BOOLEAN,
        description: 'Whether to turn the disco ball on or off.'
      }
    },
    required: ['power']
  }
};

const startMusic = {
  name: 'start_music',
  description: 'Play some music matching the specified parameters.',
  parameters: {
    type: Type.OBJECT,
    properties: {
      energetic: {
        type: Type.BOOLEAN,
        description: 'Whether the music is energetic or not.'
      },
      loud: {
        type: Type.BOOLEAN,
        description: 'Whether the music is loud or not.'
      }
    },
    required: ['energetic', 'loud']
  }
};

const dimLights = {
  name: 'dim_lights',
  description: 'Dim the lights.',
  parameters: {
    type: Type.OBJECT,
    properties: {
      brightness: {
        type: Type.NUMBER,
        description: 'The brightness of the lights, 0.0 is off, 1.0 is full.'
      }
    },
    required: ['brightness']
  }
};

```

Call the model with an instruction that could use all of the specified tools. This example uses a `tool_config`. To learn more you can read about [configuring function calling](https://ai.google.dev/gemini-api/docs/function-calling#function_calling_modes).

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
from google import genai
from google.genai import types

# Set up function declarations
house_tools = [\
    types.Tool(function_declarations=[power_disco_ball, start_music, dim_lights])\
]

config = {
    "tools": house_tools,
    "automatic_function_calling": {"disable": True},
    # Force the model to call 'any' function, instead of chatting.
    "tool_config": {"function_calling_config": {"mode": "any"}},
}

# Configure the client
client = genai.Client(api_key=os.getenv("GEMINI_API_KEY"))

chat = client.chats.create(model="gemini-2.0-flash", config=config)
response = chat.send_message("Turn this place into a party!")

# Print out each of the function calls requested from this single call
print("Example 1: Forced function calling")
for fn in response.function_calls:
    args = ", ".join(f"{key}={val}" for key, val in fn.args.items())
    print(f"{fn.name}({args})")

```

```
import { GoogleGenAI } from '@google/genai';

// Set up function declarations
const houseFns = [powerDiscoBall, startMusic, dimLights];

const config = {
    tools: [{\
        functionDeclarations: houseFns\
    }],
    // Force the model to call 'any' function, instead of chatting.
    toolConfig: {
        functionCallingConfig: {
        mode: 'any'
        }
    }
};

// Configure the client
const ai = new GoogleGenAI({ apiKey: process.env.GEMINI_API_KEY });

// Create a chat session
const chat = ai.chats.create({
    model: 'gemini-2.0-flash',
    config: config
});
const response = await chat.sendMessage({message: 'Turn this place into a party!'});

// Print out each of the function calls requested from this single call
console.log("Example 1: Forced function calling");
for (const fn of response.functionCalls) {
    const args = Object.entries(fn.args)
        .map(([key, val]) => `${key}=${val}`)
        .join(', ');
    console.log(`${fn.name}(${args})`);
}

```

Each of the printed results reflects a single function call that the model has requested. To send the results back, include the responses in the same order as they were requested.

The Python SDK supports a feature called [automatic function calling](https://ai.google.dev/gemini-api/docs/function-calling#automatic_function_calling_python_only) which converts the Python function to declarations, handles the function call execution and response cycle for you. Following is an example for our disco use case.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)More

```
from google import genai
from google.genai import types

# Actual implementation functions
def power_disco_ball_impl(power: bool) -> dict:
    """Powers the spinning disco ball.

    Args:
        power: Whether to turn the disco ball on or off.

    Returns:
        A status dictionary indicating the current state.
    """
    return {"status": f"Disco ball powered {'on' if power else 'off'}"}

def start_music_impl(energetic: bool, loud: bool) -> dict:
    """Play some music matching the specified parameters.

    Args:
        energetic: Whether the music is energetic or not.
        loud: Whether the music is loud or not.

    Returns:
        A dictionary containing the music settings.
    """
    music_type = "energetic" if energetic else "chill"
    volume = "loud" if loud else "quiet"
    return {"music_type": music_type, "volume": volume}

def dim_lights_impl(brightness: float) -> dict:
    """Dim the lights.

    Args:
        brightness: The brightness of the lights, 0.0 is off, 1.0 is full.

    Returns:
        A dictionary containing the new brightness setting.
    """
    return {"brightness": brightness}

config = {
    "tools": [power_disco_ball_impl, start_music_impl, dim_lights_impl],
}

chat = client.chats.create(model="gemini-2.0-flash", config=config)
response = chat.send_message("Do everything you need to this place into party!")

print("\nExample 2: Automatic function calling")
print(response.text)
# I've turned on the disco ball, started playing loud and energetic music, and dimmed the lights to 50% brightness. Let's get this party started!

```

## Compositional Function Calling

Gemini 2.0 supports compositional function calling, meaning the model can chain multiple function calls together. For example, to answer "Get the temperature in my current location", the Gemini API might invoke both a `get_current_location()` function and a `get_weather()` function that takes the location as a parameter.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
# Light control schemas
turn_on_the_lights_schema = {'name': 'turn_on_the_lights'}
turn_off_the_lights_schema = {'name': 'turn_off_the_lights'}

prompt = """
  Hey, can you write run some python code to turn on the lights, wait 10s and then turn off the lights?
  """

tools = [\
    {'code_execution': {}},\
    {'function_declarations': [turn_on_the_lights_schema, turn_off_the_lights_schema]}\
]

await run(prompt, tools=tools, modality="AUDIO")

```

```
// Light control schemas
const turnOnTheLightsSchema = { name: 'turn_on_the_lights' };
const turnOffTheLightsSchema = { name: 'turn_off_the_lights' };

const prompt = `
  Hey, can you write run some python code to turn on the lights, wait 10s and then turn off the lights?
`;

const tools = [\
  { codeExecution: {} },\
  { functionDeclarations: [turnOnTheLightsSchema, turnOffTheLightsSchema] }\
];

await run(prompt, tools=tools, modality="AUDIO")

```

## Function calling modes

The Gemini API lets you control how the model uses the provided tools (function declarations). Specifically, you can set the mode within the `function_calling_config`.

- `AUTO (Default)`: The model decides whether to generate a natural language response or suggest a function call based on the prompt and context. This is the most flexible mode and recommended for most scenarios.
- `ANY`: The model is constrained to always predict a function call and guarantee function schema adherence. If `allowed_function_names` is not specified, the model can choose from any of the provided function declarations. If `allowed_function_names` is provided as a list, the model can only choose from the functions in that list. Use this mode when you require a function call in response to every prompt (if applicable).
- `NONE`: The model is _prohibited_ from making function calls. This is equivalent to sending a request without any function declarations. Use this to temporarily disable function calling without removing your tool definitions.


[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
from google.genai import types

# Configure function calling mode
tool_config = types.ToolConfig(
    function_calling_config=types.FunctionCallingConfig(
        mode="ANY", allowed_function_names=["get_current_temperature"]
    )
)

# Create the generation config
config = types.GenerateContentConfig(
    temperature=0,
    tools=[tools],  # not defined here.
    tool_config=tool_config,
)

```

```
import { FunctionCallingConfigMode } from '@google/genai';

// Configure function calling mode
const toolConfig = {
  functionCallingConfig: {
    mode: FunctionCallingConfigMode.ANY,
    allowedFunctionNames: ['get_current_temperature']
  }
};

// Create the generation config
const config = {
  temperature: 0,
  tools: tools, // not defined here.
  toolConfig: toolConfig,
};

```

## Automatic Function Calling (Python Only)

When using the Python SDK, you can provide Python functions directly as tools. The SDK automatically converts the Python function to declarations, handles the function call execution and response cycle for you. The Python SDK then automatically:

1. Detects function call responses from the model.
2. Call the corresponding Python function in your code.
3. Sends the function response back to the model.
4. Returns the model's final text response.

To use this, define your function with type hints and a docstring, and then pass the function itself (not a JSON declaration) as a tool:

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)More

```
from google import genai
from google.genai import types

# Define the function with type hints and docstring
def get_current_temperature(location: str) -> dict:
    """Gets the current temperature for a given location.

    Args:
        location: The city and state, e.g. San Francisco, CA

    Returns:
        A dictionary containing the temperature and unit.
    """
    # ... (implementation) ...
    return {"temperature": 25, "unit": "Celsius"}

# Configure the client and model
client = genai.Client(api_key=os.getenv("GEMINI_API_KEY"))  # Replace with your actual API key setup
config = types.GenerateContentConfig(
    tools=[get_current_temperature]
)  # Pass the function itself

# Make the request
response = client.models.generate_content(
    model="gemini-2.0-flash",
    contents="What's the temperature in Boston?",
    config=config,
)

print(response.text)  # The SDK handles the function call and returns the final text

```

You can disable automatic function calling with:

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)More

```
# To disable automatic function calling:
config = types.GenerateContentConfig(
    tools=[get_current_temperature],
    automatic_function_calling=types.AutomaticFunctionCallingConfig(disable=True)
)

```

### Automatic Function schema declaration

Automatic schema extraction from Python functions doesn't work in all cases. For example: it doesn't handle cases where you describe the fields of a nested dictionary-object. The API is able to describe any of the following types:

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)More

```
AllowedType = (int | float | bool | str | list['AllowedType'] | dict[str, AllowedType])

```

To see what the inferred schema looks like, you can convert it using [`from_callable`](https://googleapis.github.io/python-genai/genai.html#genai.types.FunctionDeclaration.from_callable):

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)More

```
def multiply(a: float, b: float):
    """Returns a * b."""
    return a * b

fn_decl = types.FunctionDeclaration.from_callable(callable=multiply, client=client)

# to_json_dict() provides a clean JSON representation.
print(fn_decl.to_json_dict())

```

## Multi-tool use: Combine Native Tools with Function Calling

With Gemini 2.0, you can enable multiple tools combining native tools with function calling at the same time. Here's an example that enables two tools, [Grounding with Google Search](https://ai.google.dev/gemini-api/docs/grounding) and [code execution](https://ai.google.dev/gemini-api/docs/code-execution), in a request using the [Live API](https://ai.google.dev/gemini-api/docs/live).

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
# Multiple tasks example - combining lights, code execution, and search
prompt = """
  Hey, I need you to do three things for me.

    1.  Turn on the lights.
    2.  Then compute the largest prime palindrome under 100000.
    3.  Then use Google Search to look up information about the largest earthquake in California the week of Dec 5 2024.

  Thanks!
  """

tools = [\
    {'google_search': {}},\
    {'code_execution': {}},\
    {'function_declarations': [turn_on_the_lights_schema, turn_off_the_lights_schema]} # not defined here.\
]

# Execute the prompt with specified tools in audio modality
await run(prompt, tools=tools, modality="AUDIO")

```

```
// Multiple tasks example - combining lights, code execution, and search
const prompt = `
  Hey, I need you to do three things for me.

    1.  Turn on the lights.
    2.  Then compute the largest prime palindrome under 100000.
    3.  Then use Google Search to look up information about the largest earthquake in California the week of Dec 5 2024.

  Thanks!
`;

const tools = [\
  { googleSearch: {} },\
  { codeExecution: {} },\
  { functionDeclarations: [turnOnTheLightsSchema, turnOffTheLightsSchema] } // not defined here.\
];

// Execute the prompt with specified tools in audio modality
await run(prompt, {tools: tools, modality: "AUDIO"});

```

Python developers can try this out in the [Live API Tool Use notebook](https://github.com/google-gemini/cookbook/blob/main/quickstarts/Get_started_LiveAPI_tools.ipynb).

## Use Model Context Protocol (MCP)

[Model Context Protocol (MCP)](https://modelcontextprotocol.io/introduction) is an open standard to connect AI applications with external tools, data sources, and systems. MCP provides a common protocol for models to access context, such as functions (tools), data sources (resources), or predefined prompts. You can use models with MCP server using their tool calling capabilities.

MCP servers expose the tools as JSON schema definitions, which can be used with Gemini compatible function declarations. This lets you to use a MCP server with Gemini models directly. Here, you can find an example of how to use a local MCP server with Gemini SDK and the `mcp` SDK.

[Python](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#python)[JavaScript](https://ai.google.dev/gemini-api/docs/function-calling?example=meeting#javascript)More

```
import asyncio
import os
from datetime import datetime
from google import genai
from google.genai import types
from mcp import ClientSession, StdioServerParameters
from mcp.client.stdio import stdio_client

client = genai.Client(api_key=os.getenv("GEMINI_API_KEY"))

# Create server parameters for stdio connection
server_params = StdioServerParameters(
    command="npx",  # Executable
    args=["-y", "@philschmid/weather-mcp"],  # Weather MCP Server
    env=None,  # Optional environment variables
)

async def run():
    async with stdio_client(server_params) as (read, write):
        async with ClientSession(read, write) as session:
            # Prompt to get the weather for the current day in London.
            prompt = f"What is the weather in London in {datetime.now().strftime('%Y-%m-%d')}?"
            # Initialize the connection between client and server
            await session.initialize()

            # Get tools from MCP session and convert to Gemini Tool objects
            mcp_tools = await session.list_tools()
            tools = [\
                types.Tool(\
                    function_declarations=[\
                        {\
                            "name": tool.name,\
                            "description": tool.description,\
                            "parameters": {\
                                k: v\
                                for k, v in tool.inputSchema.items()\
                                if k not in ["additionalProperties", "$schema"]\
                            },\
                        }\
                    ]\
                )\
                for tool in mcp_tools.tools\
            ]

            # Send request to the model with MCP function declarations
            response = client.models.generate_content(
                model="gemini-2.0-flash",
                contents=prompt,
                config=types.GenerateContentConfig(
                    temperature=0,
                    tools=tools,
                ),
            )

            # Check for a function call
            if response.candidates[0].content.parts[0].function_call:
                function_call = response.candidates[0].content.parts[0].function_call
                print(function_call)
                # Call the MCP server with the predicted tool
                result = await session.call_tool(
                    function_call.name, arguments=function_call.args
                )
                print(result.content[0].text)
                # Continue as shown in step 4 of "How Function Calling Works"
                # and create a user friendly response
            else:
                print("No function call found in the response.")
                print(response.text)

# Start the asyncio event loop and run the main function
asyncio.run(run())

```

```
import { GoogleGenAI } from '@google/genai';
import { Client } from "@modelcontextprotocol/sdk/client/index.js";
import { StdioClientTransport } from "@modelcontextprotocol/sdk/client/stdio.js";

// Create server parameters for stdio connection
const serverParams = new StdioClientTransport({
  command: "npx",
  args: ["-y", "@philschmid/weather-mcp"]
});

const client = new Client(
  {
    name: "example-client",
    version: "1.0.0"
  }
);

// Configure the client
const ai = new GoogleGenAI({ apiKey: process.env.GEMINI_API_KEY });

// Initialize the connection between client and server
await client.connect(serverParams);

// Get tools from MCP session and convert to Gemini Tool objects
const mcpTools = await client.listTools();
const tools = mcpTools.tools.map((tool) => {
  // Filter the parameters to exclude not supported keys
  const parameters = Object.fromEntries(
    Object.entries(tool.inputSchema).filter(([key]) => !["additionalProperties", "$schema"].includes(key))
  );
  return {
    name: tool.name,
    description: tool.description,
    parameters: parameters
  };
});

// Send request to the model with MCP function declarations
const response = await ai.models.generateContent({
  model: "gemini-2.0-flash",
  contents: "What is the weather in London in the UK on 2024-04-04?",
  config: {
    tools: [{\
      functionDeclarations: tools\
    }],
  },
});

// Check for function calls in the response
if (response.functionCalls && response.functionCalls.length > 0) {
  const functionCall = response.functionCalls[0]; // Assuming one function call
  console.log(`Function to call: ${functionCall.name}`);
  console.log(`Arguments: ${JSON.stringify(functionCall.args)}`);
  // Call the MCP server with the predicted tool
  const result = await client.callTool({name: functionCall.name, arguments: functionCall.args});
  console.log(result.content[0].text);
  // Continue as shown in step 4 of "How Function Calling Works"
  // and create a user friendly response
} else {
  console.log("No function call found in the response.");
  console.log(response.text);
}

// Close the connection
await client.close();

```

## Supported Models

Experimental models are not included. You can find their capabilities on the [model overview](https://ai.google.dev/gemini-api/docs/models) page.

| Model | Function Calling | Parallel Function Calling | Compositional Function Calling<br>(Live API only) |
| --- | --- | --- | --- |
| Gemini 2.0 Flash | ✔️ | ✔️ | ✔️ |
| Gemini 2.0 Flash-Lite | X | X | X |
| Gemini 1.5 Flash | ✔️ | ✔️ | ✔️ |
| Gemini 1.5 Pro | ✔️ | ✔️ | ✔️ |

## Best Practices

- **Function and Parameter Descriptions:** Be extremely clear and specific in your descriptions. The model relies on these to choose the correct function and provide appropriate arguments.
- **Naming:** Use descriptive function names (without spaces, periods, or dashes).
- **Strong Typing:** Use specific types (integer, string, enum) for parameters to reduce errors. If a parameter has a limited set of valid values, use an enum.
- **Tool Selection:** While the model can use an arbitrary number of tools, providing too many can increase the risk of selecting an incorrect or suboptimal tool. For best results, aim to provide only the relevant tools for the context or task, ideally keeping the active set to a maximum of 10-20. Consider dynamic tool selection based on conversation context if you have a large total number of tools.
- **Prompt Engineering:**
  - Provide context: Tell the model its role (e.g., "You are a helpful weather assistant.").
  - Give instructions: Specify how and when to use functions (e.g., "Don't guess dates; always use a future date for forecasts.").
  - Encourage clarification: Instruct the model to ask clarifying questions if needed.
- **Temperature:** Use a low temperature (e.g., 0) for more deterministic and reliable function calls.
- **Validation:** If a function call has significant consequences (e.g., placing an order), validate the call with the user before executing it.
- **Error Handling**: Implement robust error handling in your functions to gracefully handle unexpected inputs or API failures. Return informative error messages that the model can use to generate helpful responses to the user.
- **Security:** Be mindful of security when calling external APIs. Use appropriate authentication and authorization mechanisms. Avoid exposing sensitive data in function calls.
- **Token Limits:** Function descriptions and parameters count towards your input token limit. If you're hitting token limits, consider limiting the number of functions or the length of the descriptions, break down complex tasks into smaller, more focused function sets.

## Notes and Limitations

- Only a [subset of the OpenAPI schema](https://ai.google.dev/api/caching#FunctionDeclaration) is supported.
- Supported parameter types in Python are limited.
- Automatic function calling is a Python SDK feature only.

Was this helpful?



 Send feedback



Except as otherwise noted, the content of this page is licensed under the [Creative Commons Attribution 4.0 License](https://creativecommons.org/licenses/by/4.0/), and code samples are licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). For details, see the [Google Developers Site Policies](https://developers.google.com/site-policies). Java is a registered trademark of Oracle and/or its affiliates.

Last updated 2025-05-13 UTC.

The new page has loaded.
