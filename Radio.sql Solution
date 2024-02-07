---- Qusetion NO 1 ----

SELECT stationName,location FROM stations
WHERE location = 'East';

---- Qusetion No 2 ----
SELECT host.HostID, HostName , ShowName FROM host
JOIN Shows on host.HostID = Shows.HostID
WHERE HostName ='Vrajesh Hirjee';

---- Qusetion No 3 ----
SELECT Shows.ShowID, Shows.ShowName, COUNT(AwardID) AS Num_Award
FROM award
JOIN shows ON award.ShowID = shows.ShowID
GROUP BY Shows.ShowID, Shows.ShowName;

---- Qusetion No 4 ----

SELECT shows.ShowID,shows.ShowName,partnerships.PartnerName 
FROM Shows
JOIN Showpartnerships on Shows.ShowID=Showpartnerships.ShowID
JOIN partnerships on ShowPartnerships.PartnershipID = partnerships.PartnershipID
WHERE  partnerships.PartnerName = 'Spotify';

---- Qusetion No 5 ----

SELECT HostName,JoinDate FROM host
WHERE YEAR(JoinDate)<'2010';

---- Qusetion No 6 ----

SELECT ShowName,LaunchDate
FROM Shows
ORDER BY LaunchDate DESC;

---- Qusetion No 7 ----
SELECT HostName AS host,sum(ShowCount) AS Total_show FROM host
GROUP BY HostName
ORDER BY  Total_show DESC;

---- Qusetion No 8 ----
SELECT PlatformName,Link 
FROM Onlinepresence ;

---- Qusetion No 9 ----

SELECT stationName,LaunchDate,Location
FROM stations
where year(LaunchDate)>2010 AND Location = 'South';

---- Qusetion No 10 ----

SELECT HostName , ShowCount,
DENSE_RANK ( ) OVER ( ORDER BY ShowCount DESC ) AS Host_Rank 
FROM host;

