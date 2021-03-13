# Cosmos
Welcome All Amateur Astronomers!!

This data base is a simple, easy to use resource for individuals looking to get started looking at the Cosmos.
It contains 2 comprehensive data tables: one containing information about exoplanets, and the other containing information about stars with comfirmed.
The data should be uploaded to an SQL server, and here is some information about the tables:


exoplanets (

	planet_name varchar, (the planets name)
	planet_status varchar, (whether it has been confirmed)
	mass decimal, (mass in Jovian units)
	orbital_period decimal (in days),
	semi_major_axis decimal (in AU),
	eccentricity decimal (a dimensionless parameter that determines the amount by which its orbit around another body deviates from a perfect circle),
	discovered decimal (year),
	detection_type varchar,
	star_name varchar,
	PRIMARY KEY (planet_name)
);

host_stars (

	star_name varchar NOT NULL (the stars name),
	radial_ascension varchar NOT NULL,
	declination varchar (can us declination and radial_ascension to find the exact spot the star is in the sky),
	class varchar (the type of star),
	PRIMARY KEY (star_name)
);

You can use these data sets to create queries that can gather data about each exoplanet and its star, and we can do some simple calculations and analysis on the data as well.
