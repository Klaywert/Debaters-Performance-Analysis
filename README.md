# Debaters-Performance-Analysis


## PROMPT 1

You are tasked to analyze the performance of debaters in a DEBATE. The speeches are in Brazilian Portuguese. The input is a text containing the instructions and the speeches of debaters and the moderator, who proposes the dynamics of the debate. Each speech is associated with a speaker, indicated by their label written in uppercase (e.g., ""-MODERATOR: ""Seja bem-vindo ao debate."" or ""-DEBATER 1: Obrigado!""). It's important to note that the moderator also plays a crucial role in the debate by proposing questions that are subsequently answered by the debaters. The theme of the debate is ""Generative AI and its impacts on society."" Your goal is to analyze and evaluate the debater's performance. The response should include each debater's Overall Score both the analysis of debaters and the Evaluation Criteria adopted, including the overall scoring.

Instructions:
Analyze the provided debate, evaluating the performance of each debater based on their speeches; 
Inform the evaluation criteria adopted;
For each debater, assign an overall score and provide an explanation of their performance evaluation.
Please think critically before responding.

Evaluation Criteria:
The model is free to choose its own evaluation criteria, but must take into account the theme of the debate. It's essential to consider the contributions of the moderator in shaping the debate and guiding the discussion through their questions.

Overall Score:

The model should assign a score (in a 0-10 scale) to each debater based on the chosen Evaluation Criteria, considering their responses to the moderator's questions and their overall contribution to the debate. Provide justification for the overall score assigned, explaining how it reflects the debater's performance in the debate.

OUTPUT: 

The output is a .json format file , following the example below:

{
  ""evaluation_criteria"": ""..."",
  ""debaters"": [
    {
      ""name"": ""Debater 1"",
      ""overall_score"": 8.5,
      ""performance_evaluation"": ""...""
    },
    {
      ""name"": ""Debater 2"",
      ""overall_score"": 9.9,
      ""performance_evaluation"": ""...""
    }
  ]
}


DEBATE:"

## PROMPT 2

You are tasked to analyze the performance of debaters in a debate. The input is a text containing the instructions and the speeches of debaters and the moderator (labeled DEBATE, in brazilian portuguese), who proposes the dynamics of the debate. Each speech is associated with a speaker, indicated by their label written in uppercase (e.g., ""- DEBATER 1: Hi, how are you?"" or ""-MODERATOR: ""Good""). It's important to note that the moderator also plays a crucial role in the debate by proposing questions that are subsequently answered by the debaters. The theme of the debate is ""Generative AI and its impacts on society."" Your goal is to analyze and evaluate the debaters based on their performance and assign an overall score. The response should include both the evaluation of debaters and the overall scoring based on the evaluation criteria.

Instructions:

Analyze the provided text, which contains the speeches of debaters and the moderator;
Evaluate the performances of debaters based on the Evaluation Criteria section, but also based on their speeches, and considering their responses to the moderator's questions;
Assign an individual overall score (in a 0-10 scale) to each debater, for each evaluation criteria provided.
Please think critically before responding.

Evaluation Criteria:

1. Argumentation. Argumentation in a debate refers to the presentation of arguments, reasons, evidence, and logic to support a position or point of view in a structured discussion. It involves the skill of formulating solid and convincing arguments that defend a thesis, opinion, or perspective to persuade the audience or debate participants. That includes: argument relevance, evidence, argument coherence and argument cohesion.

2. Persuasion. The skill of being persuasive in academic debates involves the ability of debaters to present their arguments and viewpoints in a compelling and convincing manner. It is the capacity to influence the beliefs, opinions, and decisions of the audience and, in some cases, the evaluators or judges. That includes: Eloquence and Convincingness.

3. Engagement. The skill of involvement and engagement in academic debates can be understood as the degree of a debater’s active participation and commitment to the discussion.

4. Adaptability. The skill of adaptability in academic debates refers to a debater’s ability to adjust and respond effectively to changing circumstances, including shifts in the debate’s dynamics, new arguments, questions or information, and the reactions of the audience or opponents. It is the capacity to be flexible and responsive during the debate.


OUTPUT: 

The output is a .json format file , following the example below:

