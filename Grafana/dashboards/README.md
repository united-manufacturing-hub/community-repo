## OEE and status overview of all machines in the factory

This template is designed to keep an overview of the productivity of all the machines on the shop floor. For the template, we have 5 machines we are overviewing - Warping, Weaving, Thermosetting, Printing and Cutting. For each machine it shows the OEE via a gauge, the current status and a timeline of the status of the last couple of hours. 

When using this template, make sure to adjust the topics to reflect your machines. You can also copypaste the panel for one machine to add new machines to the dashboard. 

You can download the template json [here](./factoryOverviewTemplate-grafana.json) and import it into grafana.

## Basic machine OEE dashboard

This is an OEE dashboard for a basic machine, you can derive from it to customize it to your personal shopfloor but it has many good starting points. If you want to know more about how to build your own dashboard, please watch the video below. 

{{< youtube id="n3roOntfsgI" >}}

As you can also see in the video, this dashboard has panels, which show the current machine state, the OEE, the order table, timeline of states, shifts and breaks and breakdowns of stop duration and frequencies. Everything is broken down into a single dashboard and displays the information needed very clearly. 

![Untitled](/images/knowledge-base/grafana-repo/Untitled.png)

If you don’t want to build the dahsboard yourself with the youtube video, you can download the template json [here](./oeeytvidTemplate-grafana.json) and import it into Grafana.

## Warping machine rundown

This template is designed to show all information pertaining to a singular machine: the current machine status, OEE, timeline, breaks/shifts, duration and frequencies of stops, production amount, speed, and singular tension sensor displays. The template specifically is tailored towards a warping machine for weaving preparations.

For customizations, make sure to adjust the topics ot reflect your machine. You might also replace the yarn tension sensors and the producted length panels with something more fitting to your machine.

You can download the template json [here](./factoryWeavingTemplate-grafana.json) and import it into Grafana. 

## Weaving machine rundown

This template is somewhat similar to the warping machine rundown, just without the additional sensor readouts at the bottom. Like the warping machine rundown it features the current machine statue, OEE, timeline, breaks/shifts, stop durations, stop frequency, performance, count. In addition it can also show which product categories have been produced.  

To customize this dashboard, make sure to adjust the topics to reflect your machine data.

You can download the template json [here](./factoryWeaving2Template-grafana.json) and import it into Grafana. 

## Thermosetting machine rundown

This template also shows most of the uptime indicators that the other machines are showing. In addition to readouts of machine status, OEE, timeline, breaks/shifts, stop duration and stop frequency, it also shows temperatures of the different cylinders as a gauge. 

To customize this dashboard, make sure to adjust the topics to reflect your machine data. 

You can download the template json [here](./factoryThermosettingTemplate-grafana.json) and import it into Grafana.  

## Printing machine rundown

This template shows as usual: machine status, OEE, timeline, break/shifts, stop durations and stop frequencies. In addition it shows production speed, the length of printed band, the amount of straps produced and the temperature at which it is currently printing. 

To customize this dashboard, you should adjust the topic structures to represent your machine. Also you might want to recontextualize the panels “produced straps” and “produced length” if they are non-applicable to your machine. 

You can download the template json [here](./factoryPrintingTemplate-grafana.json) and import it in into Grafana. 

## Cutting machine rundown

This template shows the machine status, OEE, order table, stops, state timeline, breaks/shifts as well as the performance and the Product types produced.

As with the other dashboards, you should adjust the topic structures to represent your machine. 

You can download the template json [here](./factoryCuttingTemplate-grafana.json) and import it into Grafana.
