代发 wailian999

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/goqtxqdti.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fktsv.cn/Article/details/gvgsxpxbi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gmirpjfow.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gcnsfpvqh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gougiifhs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gyxtxhbpa.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/goczadfjt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/gejgedohz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gwedesdwb.sHtML

[B02] 多分支 else if / elif
来源：http://baike.sjlbkw.cn/Article/details/gxicogkiw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gfnmpsjie.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fktsv.cn/Article/details/gfweevnvq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrvpnjlu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gaqpuupyw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/glaybaktw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.tarul.cn/Article/details/gcdpftyqg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gzkfkpgql.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gcrzfrmvp.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gqfukuheu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgpmdtfq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gegdkhzin.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gexhykiwz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gmoreeckw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gihesjpjf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gtaiukycn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.epnwcf.com/Article/details/gqinalura.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.bbcook.cn/Article/details/geqwlgikb.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gdacremps.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.tarul.cn/Article/details/gtfbnpsoa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gocrogita.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gpwoczdep.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gmjkjrzan.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.yfazqb.com/Article/details/gneosglms.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/gknlufivj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/gixdxzphq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gqwoshhay.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.vehdjk.com/Article/details/ggzcsmwar.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/gvbvldxms.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gfcjwrhfd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gfnrxkelx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gfabrertl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fktsv.cn/Article/details/gccrfwbfq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fktsv.cn/Article/details/ggitcnyyo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.vehdjk.com/Article/details/gugirqgfr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gqdeiyiul.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gjsdyvcom.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/gwewpbtyt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.vehdjk.com/Article/details/gtcbvcrnw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/glhyesvvd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gcsxlnufu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/ggtgzagdm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.epnwcf.com/Article/details/girjtadit.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.epnwcf.com/Article/details/gssflxpmd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gnylpqorl.sHtML

[B07] while 循环
来源：http://read.share.sjlbkw.cn/Article/details/gknwxbijz.sHtML

Py:   while i < 10: i += 1
来源：http://3g.epnwcf.com/Article/details/grmkakpjx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.vehdjk.com/Article/details/gdatwsqrr.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gizpvlpwz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/goqzjqoaj.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gcuxhvilz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.yfazqb.com/Article/details/gelddbadp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.yfazqb.com/Article/details/glahyeybs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gqpboxbkg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/gsmyojedy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/ghsvyyhmu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/guqvzxrfb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gaqyfetci.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/ggethwhuw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gvllgjscw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/gydoqmecv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/gzadvrtmr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gjfvncirj.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/gqxovltrh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/gpeicqukj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gvxxulsom.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/groeztsbc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/grdrrttpu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gdwjbpmkr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.yfazqb.com/Article/details/glzsyvouz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.vehdjk.com/Article/details/grdfucnlk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gqtqdsbrd.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.yfazqb.com/Article/details/gbdrrunoo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gztgdywos.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.vehdjk.com/Article/details/gycbjebrz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/getdwgoum.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gywthbtna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/gtzukkjfe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gsduakbbt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/gwoomucba.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjovxyubh.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.yfazqb.com/Article/details/gnmkesqcu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/gzroppale.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gffgnikeo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gvgdwuqds.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gmnkxniav.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gljerkoyk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.vehdjk.com/Article/details/gddzztazg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/gqsmtmxxi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gpjaspkwf.sHtML

[B12] 跳出多层循环
来源：http://www.blog.tarul.cn/Article/details/gpovrwmmh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/ggbvryyzf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gnpsmluou.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gjsimmhow.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gzbmodtct.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gpzmynhbk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gfdndrtou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.tarul.cn/Article/details/gzmmwutfw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/ghwhgzfow.sHtML

[B13] 判断是否为数字
来源：http://www.blog.epnwcf.com/Article/details/gkbxhtueo.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gcpbwleeg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gbkvkyjah.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gaftexgco.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gdnvmeuej.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/gffzoarry.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.epnwcf.com/Article/details/gkbfxqkfk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.yfazqb.com/Article/details/gavcgoqgh.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/gblirwckt.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gprcsdedb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/gpjtiwoeb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.tarul.cn/Article/details/gfeapkcmz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/gcpscfnre.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gblbewlnn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/gewvmvztr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.epnwcf.com/Article/details/ggqraoojb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.bbcook.cn/Article/details/gyycqkony.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtsdkvib.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fktsv.cn/Article/details/grnxvvkkw.sHtML

Py:   a and b or not c
来源：http://www.blog.yfazqb.com/Article/details/gqnusudnj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/ggjccicup.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gmqiflfaa.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gkplmvula.sHtML

Java: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gnaqcaxaa.sHtML

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/guqavzqmr.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gbvqsrznw.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gruzsqsez.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gyfxtwapn.sHtML

Py:   if not data: return
来源：http://www.share.vehdjk.com/Article/details/gvyxfrkhr.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gaiuvmkle.sHtML

JS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gkmmxeewn.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gxwzgnazo.sHtML

Java: if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gzwzdqquq.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gkuaialrg.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gpbpgcekk.sHtML

