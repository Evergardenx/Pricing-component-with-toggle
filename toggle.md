# HTML And CSS For The Toggle

## HTML

<div class="toggle">
  <label class="name">Annually</label>
  <input type="checkbox" class="checkbox" id="checkbox" />

  <label for="checkbox" class="label">
    <div class="ball"></div>
  </label>

<label class="name">Monthly</label>

</div>

## CSS

.toggle {
display: flex;
align-items: center;
justify-content: center;
margin: 0;
}

.checkbox {
display: none;
}

.label {
position: relative;
background: linear-gradient(120deg, hsl(236, 72%, 79%), hsl(237, 63%, 64%));
display: flex;
align-items: center;
justify-content: space-between;
border-radius: 50px;
padding: 5px;
margin: 0 20px;
width: 50px;
height: 26px;
cursor: pointer;
}

.name {
font-size: 14px;
color: hsl(234, 14%, 74%);
}

.ball {
background: #fff;
position: absolute;
top: 2px;
left: 2px;
border-radius: 50%;
width: 22px;
height: 22px;
transition: transform 0.15s linear;
}

.checkbox:checked + .label .ball {
transform: translateX(24px);
}
