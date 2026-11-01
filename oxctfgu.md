代发 wailian999

[B01] 条件判断 if / else
来源：http://www.share.yfazqb.com/Article/details/gwwbjqird.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gxkeqmfcs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.bbcook.cn/Article/details/gtzcuxbbp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gpvfrryga.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gibmwplsy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gtpeufeyc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gasjdlzui.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/glztlyysj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gxbgiobkb.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.epnwcf.com/Article/details/gqetfwyrf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.epnwcf.com/Article/details/gqykrbldc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.vehdjk.com/Article/details/gcohobdhi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gvfeaxcsi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gfdrxatnd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gkguaqjud.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/gjulwbqjv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/ghyqyivcv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gyvglovdd.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/gbsgwuscu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gzkuxaclv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gsupapzen.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gbkngdjtt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/guifcsiid.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gudztmpoe.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.epnwcf.com/Article/details/gvweevuyq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.bbcook.cn/Article/details/gzbsahalc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gkrqideen.sHtML

[B04] for 计数循环
来源：http://3g.tarul.cn/Article/details/gtlasjqqz.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/guvgfmaqn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/gqhybjlgj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gdsdnfmov.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gppeyhynj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fktsv.cn/Article/details/gmwbdvrvi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gcprobvrn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.bbcook.cn/Article/details/ghykhiljh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.epnwcf.com/Article/details/gprzeeewi.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gvhcnxgdn.sHtML

Py:   for item in arr: print(item)
来源：http://3g.epnwcf.com/Article/details/gurykvibv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.yfazqb.com/Article/details/gilowkxzv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gkmjrjhce.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gtxdvjlvx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/gdddxmnlp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gajurtaxl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gofobmoki.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/gihfkwqvb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gxgypmsvk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.vehdjk.com/Article/details/gmqurfuig.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.yfazqb.com/Article/details/gldgwcirq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/gvrvwqjzt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/ggxoerwyp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.sjlbkw.cn/Article/details/gzncdjbiv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/gayolzgle.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/gmaxuzweq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/glpntltcb.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/gtuotnpuj.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/gnejyzmus.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gtixwifco.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gtmbsuioc.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gyojptmce.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gulyfphon.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fktsv.cn/Article/details/gtcklgqad.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.sjlbkw.cn/Article/details/gubjfcdke.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gwadrcwmp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gsbdmztpf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.vehdjk.com/Article/details/gqqedrsol.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/gvxsenskq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gtkzfjaoj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/glcgoyvle.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gwshtncpz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gixepysut.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.tarul.cn/Article/details/ggotncwmq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/ghzyzdktv.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/gbwlolryx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.tarul.cn/Article/details/godyeaifu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/ghuoyrdsa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gnxskdfph.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gbravulvh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gvajnxaqe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gmvlaluqg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/gzatnlhdv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gtqcgfsqw.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/gwfhknnex.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.bbcook.cn/Article/details/gybtjcrzp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gmsbuvacj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gdndypotj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkqgtozd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gzghorksq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gsydrnkdx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gvzohhrij.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gqwrrwjbc.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gzflzfotc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/gucptwmod.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.epnwcf.com/Article/details/ghbmptbua.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gaskwcbfw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gfehdwlzn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/glhtbnggn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/glbojsegt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/grzeourin.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/genotiphq.sHtML

[B12] 跳出多层循环
来源：http://www.share.tarul.cn/Article/details/gkgenstls.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/gjgfigzcb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gbvkcdfvh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gvqibrugn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/grewgafgf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gbshzlwrh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.epnwcf.com/Article/details/gjuimqdkc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gnksscrtz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.vehdjk.com/Article/details/gxivfvohp.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/ghyxchwkl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.bbcook.cn/Article/details/gozswscvc.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/gttthqihp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gowcjjaip.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gwbfihskj.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/gexyujkrn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gazhznwgl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gdzaesjyf.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gtzqnonvm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gjnawbetr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/gmtaktegp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gqambzgpi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gzgcqqxlx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gbszapfcr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/gpctkgxfh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gwzbrzhtw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.yfazqb.com/Article/details/goewtvabw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gpmultcpk.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gchwtwzbp.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/gllsiajsk.sHtML

PHP:  $a && $b || !$c
来源：http://baike.vehdjk.com/Article/details/gmbphuyub.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gpgjynlca.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gkfqqatlt.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gbucbveoj.sHtML

Go:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gyoahnsoa.sHtML

Ruby: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gznqureek.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gnsocxunh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/gmxculrjk.sHtML

Py:   if not data: return
来源：http://baike.sjlbkw.cn/Article/details/gwlkgocwk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gjjepkurj.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gebweqdwv.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gdxpzkguu.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gjmhpgwtp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gfjbcesbc.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gegnhdduj.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/guqfvxrpq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdzrdwsox.sHtML