{
  ""debaters"": [
    {
      ""name"": ""Debater 1"",
      ""overall_score"": 8.5,
      ""scores"": {
        ""argumentation"": 8.7,
        ""persuasion"": 8.8,
        ""engagement"": 8.4,
        ""adaptability"": 8.2
      },
      ""performance"": {
        ""performance_analysis"": ""...""
      }
    },
    {
      ""name"": ""Debater 2"",
      ""overall_score"": 7.9,
      ""scores"": {
        ""argumentation"": 8.0,
        ""persuasion"": 7.8,
        ""engagement"": 7.9,
        ""adaptability"": 7.6
      },
      ""performance"": {
        ""performance_analysis"": ""...""
      }
    }
  ]
}


DEBATE:"


## PROMPT 3

You are tasked to analyze the performance of debaters in a debate. The input is a text containing the instructions and the speeches of debaters and the moderator (labeled DEBATE, in brazilian portuguese), who proposes the dynamics of the debate. Each speech is associated with a speaker, indicated by their label written in uppercase (e.g., ""- DEBATER 1: Hi, how are you?"" or ""-MODERATOR: ""Good""). It's important to note that the moderator also plays a crucial role in the debate by proposing questions that are subsequently answered by the debaters. The theme of the debate is ""Generative AI and its impacts on society."" 
Your goal is to evaluate the performance of each debater based on occurrences of positive and negative events related to some definitions that can be found in the Definitions section.

Instructions:

For each debater, identify instances of positive and negative events throughout the debate;
List short descriptions of the instances found. Ensure that the descriptions are specific and not overly general;
Multiple instances of the same event type must be considered as a distinct item in the list;
Provide an overall performance analysis for each debater.
Please think critically before responding.


Definitions:

1. Argumentation. Argumentation in a debate refers to the presentation of arguments, reasons, evidence, and logic to support a position or point of view in a structured discussion. It involves the skill of formulating solid and convincing arguments that defend a thesis, opinion, or perspective to persuade the audience or debate participants. That includes: argument relevance, evidence, argument coherence and argument cohesion.

2. Persuasion. The skill of being persuasive in academic debates involves the ability of debaters to present their arguments and viewpoints in a compelling and convincing manner. It is the capacity to influence the beliefs, opinions, and decisions of the audience and, in some cases, the evaluators or judges. That includes: Eloquence and Convincingness.

3. Engagement. The skill of involvement and engagement in academic debates can be understood as the degree of a debater’s active participation and commitment to the discussion.

4. Adaptability: a debater’s ability to adjust and respond effectively to changing circumstances, including shifts in the debate’s dynamics, new arguments, questions or information, and the reactions of the audience or opponents. It is the capacity to be flexible and responsive during the debate. 

Events:

A. Positive Events:

1. Relevant Argumentation: Presenting arguments directly related to the topic under discussion, supported by relevant evidence and examples.
2. Credible Evidence: Using reliable sources and solid data to substantiate the arguments presented.
3. Coherence and Cohesion: Clearly and logically articulating arguments while maintaining a cohesive and coherent structure throughout the debate.
4. Eloquent Persuasion: Articulating persuasively to captivate the audience and convey viewpoints convincingly.
5. Conviction in Arguments: Demonstrating conviction and confidence in one's ideas, conveying credibility to the presented arguments.
6. Active Engagement: Actively participating in the debate, showing genuine interest in the topic, and engaging constructively with other debaters.
7. Adaptability to Questions and Rebuttals: Effectively responding to the moderator's questions and other debaters' rebuttals promptly while maintaining the consistency of arguments.

B. Negative Events:

1. Irrelevant Argumentation: Presenting arguments that are not directly related to the topic at hand, diverting attention from the core debate topic.
2. Lack of Evidence or Unreliable Sources: Using unsupported information or questionable sources, undermining the credibility of arguments.
3. Lack of Coherence and Cohesion: Lack of clarity in articulating arguments, resulting in a confusing and inconsistent structure.
4. Ineffective Persuasion: Expressing arguments in an unconvincing manner, struggling to convey viewpoints persuasively and interestingly to the audience.
5. Lack of Conviction: Displaying hesitation or lack of confidence in one's ideas, weakening the persuasiveness of arguments.
6. Passive or Distracted Engagement: Demonstrating passive participation or lack of engagement with the topic or arguments presented by other debaters.
7. Difficulty in Adapting to Questions and Rebuttals: Providing inadequate responses or struggling to address the moderator's questions and other debaters' rebuttals, indicating insufficient preparation or understanding of the topic.


Output: 

The output is a .json format file , following the example below (Debate theme: Impacts of IA on Medicine):

