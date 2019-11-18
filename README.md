select * from films left join actors on (actors.film_id = films.id) left join producers on(producers.producer_id = actors.film_id) left join Genres on(Genres.genre_id = actors.film_id);
Здесь я соеденил все таблицы и столбцы включая связующие;
Далее в этом запросе, используя сокращения я вывел только интересующие нас столбцы с таблиц без лишних свзующих)
          →
          →
          →
select  q.name,  w. actor,  e.producer, r.Genre FROM films q left join actors w on w.film_id = q.id left join producers e on e.producer_id = q.id left join Genres r on r.genre_id = q.id;
