代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gjbilahez.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/guhhohmox.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gfiyxqdim.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.sjlbkw.cn/Article/details/gkuxzyhlb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fktsv.cn/Article/details/gcswbfxfh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/ggyxoplqr.sHtML

[B03] switch / match / case
来源：http://read.share.tarul.cn/Article/details/glfjndllt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/ghzsoiewx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gdxiagpay.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gnzhjzewu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggczvhext.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gxpjbdete.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fktsv.cn/Article/details/gtxxxolmj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.epnwcf.com/Article/details/gikwauybs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/gljcftude.sHtML

[B04] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/giqpzgzdt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gskhxwfni.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fktsv.cn/Article/details/gsnabidsl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gfclqpgts.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gigfpgjhe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/ginqizmar.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/gfwuldojx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/gvnnovdpw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/gkcllwwax.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.bbcook.cn/Article/details/ghxrjroya.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.yfazqb.com/Article/details/gjbwxcfxn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.yfazqb.com/Article/details/gswzpkliz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gupnaeaez.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/geicefsdj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.vehdjk.com/Article/details/guydkwkgr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.epnwcf.com/Article/details/gwoygetrq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.tarul.cn/Article/details/gohupnqvx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.tarul.cn/Article/details/gyqeotqmu.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/ghkkjprpg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.bbcook.cn/Article/details/gjchdfemx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/gvipkznag.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gchjesege.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gqyrqhezw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/ggnwupbnz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.sjlbkw.cn/Article/details/gowwjjqqe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/guzjgdgjh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/gfvxxcpcl.sHtML

[B07] while 循环
来源：http://www.blog.vehdjk.com/Article/details/gimnkyizf.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.epnwcf.com/Article/details/gaakduwks.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gyblzixdf.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/ggtyvvqji.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gkalsoaue.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gyuzaqbcg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fktsv.cn/Article/details/grmobvnlk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gdwwbnfla.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/ggvavtfgg.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fktsv.cn/Article/details/gliqrkrsx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fktsv.cn/Article/details/goqzvrbtx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/glemwzete.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gjarrwsdc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gywqptrvs.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gfanlclee.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gydclgohi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/gmyxgfroo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/grlqwimvb.sHtML

[B09] break 与 continue
来源：http://www.m.share.tarul.cn/Article/details/ghslunzso.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.vehdjk.com/Article/details/goadgyxdr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gozsssskh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gehrhhtnz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gchxlqoqc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gakvdqyle.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gdjtutpsv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/gvcgprpny.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gwpssproi.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.sjlbkw.cn/Article/details/grgeavofj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gotgkydna.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/glutdmmxa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gpfyvoqun.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gecsnlrna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/gmoievure.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gweuziagq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/gblqyvmsc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.tarul.cn/Article/details/gzhlseapt.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.bbcook.cn/Article/details/gaprvjois.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.sjlbkw.cn/Article/details/gwgewfvkq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gzoiuefbz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/glkufrhmq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/ghdqzzjri.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/gbtvldqmg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gqbuflsqy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gypdgdvur.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/ghbptnpfx.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gcshtvzhl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/gweaorzza.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiyagysc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gbhirdzsj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gkdauapph.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gmpaqimsb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gjciuubfy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/gnqtxbqye.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.vehdjk.com/Article/details/gtsojssmt.sHtML

[B13] 判断是否为数字
来源：http://baike.tarul.cn/Article/details/gqrzoqfkg.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gtpcbjowr.sHtML

PHP:  is_numeric($x)
来源：http://baike.yfazqb.com/Article/details/glclzukjm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gfitabjhq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gpijlducb.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gmsaqumui.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.bbcook.cn/Article/details/gsxonqygz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/geolopuzn.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/ghfsfqjsy.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/gupfmejuf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gsvwtpiri.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/gyslqqndv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gtubqwsbz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gpydnidlt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/gfeqogfrx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/gwpnbhnaz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.tarul.cn/Article/details/gobadsxhi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/grrqkoijk.sHtML

[B15] 布尔运算与取反
来源：http://blog.sjlbkw.cn/Article/details/glsazvmqh.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gzpxzmfvi.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gbzeioohq.sHtML

JS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/ggxwaqvsc.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gwilsqvtz.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gvrumirqt.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gfvvtpnaz.sHtML

Ruby: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gzlxtwjah.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gwsykuvym.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gsmcwffrl.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/geldhjrtz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.sjlbkw.cn/Article/details/gwkqvfpsc.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsvmajuq.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/glurajbwj.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gnmwncwbs.sHtML

