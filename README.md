# Nevi's Edited Diffsinger Colab
My version of the diffsinger training google colab made by Usamireko (originally made by Ghin_MLo7)


Full honesty some of the changes i made were altered by Claude. I'm not a good coder so half of the time i make a change it breaks or doesn't work periodt so at a few points i have used Claude to fix my shitty code.

I'm sorry if thats upsetting :(

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NeviNevethos/NevisDiffsingerColab/blob/main/DiffSinger_colab_notebook_Nevi.ipynb)


# What's the difference between this colab and others?
- Mix-LN (new) in branch selector (this is the one with blacklist and SDP).
- Edit Config cell automatically only picks 1 test_prefix per dataset entry instead of 3.
- Automatic speaker_id configuration.
- Being able to change smooth widths for embeds in Edit Config cell.
- GAME implementation instead of SOME.
- Batch CSV cleaner (to remove segments that are only rests when using GAME or SOME generated .ds files)

If you run into any crashes that you think are exclusive, please open an issue on github or send me a message on my discord!
(Username: Nevethos)
