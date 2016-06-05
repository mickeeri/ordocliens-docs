# Arkitektur 

### Struktur
Applikationen är konstruerad med Ruby on Rails, men istället för vyer skapde med Embedded Ruby består vyerna av [.jsx-filer](https://facebook.github.io/react/docs/jsx-in-depth.html) som används tillsammans med JavaScript-ramverket React. 

Det åstadkoms med ruby-gemet [react-rails](https://github.com/reactjs/react-rails) som erbjuder utvecklare att använda React integrerat med Rails Asset Pipeline. Det jag gör att är att i min controller rendera React-komponenter istället för vyer enligt [följande beskrivning](https://github.com/reactjs/react-rails#rendering-components-instead-of-views). Det tillåter så kallad [Isomorphic JavaScript](https://medium.com/technically-speaking/isomorphic-reactjs-app-with-ruby-on-rails-part-1-server-side-rendering-8438bbb1ea1c#.k0xpa82lf). Vyerna (eller komponenterna) renderas alltså på serversidan första gången. De uppdateras sedan genom jQuery's ajax-metoder, ungefär som ett vanligt API. 

### Databas 
![Databasmodell](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/img/Lawfirm%20database%20(1).png)

