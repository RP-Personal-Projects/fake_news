# fake_news


Key Aspects of Fake News Detection
Definition and Types

Fake news: Deliberately fabricated information mimicking news media content but lacking journalistic standards and practices
Misinformation: False information shared without malicious intent
Disinformation: False information deliberately created and shared to cause harm
Satire/Parody: Content using humor that may be misinterpreted as factual
Clickbait: Sensationalized headlines designed to generate clicks, often with misleading content


Fake News Detection Methods
•
Content-Based Methods
◦
Textual Analysis
▪
Linguistic Features
•
Lexical (e.g., word frequencies, n-grams, TF, TF-IDF)
•
Syntactic (e.g., sentence structure)
•
Semantic (e.g., meaning of words and sentences)
▪
Word Embeddings (Context-Independent)
•
Word2Vec
•
GloVe [8, 10, 49, 61, 66–70, 112, 123, 35]
•
fastText
▪
Transformer Models (Context-Dependent)
•
BERT
•
DistilBERT
•
RoBERTa
•
BART
•
ELECTRA
•
XLNet
•
GPT
•
GPT-2
▪
Count-Based Methods
•
Bag-of-Words (BOW)
◦
Style-Based Features
▪
Analysing writing patterns and characteristics
◦
Visual-Based Features
▪
Analysis of images and videos
◦
Knowledge-Based Approaches
▪
Fact-checking against Knowledge Bases (KGs) (e.g., Freebase, YAGO, Probase)
▪
Entity linking and conceptualisation
▪
Knowledge fusion and comparison
•
Social Context-Based Methods
◦
Credibility-Based Techniques
▪
Assessing the reliability of users and sources
▪
Analysing user profiles
◦
Propagation-Based Methods
▪
Analysing how fake news spreads online
▪
Studying network structures
▪
Using Graph Neural Networks (GCNs) to model propagation
•
Hybrid Methods
◦
Combining content-based and social context-based features
◦
Multi-modal fake news detection (using text, images, etc.)
•
Deep Learning-Based Methods
◦
Convolutional Neural Networks (CNNs)
◦
Recurrent Neural Networks (RNNs)
▪
Long Short-Term Memory (LSTM)
▪
Gated Recurrent Units (GRU)
◦
Graph Neural Networks (GNNs)
◦
Transformer Models
◦
Hybrid Deep Learning Models (e.g., combining CNNs and RNNs)
•
Methods Based on Intrinsic Characteristics
◦
Intentional feature-based approaches: Identifying features related to the intent behind creating fake news.
◦
Propagation-based approaches: Analysing propagation structures to infer veracity.
◦
Stance-based approaches: Using user viewpoints to detect fake news.
This mind map provides a structured overview of the broad methods used in fake news detection, drawing from the information in the provided sources and our previous conversation.



Zhou et al. [5] categorize current techniques into knowledge-based methods, style-based approaches, propagation-based algorithms and credibility-based networks. 

Zhang et al. [46] review the fake news detection mechanisms corresponding to three types of features of fake news, such as creator/user-based, news content-based and social context-based features.

This paper

- Intentional creation
  Unlike real news that reports real events, fake news is usually created with intention
- Heteromorphic transmission
  Real news is usually spread by ordinary users, while fake news however tends to be propagated by diverse types of users, which thereby results in heteromorphic transmission patterns. For example, as pointed out by Ma et al. [26], fake news is typically posted by a low-impact user first and then widely spread by opinion leaders, while real news is usually initiated by an opinion leader and spread by normal users.
- Controversial reception
People are more likely to hold different views towards fake news than real news. 


Given this techniques are characterised into:
- intentional feature based
- propagation based
- stance bases


Types of disinformation

| Information Type | Authenticity    | Intention                   |
|:----------------|:----------------|:----------------------------|
| Fake News       | Verified False  | Intentionally Deceptive     |
| Misinformation  | False           | Not Intentionally Deceptive |
| Rumor           | Unverified      | Unknown Intention           |

As shown in Table 1, intentional features of fake news can be categorized into four types: misleading the public, manipulating opinions, attracting user attention and other general features.


https://firstdraftnews.org/wp-content/uploads/2019/10/Information_Disorder_Digital_AW.pdf



The Ambiguity Problem

Definitional chaos: There's no universal definition of "fake news" because it encompasses many phenomena (misinformation, disinformation, malinformation) with different intents, formats, and severities.
Taxonomical fragmentation: Different researchers focus on different aspects (content, source, spread patterns, intent), creating overlapping taxonomies rather than a unified framework.
System classification confusion: Detection systems vary by methodology (AI/ML, crowd-sourcing, expert verification), features analyzed (linguistic, network, user behavior), and objectives (early detection vs. deep verification).
Market immaturity: Despite academic research, commercial products are limited by technical challenges, platform-specific constraints, and the evolving nature of misinformation.

The Ambiguity Problem

Definitional chaos: There's no universal definition of "fake news" because it encompasses many phenomena (misinformation, disinformation, malinformation) with different intents, formats, and severities.
Taxonomical fragmentation: Different researchers focus on different aspects (content, source, spread patterns, intent), creating overlapping taxonomies rather than a unified framework.
System classification confusion: Detection systems vary by methodology (AI/ML, crowd-sourcing, expert verification), features analyzed (linguistic, network, user behavior), and objectives (early detection vs. deep verification).
Market immaturity: Despite academic research, commercial products are limited by technical challenges, platform-specific constraints, and the evolving nature of misinformation.


| Type of Mis/Disinformation | Description | Threat Level | Detection Needs |
|----------------------------|-------------|--------------|-----------------|
| Satire/Parody | Content with no intention to harm but potential to fool | Low | Context recognition, source verification |
| Misleading Content | Misleading use of information to frame issues or individuals | Medium | Fact verification, source tracking |
| Imposter Content | Impersonation of genuine sources | High | Authentication systems, digital signatures |
| Fabricated Content | Content that is 100% false, designed to deceive | High | Cross-reference verification, comprehensive fact-checking |
| False Connection | Headlines, visuals or captions that don't support content | Medium | Content-headline consistency checks |
| False Context | Genuine content shared with false contextual information | High | Temporal analysis, context verification |
| Manipulated Content | Genuine information or imagery manipulated to deceive | Critical | Digital forensics, content authentication |



| Category | Company/Organization | Services | Focus Areas | Australian Presence |
|----------|----------------------|----------|-------------|---------------------|
| International Players | Newsguard | News source credibility ratings | Source verification | Australian media coverage |
| | Storyful | Social media verification | Content authenticity | Sydney office |
| | Logically.ai | AI-human hybrid fact-checking | Comprehensive detection | Australian clients |
| Australian-Specific | RMIT FactLab | Academic fact-checking service | Political claims, COVID | Melbourne-based |
| | Crikey's Fact Check | Media-based verification | Political statements | Australian-owned |
| | AAP FactCheck | News agency verification service | Breaking news, political claims | National coverage |
| Technology Integration | Accenture | Custom misinformation solutions | Enterprise integration | Multiple AU offices |
| | Deloitte | Digital trust solutions | Organizational response | National presence |
| | PwC | Information integrity services | Risk management | Major cities |
| Social Media Monitoring | Brandwatch | Social listening with misinfo alerts | Trend identification | Australian operations |
| | Meltwater | Media monitoring | Reputation management | Sydney, Melbourne offices |
| | Sprinklr | Enterprise misinfo detection | Brand protection | Australian clients |
| Academic-Commercial | Various university partnerships | Research-based consulting | Specialized detection | Nationally distributed |