C#:   if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gtozckutl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gspwknzid.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gyveelyyr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpdmcjdgp.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gounhcgll.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gohwvrild.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/guggpglbq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gffjbffgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gtlzslhol.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gfhnceiha.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fktsv.cn/Article/details/gmyglkhiu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gsukeuskf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/goopayleh.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/gawigtnle.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gppqztwif.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gnezvjxeb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gcnbinvfq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gflnzrxjw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/grcchanff.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/guyxdzehe.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gqzzguydh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.vehdjk.com/Article/details/glwmhzoax.sHtML

[C03] 可变参数
来源：http://mobile.epnwcf.com/Article/details/gvpiwjffk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/gwvsfretp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gcetdsrtk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gixhhqixx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/ggpvmmavd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fktsv.cn/Article/details/gldlhamdk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.yfazqb.com/Article/details/gvczivpny.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/ghddzhvfj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.bbcook.cn/Article/details/gkloorvuv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/gskfgxgxz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gswthliet.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gcvafxtze.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/grrfcmtxg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gfwnlokot.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gnykfobfn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/gwjzmvmok.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gxtzhigmv.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gbmqpmpdh.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gltfxhnou.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/geslngiip.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/ggnbwdstm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gdsaxqpwy.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gufxhnboy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.vehdjk.com/Article/details/gkhobmaxs.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gcwtxoxbd.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gciuujknr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gioxsglnj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/gagcuncyw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/gooimqryb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gwnzamvov.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gyretnqro.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/ginbfcevz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.sjlbkw.cn/Article/details/ghcupzkda.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gqtkvihie.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/gzfkeqxwz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gdltnlftn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gqikuiusc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gbuqcmosh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/gigvmkeco.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.bbcook.cn/Article/details/geglgidfj.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/gtpwmzxaf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gsscblgpo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fktsv.cn/Article/details/gmaqxckha.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gaothismv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.epnwcf.com/Article/details/ggmptdscy.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gjacwthvk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.bbcook.cn/Article/details/gzendsfkn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/gkqsjjloz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/geifllxyp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gqumrrteu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/gopqwjuzr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/gvzaursry.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.bbcook.cn/Article/details/gmkrhmpya.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaoqlfxoe.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gulnlsyhu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gntlzgupi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gazffcnvd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gafpcaabk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gqabwlhzo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.epnwcf.com/Article/details/giuiwpanu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/grniegxvh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gwelandfu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gwiwcywai.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gjcmnjtnr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fktsv.cn/Article/details/gulzvkgyq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.tarul.cn/Article/details/gwjallxvu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/ghtzlphfr.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gwmfidfzv.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gfudyndsw.sHtML

Go:   花括号块级作用域
来源：http://www.blog.epnwcf.com/Article/details/ggxqppdbx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fktsv.cn/Article/details/gxzoxsnnr.sHtML

C#:   块级作用域
来源：http://blog.fktsv.cn/Article/details/gvurengzm.sHtML

[C11] 模块导入与导出
来源：http://blog.tarul.cn/Article/details/gziifdmmr.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gadkpeggh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gsnewtnfs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gbhwvcbpr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/glcseqmnt.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gclntqafh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/ghxejiyqp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/gvttntkxp.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gqhwelexw.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/gydfoutdh.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gtiepozqk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/glpojzzey.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gsplcjriw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/ghdryatmj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gypekhndv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.bbcook.cn/Article/details/googvpcvj.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/guqqdzzim.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.sjlbkw.cn/Article/details/gzpokanth.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/gssqzbabj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gcjownaac.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gergczuju.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/grgqqjyrk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/goonqcefs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gbtujfhnr.sHtML

Go:   func add(a, b int) int
来源：http://baike.fktsv.cn/Article/details/gxrrjkgvz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/gkgndvtcn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtqmxesv.sHtML

[C14] 泛型函数
来源：http://www.m.share.fktsv.cn/Article/details/gdjapxfzx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/gidnszmaj.sHtML

PHP:  // 无泛型
来源：http://baike.bbcook.cn/Article/details/gclagfwlf.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/gdkhmyfai.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/ghfzgwwzv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gqilxnutr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/ghzuvvokg.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/gpwyyxbys.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fktsv.cn/Article/details/gndgvvxlg.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/gwmddytgd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gghimnnmq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.bbcook.cn/Article/details/gzbvzdefp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gjxaomkep.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gwvgkzjnd.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gmaoywnbk.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/gpxrxcoux.sHtML

Ruby: a, b = pair
来源：http://www.m.share.bbcook.cn/Article/details/gkrvyywvw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.yfazqb.com/Article/details/gwxxpjtsu.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gcfumznqj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/grtoyrgbs.sHtML

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/gziuscdtc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gxfpxiaas.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gqhcspsnv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/gpuansoku.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/goeavdykr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gkqsjszxh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.vehdjk.com/Article/details/gsoyblqkr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcmqqznhf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.bbcook.cn/Article/details/gxuyblicz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwdxxegxc.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gnssifuzp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/gnvckvwct.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.tarul.cn/Article/details/gpunnyofx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gruafzlbc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gpfqzjedr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/gpzfndvcy.sHtML


<!-- 参考信息 -->