{
  ""debaters"": [
    {
      ""name"": ""Debater 1"",
      ""positive_events"": {
        ""relevant_argumentation"": [
          ""Provided a detailed analysis on the ethical impacts of AI in patient privacy"",
          ""Provided a detailed analysis on the social impacts of AI in improving healthcare accessibility"",
          ""Provided a detailed analysis on the economic impacts of AI in reducing medical costs"",
          ""Presented a strong argument on the benefits of AI in diagnostic accuracy""
        ],
        ""credible_evidence"": [
          ""Cited recent studies from reputable medical journals on AI in radiology"",
          ""Used statistical data effectively to show the reduction in diagnostic errors due to AI""
        ],
        ""coherence_and_cohesion"": [
          ""Maintained a clear structure throughout the debate, starting with ethical implications and progressing to economic benefits"",
          ""Connected points logically, showing how ethical considerations impact economic outcomes""
        ],
        ""eloquent_persuasion"": [
          ""Used rhetorical questions effectively to engage the audience on the importance of ethical AI""
        ],
        ""conviction_in_arguments"": [
          ""Spoke passionately about the potential of AI to revolutionize medicine"",
          ""Maintained a firm stance on the necessity of AI in early diagnosis and treatment""
        ],
        ""active_engagement"": [
          ""Engaged with the audience through sustained eye contact""
        ],
        ""adaptability"": [
          ""Adapted arguments when new points were raised by the opponent"",
          ""Acknowledged counterarguments gracefully and provided well-reasoned rebuttals""
        ]
      },
      ""negative_events"": {
        ""irrelevant_argumentation"": [
          ""Discussed the use of AI in unrelated fields like agriculture"",
          ""Mentioned advancements in AI for autonomous vehicles which were off-topic""
        ],
        ""lack_of_evidence"": [
          ""Failed to provide sources for claims about AI replacing doctors entirely"",
          ""Made broad statements about AI without backing them up with specific data""
        ],
        ""lack_of_coherence_and_cohesion"": [],
        ""ineffective_persuasion"": [],
        ""lack_of_conviction"": [],
        ""distracted_engagement"": [
          ""Lost focus during the opponent's speech, appearing disinterested""
        ],
        ""difficulty_in_adapting"": []
      },
      ""performance"": {
        ""performance_analysis"": ""Debater 1 presented well-structured arguments and robust evidence to support their positions, standing out in clarity and persuasive ability. They demonstrated a deep knowledge of the subject and effectively responded to questions from opponents and the audience.""
      }
    },
    {
      ""name"": ""Debater 2"",
      ""positive_events"": {
        ""relevant_argumentation"": [
          ""Discussed the potential job creation from AI development in the medical field"",
          ""Highlighted the role of AI in personalizing patient care plans""
        ],
        ""credible_evidence"": [
          ""Referenced government reports on AI impact on healthcare systems"",
          ""Cited case studies where AI improved patient outcomes"",
          ""Mentioned peer-reviewed articles on AI in predictive analytics""
        ],
        ""coherence_and_cohesion"": [
          ""Structured arguments in a logical sequence from AI development to implementation""
        ],
        ""eloquent_persuasion"": [
          ""Used metaphors to illustrate complex AI concepts in simple terms"",
          ""Utilized personal stories of patients benefitting from AI""
        ],
        ""conviction_in_arguments"": [
          ""Showed enthusiasm for the potential of AI in preventative care"",
          ""Maintained a positive outlook on AI's role in medical advancements""
        ],
        ""active_engagement"": [
          ""Asked the opponent clarifying questions to challenge their points""
        ],
        ""adaptability"": [
          ""Modified stance slightly in response to new information provided by the opponent""
        ]
      },
      ""negative_events"": {
        ""irrelevant_argumentation"": [
          ""Mentioned unrelated technology advancements in non-medical fields"",
          ""Discussed AI in entertainment which was not relevant to the topic""
        ],
        ""lack_of_evidence"": [
          ""Failed to provide sources for some claims about AI's long-term impacts""
        ],
        ""lack_of_coherence_and_cohesion"": [
          ""Arguments lacked a clear connection at times between points on AI and patient care""
        ],
        ""ineffective_persuasion"": [
          ""Some analogies were confusing and did not clearly support the arguments""
        ],
        ""lack_of_conviction"": [
          ""Appeared unsure about certain statements regarding AI ethics"",
          ""Showed hesitation when discussing AI's potential drawbacks""
        ],
        ""distracted_engagement"": [
          ""Lost focus during opponent's speech, appearing disinterested"",
          ""Frequently checked notes, breaking the flow of engagement""
        ],
        ""difficulty_in_adapting"": [
          ""Struggled to counter unexpected arguments about AI biases"",
          ""Had difficulty addressing questions about AI's role in specific medical procedures""
        ]
      },
      ""performance"": {
        ""performance_analysis"": ""Debater 2 performed well, with convincing arguments and a good understanding of the topic. However, at times, their responses were less detailed, and they struggled to refute some critical points raised by the opponent.""
      }
    }
  ]
}


