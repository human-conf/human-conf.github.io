---
title: "Iterations"
permalink: /iterations
layout: splash
excerpt: "Past, Present, and Future HUMANs"
---

<script src="https://momentjs.com/downloads/moment-with-locales.js"></script>
<script src="https://momentjs.com/downloads/moment-timezone-with-data-10-year-range.js"></script>

<script type="text/javascript">
let my_zone = moment.tz.guess(true);

function my(date) {
    let conf_date = moment.tz(date, "CET");
    let my_date = moment(conf_date).tz(my_zone);
    
    return ''
        + `<td>${my_date.fromNow()}</td>`
        + `<td>${conf_date.format("LL")}</td>` 
        + `<td>${my_date.format("LL")}</td>`;
}
</script>

# List of Previous and Future Iterations

<table>
    <thead>
        <tr>
            <th>Relative Time</th>
            <th>CET</th>
            <th>Your Time Zone</th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <script>
                document.write(my("2022-03-18 15:00"));
            </script>
            <td>
                <a href="https://human-conf.github.io/human22/">1st HUMAN workshop,</a> co-located with SANER 2022
            </td>
        </tr>
        <tr class="highlighted">
            <td>TBA</td>
            <td>2023</td>
            <td>2023</td>
            <td>
                <strong>2st HUMAN workshop</strong>
            </td>
        </tr>
    </tbody>
</table>