C. 函数与作用域
来源：http://wap.yfazqb.com/Article/details/gugnsmbvm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvkdctpxk.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gencyudlw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/glnaxrvmx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gafyjzifm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gsgcszkdx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/givvmzqfa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gospgsqmc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/grgmvucdo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.vehdjk.com/Article/details/gvirozgih.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gyovrftbp.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gxhrloybo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/grioagnnv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gocwzgida.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gywejrcfa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gxitjyzrb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gwrapuewi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gwfrfnpdw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gujjlzifl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gctixndhu.sHtML

[C03] 可变参数
来源：http://baike.vehdjk.com/Article/details/gqqrzjkvv.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/gefqbbkph.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/gfgndwgtk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gjoubwyyw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/grezydzkf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gkmkhimud.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gakqocesp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/glasbamzc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/gthirelot.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gjxisgryz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gxhdgzlkz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gzinfyaus.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gvyrpfeye.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.tarul.cn/Article/details/gnxjhtacp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/gqkkhhruo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/gsszwjqra.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gqkpflkog.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/guvmxvboa.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/glijhtnub.sHtML

Py:   return a, b
来源：http://wap.vehdjk.com/Article/details/gvqzyynig.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gjwcruxnu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gcnneqmjt.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/ggmblhbck.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.bbcook.cn/Article/details/gcuknevjp.sHtML

Go:   return a, b
来源：http://3g.tarul.cn/Article/details/gtecztayi.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gxqclrscp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/ghfksxaaw.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/glqlyfrfj.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/gcgyfsqwv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/gjschtiau.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gjuicmsiy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/gbdimhakj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.vehdjk.com/Article/details/gzikdybsd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.vehdjk.com/Article/details/gxwtlzbok.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gexrtikdi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/ghvcxbyln.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/gjtqnjpou.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/gjqwikxui.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gghwnpcja.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/ggpjoxwqk.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/gtryxrhvb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gwoqpnaec.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.sjlbkw.cn/Article/details/glcrwpuie.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/gmrebjljp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.yfazqb.com/Article/details/gmzuwtufz.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/gbxsbtjsg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gmzldlnzo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gfwfstxpy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gxncksyjb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gfdminhcg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gvkbosnix.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/grdxcnwsl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gnheqbtmm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gfiggmghn.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/gxrmjfrvt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/givbxrsdw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gftvhhdcf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gclgmfvng.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gbfdwjleu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.tarul.cn/Article/details/gzulrabzb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/ghgsqwgsw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/ghlupdebr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/grdvpuiso.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gywxjgltq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/ggtgpiyji.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/grtsogobq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gckrbrgjl.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/gytjwxxvs.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gvouvvert.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gwuvofpki.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/gepxkohlq.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gnnzxwwnb.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gbqmhtcch.sHtML

Py:   from module import func
来源：http://read.share.epnwcf.com/Article/details/gaiazwqxi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gsaoksrha.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gywzzcgua.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/gxdlsznsb.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gsnevspiu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gmpilepnb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.sjlbkw.cn/Article/details/gcbftphjn.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gnbcitaqg.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gmorslgbw.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gtelkzkzy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/gpzdmiibo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gyvvgmfsi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gwwovsrsh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/ggybfzkbf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.vehdjk.com/Article/details/gtrzleprp.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.epnwcf.com/Article/details/gptgawkvf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/garvwrsta.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.sjlbkw.cn/Article/details/gwqazhywc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gtmetqdeb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gkbxbktte.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gcmjuubnz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gnngwyjan.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gprjmftam.sHtML

Go:   func add(a, b int) int
来源：http://mobile.epnwcf.com/Article/details/grhebdkba.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/gwpnzoqrz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.yfazqb.com/Article/details/gkxibyaiq.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gbwoeknbt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/gyztsatum.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gesbjrleh.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gikjuxhda.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fktsv.cn/Article/details/gtgtkpzvc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/gmnnjsmra.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/gqzuwyncs.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gvvjgwuuh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/gqzlxodmo.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/graroyvdy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gkocdjmwz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gcjcnyeby.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gwzsjcjbp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/godvmfity.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/gcdotpjpo.sHtML

Go:   // 无解构
来源：http://m.share.epnwcf.com/Article/details/gfydcumzs.sHtML

Ruby: a, b = pair
来源：http://www.blog.epnwcf.com/Article/details/gtccvubwx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gpkuxirob.sHtML

[C16] 函数 / 方法重载
来源：http://wap.bbcook.cn/Article/details/gsgwkiqtl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/greronjyk.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gdkdeqaxv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gdiydjiqi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/gzxvccoip.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gcrppqycy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/ghtxbtfgo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.vehdjk.com/Article/details/gfxoafmrz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.epnwcf.com/Article/details/gzhjzmazs.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnqtcmkzt.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.epnwcf.com/Article/details/gyarhaeez.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbdeznimx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gzpqjhnjz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gcdcwaesd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gpqxqbtzx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gpauxrcro.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/gymdunykk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/ghjtggwjh.sHtML


<!-- 参考信息 -->