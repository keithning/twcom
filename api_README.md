Taiwan Company's Network Rest API

1. Company network from company id

    Syntax:

        url/com?id=&maxlvl=

    Input:

        id: company id
        maxlvl: max levels

    Output:

        company network with node, edge informations

2. Boards network from company id

    Syntax:

        url/boss?id=&maxlvl=

    Input:

        id: company id
        maxlvl: max levels

    Output:

        Boss network with node, edge informations


3. Company network from boss name

    Sytax:

        url/com?boss=&target=

    Input:

        boss: boss name
        target: (Optional) boss target

    Output:

        company network with node, edge informations


4. Company network from boards of the same company

    Syntax:

        url/com?comboss=&maxlvl=

    Input:

        comboss: company id
        maxlvl: max levels

    Output:

        company network with node, edge informations

5. Company network from address of the company

    Syntax:

        url/com?comaddr=&maxlvl=

    Input:

        comaddr: company id
        maxlvl: max levels

    Output:

        company network with node, edge informations

6. Query boss with similar name (in SQL: "name like '%boss%'")

    Syntax:

        url/query?boss=

    Input:

        boss: boss name

    Output:

        dict of different group of bosses, {target: [companys]}

7. Query company name and id from company name (in SQL: "name like '%name%'")

    Syntax:

        url/query?com=

    Input:

        com: company name

    Output:

        dict of companys, {id: name}
