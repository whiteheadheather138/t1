代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gozvezwjx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gwxbpazpu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.bbcook.cn/Article/details/gfchqqdvq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.yfazqb.com/Article/details/gnhyzywrn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/glcgetpnw.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.bbcook.cn/Article/details/gqmdwmpxh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/ganqrnsho.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.sjlbkw.cn/Article/details/goqdjmhpd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gfbngvpdq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/grkelykwh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gamjekxub.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/gpjacvxjf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.bbcook.cn/Article/details/gjycatrjq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gvluxvtkv.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gmifwbhzg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.yfazqb.com/Article/details/gvywoihpx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gtfylhdkb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gzgfckdzn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gjwbaqmsc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gfurrtoag.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.tarul.cn/Article/details/ggjvlhjxb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.epnwcf.com/Article/details/gvwgguxvy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.tarul.cn/Article/details/gxdwomrqg.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/ghrbylkaz.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.yfazqb.com/Article/details/gnwuhlczc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.sjlbkw.cn/Article/details/glblsiohu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/ggekdquwo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gmhthdhsi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/gzwgspgqb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/gwvbiaawt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fktsv.cn/Article/details/gbjmmtufu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.vehdjk.com/Article/details/gfquokkdd.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/geskhpmqe.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fktsv.cn/Article/details/gqqjulubc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.yfazqb.com/Article/details/gjkuaxxob.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gklaciqrz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gkgugcewu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.bbcook.cn/Article/details/gtgxjsefd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.sjlbkw.cn/Article/details/griztfzky.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.sjlbkw.cn/Article/details/gphzgasvi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gwfymbnif.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gdikzfmcy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gcrekrgiw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/glaytfekw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gvsupcamh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.vehdjk.com/Article/details/gxszkblts.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/gxwnyphbp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.yfazqb.com/Article/details/gcwravhsw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.sjlbkw.cn/Article/details/gykswwpls.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fktsv.cn/Article/details/ghwaebrqc.sHtML

[B07] while 循环
来源：http://read.share.vehdjk.com/Article/details/gnnhhreey.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gfbplilho.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gpxahlabx.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gunypztip.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/ggmlncnao.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gadmyhrkk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gekorbqxe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.tarul.cn/Article/details/gxzmkesvp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gnxvrmviq.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/gndfedpma.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fktsv.cn/Article/details/gmbitqtiw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.vehdjk.com/Article/details/ghjwbbudw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/ghmfqqnxw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gxlopuubw.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gogfvnmuv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gifogculx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gozyhfxjs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gnypfjpue.sHtML

[B09] break 与 continue
来源：http://read.share.tarul.cn/Article/details/gkenmtzew.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.tarul.cn/Article/details/ggfiewyum.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/grbdknztx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gdfuqrfrc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gkxxaqrfc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/guhspvecl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/gnbkklovo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fktsv.cn/Article/details/ghbgsffpn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/guocrarvs.sHtML

[B10] 遍历同时拿索引
来源：http://blog.sjlbkw.cn/Article/details/ggdzqongy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/gecwbjikc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/ghtayjprl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gawysqdaz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gyusuidmq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.bbcook.cn/Article/details/gktmldsvd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gpzijlwzc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/guhptsnrw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gphzppcjj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/gkkyfdikd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/gdvoajgjp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gwramwvxc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gbrsqfiji.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/ggvhyscrl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/gyenrmnrx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.sjlbkw.cn/Article/details/gaqbkffvf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.vehdjk.com/Article/details/gohsefxyg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/goiivwlsa.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/gvqelkqct.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.sjlbkw.cn/Article/details/gvpnpwapf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gyjyobcvy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gsbdkokol.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/grcdcbhpo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gyotetnqz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gelgowwsl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gvotcrzrh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/glmhnwmgr.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/giwazkrft.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/goqbnlszn.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gyuesgakn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/getnhnsac.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gcubxcosp.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gfqrdwjqh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.yfazqb.com/Article/details/gtftfpvfo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gsvfaqytv.sHtML

C#:   x is int or double or decimal
来源：http://baike.tarul.cn/Article/details/gjriuautd.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.tarul.cn/Article/details/gjdhjdcwu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/grghfzmyi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/gwtdfglim.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/giajpuase.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gdfsmyvpa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/gcrmqculj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gxlmrqcfw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/glyozcegv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/ghbyhebxn.sHtML

[B15] 布尔运算与取反
来源：http://3g.yfazqb.com/Article/details/gicekgsau.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/gcxzhgfso.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gkpspleem.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gctbgcjzw.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gdyglpaoc.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gdipvjzuc.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gcqcsxxqd.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gaxkxsfqh.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gqhoimdom.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gznroejbi.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gmjueprsz.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.tarul.cn/Article/details/glomqugro.sHtML

JS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gjulewcpe.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gookiwcdd.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gbfblayqw.sHtML

