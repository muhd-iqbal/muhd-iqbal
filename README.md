```php
<?php

const NAME = 'Muhamad Iqbal';

$skills = [
    'PHP',
    'Laravel',
    'Tailwind CSS',
    'JavaScript',
    'MySQL',
];

function introduction(string $name, array $skills): string
{
    $skill = $skills[array_rand($skills)];
    return "Hi, I'm {$name}, a {$skill} developer. Nice to meet you 👋";
}

echo introduction(NAME, $skills);
