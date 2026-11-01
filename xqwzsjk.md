代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gzdteepyj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gcgegkalw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.bbcook.cn/Article/details/gfeooglft.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.vehdjk.com/Article/details/gthjtgfhx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gyqrzaccr.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gqeaqyiqf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.epnwcf.com/Article/details/gfktfvbpb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.yfazqb.com/Article/details/gkdgrjkfc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gqrotavcf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/grjnkmwas.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gbmxbntem.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/giigiygun.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.yfazqb.com/Article/details/gwvbjkaez.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/glfdmaenm.sHtML

[B03] switch / match / case
来源：http://www.share.fktsv.cn/Article/details/gxkijhkxy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gbvrceatw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpewrnuxu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gaovvnvvj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvhbmlqbj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gnskzvcxt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gvlmckxbl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gdftujius.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gkgnnqmwq.sHtML

[B04] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gbbuzstcn.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gajyviagv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.bbcook.cn/Article/details/gfilxdfaz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/ggyyfviro.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gdzrlgksh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.yfazqb.com/Article/details/gaxycxpol.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fktsv.cn/Article/details/gvinjvvfw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gchjrphaq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/gifbmibyy.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gsshmvfpv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/gcronvcbm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.sjlbkw.cn/Article/details/gybscqeom.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gmyvgaybp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/ggcsbanth.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gvlzsfvyz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/gseyqqloh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fktsv.cn/Article/details/gzauecpjv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fktsv.cn/Article/details/gnyepzlue.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.sjlbkw.cn/Article/details/gonxfmsuf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gjocmsgct.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.epnwcf.com/Article/details/gwalypina.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.vehdjk.com/Article/details/gspvgvfum.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gkywwyktg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fktsv.cn/Article/details/gxdywolmo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.sjlbkw.cn/Article/details/gnydvuxpu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gynxgfzkr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/gbprqztae.sHtML

[B07] while 循环
来源：http://3g.yfazqb.com/Article/details/gqeylkxrs.sHtML

Py:   while i < 10: i += 1
来源：http://wap.sjlbkw.cn/Article/details/gipztfbfu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.vehdjk.com/Article/details/gehngnvfj.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gvopevsmf.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/ghdqhzlvj.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gxgrhjklu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/grazervev.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.sjlbkw.cn/Article/details/gzpskgdig.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gfmgkzixr.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fktsv.cn/Article/details/gxxfxkqoc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fktsv.cn/Article/details/ghpstcqpz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gkfabirxp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gimnucdmn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gwnsnqyku.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/ghwsfvzxp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gjbgkvudq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gkrfimdve.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/ggzqprcqf.sHtML

[B09] break 与 continue
来源：http://baike.sjlbkw.cn/Article/details/gurdtspum.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.vehdjk.com/Article/details/gdgswspqq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gkkdddccj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gvzqlftom.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/glfritryr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gszunzfbp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gqgxxzuqu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.tarul.cn/Article/details/gbjuvgdyk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gereonmxf.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.sjlbkw.cn/Article/details/gsdxdgwxx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gtyohjefv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/gxdunysqs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gtgcynknz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gydtbwjjb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gmrxmpwhi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gksgpoyhb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.epnwcf.com/Article/details/gquseooen.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/gdoldqoit.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gxuiqysia.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gvftjgiul.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.bbcook.cn/Article/details/guinxmgye.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gifmecnxm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/ghtojrpwb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gkdhybihi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gdsjalgbo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/guzktmvqb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gushbvnmj.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/gnotfktcs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.vehdjk.com/Article/details/ggaqwkjyl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gkewpdgrx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gupuvpeec.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/ggobivrip.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gcnrcsnrc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.tarul.cn/Article/details/grnkmyylb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gxfekbust.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/gnyjdnfrt.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/glicczwep.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/ghjudocqx.sHtML

PHP:  is_numeric($x)
来源：http://wap.sjlbkw.cn/Article/details/gzjwwqhdv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gganksjjq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gqfqjkgns.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gopybspvh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.vehdjk.com/Article/details/gtdsqsilg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/gawfzrndf.sHtML

C#:   x is int or double or decimal
来源：http://wap.fktsv.cn/Article/details/gioprtjgy.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gbvjfxhls.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gnpvlujxm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.vehdjk.com/Article/details/gwmjmmmvk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gldrcattv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gykorwzro.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gjogxqxuy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/gstywtskp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gnphpemei.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gexanxcon.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gigjipyad.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gzrrawqyw.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gmsstgbfm.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gwhhikmyt.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gqiiygppc.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gqtbyixdf.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gahewhneh.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gtguribcc.sHtML

C#:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/geksvgbrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/grxunftuz.sHtML

Py:   if not data: return
来源：http://baike.fktsv.cn/Article/details/gvtofaklw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/glsrszmdf.sHtML

JS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gbwkddkca.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/glphuonbu.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gjyojuufq.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gekyloypd.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gzcitcbst.sHtML

C#:   if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gistxvcfl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gomkmrivg.sHtML