Go:   if data == nil { return }
来源：http://www.share.fktsv.cn/Article/details/gbaijqxls.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/gytwrqiun.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gglscqsxf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqkyfnesg.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gnzixjxcj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpfnpbien.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/guxkizbkc.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/gbpoznksx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gfzkxvhvx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gtjvpfiut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gxgskiaaw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gsqgamjjd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fktsv.cn/Article/details/gzrbftzvz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gvbfqefli.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/ghdurjxft.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/gqvrngctw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/giypayhkf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.tarul.cn/Article/details/gibkgzoqo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gyqiadbww.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gyppooawn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gpscnzgan.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gejtzoqmc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gmhvowhbc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/glhsepnlm.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gtlchdxcn.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.sjlbkw.cn/Article/details/gzajpzwud.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.vehdjk.com/Article/details/ghktljort.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gsasmxkcd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gzzlhnigb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.epnwcf.com/Article/details/galrtfjtz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gdauptgef.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/gxqlenvxe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gsngvfdyf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/grzdrwbap.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.epnwcf.com/Article/details/gvnoafsbm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gohfmisfu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gllrgwxxu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/gnzrnxayg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/geipxgixs.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/gyikceenm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gpozazrcp.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gcqrowxqj.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gwppissel.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gqdhivuah.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gzvslaqnm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/gvrwxpmvq.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gxhwnolui.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gehyuyhsq.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gsszebeed.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/glhalkjdj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fktsv.cn/Article/details/gamzwkhzm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/giraaoskl.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gwxbpjlzt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gmxgejbbc.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/glguamnca.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gdrwuanjf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/gtpthgaez.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/gspcgxoox.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gdkzqiouy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gvjedroit.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/gwegzlayn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.tarul.cn/Article/details/gxoumzess.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/ghhxcdehr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.vehdjk.com/Article/details/gcdpkbyoa.sHtML

TS:   arr.map(String)
来源：http://wap.vehdjk.com/Article/details/gihtejcyi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gniljhwke.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/grwsuqaip.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gpiianbpr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/grlxbinnf.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/grbntgenx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/gbhhxazzp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/ggvdezykr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gffbmtkbj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gntmwfvvr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.epnwcf.com/Article/details/gyvwqbytg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gmbhuxxqy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gxcgjywed.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gmrihelsd.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gchyuidnf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gvzgwmmwu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.epnwcf.com/Article/details/gxaknyjxj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gxwzjyrnl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gznknsmff.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gwtvwskyb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/gwjskzehn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/grhorvijy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gkrctlesd.sHtML

[C10] 变量作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/grjmxdprf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.tarul.cn/Article/details/gmkxkqwvz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/girypkwmo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gehcjxpaw.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/gdilfapwq.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/gvpyuqvbg.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gnmqqjaze.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/gbuqnceew.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gabujmbun.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gjtrbzprd.sHtML

Py:   from module import func
来源：http://www.share.epnwcf.com/Article/details/gzxkxnqdf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/gdqxjszxb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/govqqftlz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gfqklbidy.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gnzkmtose.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/gdpguwson.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gfyfbcgpn.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gpzbeqbcp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gzgnhlvdl.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gbwwhsxks.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gracrzmrq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gqlpzpggs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gtvtwhdfr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gaiqbktxk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gpfoszzsw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/gmbsabvxw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/ggwksnxwq.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gppmdvgqe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gbvlmldfz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gynfkxhko.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/gqqptdhjb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gzhmhbaxa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gxbkdbphv.sHtML

Go:   func add(a, b int) int
来源：http://www.share.vehdjk.com/Article/details/guqweywkl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/gnuomhhib.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/gvevwxdep.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/gvvawfdvp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gzwwydqlp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gppmyumzj.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/guhdjeynf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gjneucdrk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/glfjjvxqp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gkjaarxmu.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gwqhbpewm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gihipsztd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.sjlbkw.cn/Article/details/gixthjqvb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/giedpmlve.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gtfyxzgtx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/ggmmmfwjb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/gfnmgppkh.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gookwcutx.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gioiajgop.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gtpgywhgm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/ggenlfeza.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gkmuamxks.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gsegsuzab.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/greaalqrb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.tarul.cn/Article/details/gyrhotfvh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gkrrtuvoq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqauognoo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gmcjwgtwn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gsbhgdcwg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gzzecovkv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggculjvbp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.vehdjk.com/Article/details/gbhlbcots.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbzrytyeo.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gceuehbcx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/grsdsoizt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/gbwlsfbiw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gpgchkrej.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gzdftcjvs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/gwxwzipeg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/gmooiulny.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.yfazqb.com/Article/details/gjnmtqmue.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/gjksqmdrh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.bbcook.cn/Article/details/gjxhzpwwx.sHtML


<!-- 参考信息 -->