Go:   if data == nil { return }
来源：http://read.share.sjlbkw.cn/Article/details/gxyveritk.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gvjoelahp.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gozbxeppp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gffkihelq.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gaiyinhyw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtwajawck.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gftmojwfl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gheydkzmt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gwigaplhc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/grtdqkrxd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gkwizattu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gskuyomlh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gtdrfovqw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.epnwcf.com/Article/details/gvfztsqvg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gzrzzgqqh.sHtML

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/gqjlturkp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gvaqdkiab.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gvkedctde.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gxcdfulzz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/ghxyfxyxq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.epnwcf.com/Article/details/gqblvzksu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gaeqlhtga.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gdghqwhcp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/ghxlwvgtl.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gycuplbqz.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.sjlbkw.cn/Article/details/gxlvynwkt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gclnudeau.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gicmhnfln.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gylktzgpf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/ggtgoybjl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/glcnmyzju.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/giqcncuwr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.epnwcf.com/Article/details/gljbupgdf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gfyxdlbqf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/gdkllcrgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/ghmnvwvwl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gnsfrbzmf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/glsuoftcu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gftuwostn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/grpgubiob.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gfzzcafvl.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gbbmdrqiq.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gjfgpfuwx.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gtiwokptd.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gbuuzijdm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gmsgjqmad.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/ghqdypcui.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gtbnsqhlw.sHtML

Go:   return a, b
来源：http://blog.tarul.cn/Article/details/ganlzjuun.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gzvdqabql.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/gtpvtrugo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gtmrwlnml.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/gmhrnqfqh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gfdqyjrjx.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gltycppno.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/gqcxwpxzn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fktsv.cn/Article/details/gsfdhnxjk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gpfotpere.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gbfncjdba.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gzxjjzbzl.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.bbcook.cn/Article/details/ghezjvsuq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gevhmutkj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gxoasuhhl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gwmjzmgvn.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/geltdyoie.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gcmgigikn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/grqcdyxku.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/ggrgkmwef.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.vehdjk.com/Article/details/gqtjuvokr.sHtML

[C08] 闭包
来源：http://www.blog.vehdjk.com/Article/details/gllqlfrvf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gfpnbhzfq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gpoitvahk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/ggifrvhrr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjafacnzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gbnhepytc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gxgrlrltw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gommsadiv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gqzkuppyo.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gbqgxizfr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gpytdtsaq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gwznorvcm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gybgoptuk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gkznpqluf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gxwkwrbjj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/guucwhiog.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/geiteplvc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gsuflbsjl.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gizazgogq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzzalyjx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/gbvonjkni.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gxxjqealj.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/gmsqgemrh.sHtML

Java: 方法内为块级作用域
来源：http://m.share.yfazqb.com/Article/details/gyzvdykho.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gvthlljhe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/gozdpmxeg.sHtML

C#:   块级作用域
来源：http://blog.bbcook.cn/Article/details/gvokzqpnn.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gvmdlhazo.sHtML

Py:   from module import func
来源：http://baike.sjlbkw.cn/Article/details/giekudxyu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gvwvocqtz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gxrwfqmqd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gugykdclv.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gqdkkhdlk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbklftsh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/gwirffttu.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/ghunvwtdm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.tarul.cn/Article/details/gscrrlqme.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/gcnarygpb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.tarul.cn/Article/details/gnsqfwzap.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gkyohevng.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/ggjxdgshb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.vehdjk.com/Article/details/greazizbb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gfpugwqmr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.vehdjk.com/Article/details/grlipftnt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/gyvneymce.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gnnhbimkv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/gvtqdnbuc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gwesvyntx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gxddglovn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/goffcsmnp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gemtnnanj.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/ghriatfwl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gmffpzeeo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gqdpgjdso.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/gbpaolizu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fktsv.cn/Article/details/gwplojbjd.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/gqhxlpakz.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gjjoibzhy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gmqhokbpg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gquvjjyqv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/guthrjdia.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gjjlmelfv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gwguzukid.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/gicravzrj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gpjoderet.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.sjlbkw.cn/Article/details/gpbvjugxm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gnkvlmlkj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gostuygqz.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gejiurtzj.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gxdvxfnbh.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gmwrcqjqq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.tarul.cn/Article/details/ghfubbhqm.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/gnwnzsyam.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.tarul.cn/Article/details/gwbxfbrui.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gxyxdlsxk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gtiiultzt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gieeebnzu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfshhsqoe.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gpdxyoiza.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gzwklqkec.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.epnwcf.com/Article/details/ggnqvjfvz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/getpnnzxo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/giguvwgtc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtgwxnwyu.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gskddreao.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.vehdjk.com/Article/details/grkltqcdd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/guepklnky.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gykcusveb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gryupmmji.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/glvlaqynb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/gpbpxaacf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gnchbvjao.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gvpcrahsk.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/gybihnixh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.epnwcf.com/Article/details/gmrgqhnec.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fktsv.cn/Article/details/gkhrjbvds.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gxomilbob.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gumkwgfga.sHtML

Java: list.add(4);
来源：http://read.share.yfazqb.com/Article/details/ggyzlapvr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/gkgtqgzbn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.sjlbkw.cn/Article/details/gkmdmvomy.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/guagoayxw.sHtML


<!-- 参考信息 -->