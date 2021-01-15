# vitae
Resume manager with experience tracking and resume generation

```rust
use ?::Email
use ?::WebAdress
use ?::PhoneNumber

struct Person {
    personal_info: PersonalInfo,
    contact_info: ContactInfo,
    skills: Vec<Skill>,
    experience: Vec<Experience>,
    hobbies: Vec<Hobby>
}

struct PersonalInfo {
    first_name: String,
    last_name: String,
    nickname: String,
    pronounce: String
}

struct ContactInfo {
    mobile_phone: Option<PhoneNumber>,
    home_phone: Option<PhoneNumber>,
    primary_email: Email,
    secondary_email: Option<Email>,
    web: Option<WebAdress,
    vcs: Option<VerCtrlSys>
}

struct PhoneNumber {
    type: String,
    number: ?
}

struct VerCtrlSys {
    platform: String,
    address: WebAdress
}

struct Skill {
    
}

enum SkillType {
    TechSkill,
    OtherSkill(String)
}

```