DEBATE:"

## PROMPT 4

You are tasked to analyze the performance of debaters in a debate. The input is a text containing the instructions and the speeches of debaters and the moderator (labeled DEBATE, in brazilian portuguese), who proposes the dynamics of the debate. Each speech is associated with a speaker, indicated by their label written in uppercase (e.g., ""- DEBATER 1: Hi, how are you?"" or ""-MODERATOR: ""Good""). It's important to note that the moderator also plays a crucial role in the debate by proposing questions that are subsequently answered by the debaters. The theme of the debate is ""Generative AI and its impacts on society."" 
Your goal is to evaluate the performance of each debater based on the occurrences of evaluation aspects (Evaluation Aspects section) that are related to some definitions that can be found in the Definitions section.

Instructions:

For each debater, identify instances of Evaluation Aspects throughout the debate. These aspects can manifest in both positive and negative ways. The goal is to measure how positive or how negative the performance was, using a Likert scale. The Likert scale ranges from Very Good (+3), Good (+2), Acceptable (+1), Poor (-1), to Very Poor (-3).
List short descriptions of the instances found. Ensure that the descriptions are specific and not overly general. At the end of each instance, show the attributed score. For example: ""[Used statistics (+1), Provided some information that is not real (-3)]"".
Multiple instances of the same aspect (positive or negative) type must be considered as a distinct item in the list;
For each evaluation aspect, assign a score that considers the sum of the scores attributed to that aspect. The score should accurately reflect the sum of the scores assigned to the occurrences in each evaluation aspect.
Provide an overall performance analysis for each debater.
Please think critically before responding.


Definitions:

1. Argumentation. Argumentation in a debate refers to the presentation of arguments, reasons, evidence, and logic to support a position or point of view in a structured discussion. It involves the skill of formulating solid and convincing arguments that defend a thesis, opinion, or perspective to persuade the audience or debate participants. That includes: argument relevance, evidence, argument coherence and argument cohesion.

2. Persuasion. The skill of being persuasive in academic debates involves the ability of debaters to present their arguments and viewpoints in a compelling and convincing manner. It is the capacity to influence the beliefs, opinions, and decisions of the audience and, in some cases, the evaluators or judges. That includes: Eloquence and Convincingness.

3. Engagement. The skill of involvement and engagement in academic debates can be understood as the degree of a debater’s active participation and commitment to the discussion.

4. Adaptability. Debater’s ability to adjust and respond effectively to changing circumstances, including shifts in the debate’s dynamics, new arguments, questions or information, and the reactions of the audience or opponents. It is the capacity to be flexible and responsive during the debate. 

Evaluation Aspects:

Argumentation Quality: The overall quality of presenting arguments, combining relevant argumentation from Positive Events and irrelevant argumentation from Negative Events.
Evidence Quality: The overall reliability and strength of evidence used to support arguments, combining credible evidence from Positive Events and lack of evidence or unreliable sources from Negative Events.
Coherence and Structure: The overall clarity, coherence, and structure in articulating arguments, combining coherence and cohesion from Positive Events and lack of coherence and cohesion from Negative Events.
Persuasion Quality: The overall effectiveness and persuasiveness in articulating viewpoints, combining eloquent persuasion from Positive Events and ineffective persuasion from Negative Events.
Conviction and Confidence: The overall level of conviction and confidence demonstrated in presenting ideas, combining conviction in arguments from Positive Events and lack of conviction from Negative Events.
Engagement Level: The overall level of active participation, interest, and engagement in the debate, combining active engagement from Positive Events and passive or distracted engagement from Negative Events.
Adaptability and Responsiveness: The overall ability to adapt to questions, counter arguments, and maintain consistency, combining adaptability to questions and rebuttals from Positive Events and difficulty in adapting to questions and rebuttals from Negative Events.

Output: 

The output is a .json format file , following the example below:

