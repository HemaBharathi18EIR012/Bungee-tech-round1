# Bungee-tech-round1
import pandas as pd
import numpy as np
euro12 = pd.read_csv('../input/Euro 2012 stats TEAM.csv')

euro12
euro12.Goals
euro12.shape[0]
euro12.shape[1]
discipline = euro12[['Team', 'Yellow Cards', 'Red Cards']]

discipline
discipline.sort_values(['Yellow Cards', 'Red Cards'], ascending = False)
round(euro12['Yellow Cards'].mean())
euro12[euro12.Goals>6]
euro12[euro12.Team.str.startswith('G')]
euro12.iloc[:, :7]
euro12.iloc[:, :-3]
euro12.loc[euro12.Team.isin(['Englad', 'Italy', 'Russia']), ['Shooting Accuracy']]