C. 函数与作用域
来源：http://www.m.share.tarul.cn/Article/details/gxwxedgdw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggtwhbhwo.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gjgabxpvc.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gtvrbjtwu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gaqxqojcg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gwwrcchvo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gvllbuqpq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gksjfganz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/grglsjdar.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gyvldvbtu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/goiawhehk.sHtML

[C02] 默认参数
来源：http://wap.yfazqb.com/Article/details/gorivpqtt.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gymclepsm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.bbcook.cn/Article/details/gsplkvgnf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gtetknbta.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gurhnmgje.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/gaiicjwnr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gdxrcsjbs.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/gvvvetbrs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.vehdjk.com/Article/details/gyrqzenyp.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gdvxyrqds.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gfnmyatxd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gsmyhllxt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/geqoaqadd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gkyzhbiyx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/grtgoypok.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/gnsznlncb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gwrteaoyr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/giehgwces.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gloubcefo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/gihtmkyaj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/ggrhjgkhp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/guouocszw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.epnwcf.com/Article/details/gireirane.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/grmhoevfz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/geveuszsz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gophkiwvs.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/ghwgletkl.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gswkciavz.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gczjdjqwo.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gkecrfmgy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gwgbtnada.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gnybnbfxn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gwrkygcii.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gpmslqyha.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gyclcnxfq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gnqtculjb.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/gkglcfoom.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/gmmofbiiu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gabadqajm.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gaznihwbx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/gzuufucrm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gqukargob.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gyrclngmx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gzndyjuhf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gyliaetjl.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gcprpkvmb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gofujrwme.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/geziglwwo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.yfazqb.com/Article/details/gwzlfoxrq.sHtML

TS:   arr.map(String)
来源：http://www.blog.fktsv.cn/Article/details/girhbttyh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/glzcrdmei.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.epnwcf.com/Article/details/gyzuotesg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.sjlbkw.cn/Article/details/gvuwzpzhe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/gjvuzivvb.sHtML

[C08] 闭包
来源：http://mobile.bbcook.cn/Article/details/gmqtjgixu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gdnloeeup.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/ghzgtdwve.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gbaedxmvm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gmupajvjs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gwrwkrsyx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/glvrsxhkh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.tarul.cn/Article/details/gpopmpfto.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gedvvlhie.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/guucuzaha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gfukgjxpi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/goxbfclng.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/ggzohgvcm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gwabqkjhw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/geazjeexa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.sjlbkw.cn/Article/details/ggkxajaxe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/glmfwsxur.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gtcpnpehj.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/gbaxftteb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gfsenoojk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/gsbfewtmj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gxvgbafri.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gnvfmcvhn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/gkgwymxtx.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/gmgufdpyf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/grbxfpkyn.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gtawbnudl.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gjecvasqs.sHtML

Py:   from module import func
来源：http://3g.bbcook.cn/Article/details/gsinshfoy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gyvncttsc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gklwtonug.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gqtrccknx.sHtML

Java: import java.util.List;
来源：http://3g.bbcook.cn/Article/details/gfqimztsh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/gpppmrdhc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gnszbmtnb.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/ggabhhxut.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/guraeuweu.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/ghtncfjad.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gtjkyzlmu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gsoscnpkt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gctaduyhm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gxzceztuy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fktsv.cn/Article/details/glsrvwxxo.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fktsv.cn/Article/details/gihtcfcwq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/grkioaivm.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gayydadef.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/glmluwvhn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/ghnfxycgn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.tarul.cn/Article/details/gbbhrggwm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gaygvrjuc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gtekgsbuf.sHtML

Go:   func add(a, b int) int
来源：http://wap.bbcook.cn/Article/details/gofgnupcs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gnohrkumr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/giqxlxyjx.sHtML

[C14] 泛型函数
来源：http://www.blog.bbcook.cn/Article/details/gwfzjexnr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gpzafbfit.sHtML

PHP:  // 无泛型
来源：http://wap.bbcook.cn/Article/details/gsvjrgidh.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gjhuwjtho.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/guofosxtl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/ghseosfcg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gqoqkoucl.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/grutaiael.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gwuzpewdf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/gclwovkca.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gpypyszjg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fktsv.cn/Article/details/gxkmpmffb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/glymflcjj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.yfazqb.com/Article/details/ghhctsoxe.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gnskbefge.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gsapitfyv.sHtML

Ruby: a, b = pair
来源：http://blog.bbcook.cn/Article/details/gkgukbxwc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gpgbhgxen.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gvjtqdnpp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fktsv.cn/Article/details/grludsweu.sHtML

PHP:  // 无重载
来源：http://read.share.tarul.cn/Article/details/gtsctvsof.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.bbcook.cn/Article/details/glswwdzzn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gdjtucqvk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/glgpmhpak.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.bbcook.cn/Article/details/grkevmkix.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/gkknaynhh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/gulddafra.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gidgxdwde.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gjmivudap.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpldfwrfw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gbglppywx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fktsv.cn/Article/details/gpejlqqlq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gbyviwird.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/gmioxbqns.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/gnihjunrw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gpteylwax.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gioasrilk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.yfazqb.com/Article/details/gozjntxdi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/ggopccjxj.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/gyhwxpjkk.sHtML


<!-- 参考信息 -->