{
  ""debaters"": [
    {
      ""name"": ""Debater 1"",
      ""evaluation_aspects"": {
        ""argumentation_quality"": {
          ""score"": 8,
          ""occurrences"": [""Provided a detailed analysis on the ethical impacts (+3)"", ""Presented a strong argument on economic benefits (+3)"", ""Highlighted the potential risks of AI in medical decision-making (+2)""]
        },
        ""evidence_quality"": {
          ""score"": 11,
          ""occurrences"": [""Cited recent studies from reputable journals (+3)"", ""Used statistical data effectively (+3)"", ""Referenced case studies on AI implementation in healthcare (+2)"", ""Quoted expert opinions from medical professionals (+3)""]
        },
        ""coherence_and_structure"": {
          ""score"": 5,
          ""occurrences"": [""Maintained a clear structure throughout the debate (+3)"", ""Connected points logically (+2)""]
        },
        ""persuasion_quality"": {
          ""score"": 6,
          ""occurrences"": [""Used rhetorical questions effectively (+2)"", ""Displayed confident body language (+2)"", ""Maintained eye contact with the audience (+2)""]
        },
        ""conviction_and_confidence"": {
          ""score"": 8,
          ""occurrences"": [""Spoke passionately about the subject (+3)"", ""Maintained a firm stance (+2)"", ""Expressed strong belief in the positive impacts of AI in patient care (+3)""]
        },
        ""engagement_level"": {
          ""score"": 2,
          ""occurrences"": [""Engaged with the audience through eye contact (+1)"", ""Responded promptly to questions (+1)"", ""Listened attentively to opponents' arguments (+1)"", ""Missed some audience questions (-1)""]
        },
        ""adaptability_and_responsiveness"": {
          ""score"": 3,
          ""occurrences"": [""Adapted arguments when new points were raised (+2)"", ""Acknowledged counterarguments gracefully (+1)""]
        }
      },
      ""performance"": {
        ""performance_analysis"": ""Debater 1 presented well-structured arguments and robust evidence to support their positions, standing out in clarity and persuasive ability. They demonstrated a deep knowledge of the subject and effectively responded to questions from opponents and the audience.""
      }
    },
    {
      ""name"": ""Debater 2"",
      ""evaluation_aspects"": {
        ""argumentation_quality"": {
          ""score"": 3,
          ""occurrences"": [""Discussed the potential job creation from AI development (+3)"", ""Analyzed the ethical implications of AI in patient-doctor relationships (+2)"", ""Failed to address potential ethical concerns raised by the opponent (-2)""]
        },
        ""evidence_quality"": {
          ""score"": 6,
          ""occurrences"": [""Referenced government reports on AI impact (+2)"", ""Cited recent medical studies on AI in disease diagnosis (+3)"", ""Provided examples of successful AI implementation in hospitals (+2)"", ""Mentioned potential ethical concerns without adequate evidence (-1)""]
        },
        ""coherence_and_structure"": {
          ""score"": 2,
          ""occurrences"": [""Structured arguments in a logical sequence (+2)"", ""Maintained coherence in transitions between points (+2)"", ""Jumped between points without clear connections (-2)""]
        },
        ""persuasion_quality"": {
          ""score"": 2,
          ""occurrences"": [""Used metaphors to illustrate points (+2)"", ""Emphasized the urgency of AI integration in healthcare (+2)"", ""Used overly complex language that may have confused some listeners (-2)""]
        },
        ""conviction_and_confidence"": {
          ""score"": 2,
          ""occurrences"": [""Showed enthusiasm for the topic (+2)"", ""Maintained a positive outlook on AI's role in medical advancements (+3)"", ""Expressed uncertainty when addressing some audience questions (-3)""]
        },
        ""engagement_level"": {
          ""score"": -1,
          ""occurrences"": [""Asked the opponent clarifying questions (+1)"", ""Listened attentively to opponents' arguments (+1)"", ""Missed some audience questions (-1)""]
        },
        ""adaptability_and_responsiveness"": {
          ""score"": -2,
          ""occurrences"": [""Modified stance slightly in response to new information (+1)"", ""Failed to address opponent's rebuttals (-3)""]
        }
      },
      ""performance"": {
        ""performance_analysis"": ""Debater 2 performed below expectations, showing inconsistencies in argumentation and failing to address key points raised by the opponent. Their lack of engagement and adaptability hindered their overall performance.""
      }
    }
  ]
}


DEBATE:"
