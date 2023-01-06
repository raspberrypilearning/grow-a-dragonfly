## Symudiad pryfyn ar hap

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Mae'r pryfed yn dy ap yn symud mewn patrwm cyson iawn, ond mewn bywyd go iawn maen nhw'n anodd eu dal. 

Byddi di'n defnyddio'r bloc `dewis ar hap`{:class="block3operators"} i wneud i'r pryfyn symud mewn ffordd fwy naturiol.
</div>
<div>
![Y Llwyfan yn dangos pryfed yn pwyntio i gyfeiriadau gwahanol.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Ychwanega sgript at **Insect 2** i wneud iddo bwyntio i gyfeiriad ar hap bob 1–3 eiliad.

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Profi:** Rheda dy brosiect a gwylia sut mae'r pry yn symud. Rho gynnig ar newid y rhifau i gael yr effaith rwyt ti ei heisiau.

Galli di hefyd lusgo'r sgript yma i'r corlun **Insect** fel ei fod hefyd yn symud ar hap.

--- /task ---

--- task ---

Newidia'r pryfed nes eu bod nhw'n ymddwyn yn y ffordd rwyt ti am iddyn nhw wneud.

Gallet ti newid nifer y camau maen nhw'n eu `symud`{:class="block3motion"} i'w gwneud yn gyflymach neu'n arafach.

Gallet ti hefyd newid cyflymder y gwas-y-neidr.

--- /task ---

--- task ---

Gallet ti hefyd newid y maint sydd ei angen ar y gwas-y-neidr i dyfu i gyrraedd ei lawn faint.

Gwna ragor o newidiadau nes dy fod ti'n hapus gyda dy brosiect.

--- /task ---

--- save ---
