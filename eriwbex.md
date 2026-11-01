代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gtgchltfi.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.sjlbkw.cn/Article/details/gwksnkusm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/gyuyiking.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.yfazqb.com/Article/details/gjpuvxlbw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gcqnjnkqk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gfjmvnwmj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gwoqgrjjq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fktsv.cn/Article/details/gdlyfyxwe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fktsv.cn/Article/details/gqbxsffvn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gbisgzpsf.sHtML

[B03] switch / match / case
来源：http://mobile.yfazqb.com/Article/details/gyxzjizuk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/ghjkceppw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbbvbjyhe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gfrpudeys.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gnnxbqchk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gmylpkpfg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gojalwcqi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.bbcook.cn/Article/details/glpozkbnh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gmwfqmqvk.sHtML

[B04] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gesrwpxqs.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.epnwcf.com/Article/details/gtigbkgen.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/glcnmhgtr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gaijggyaz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gvhyyyymj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gdjyueamb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/gwzuhcimz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/gnlgpyjny.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gkevxjtsh.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gjlfrjlxg.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.vehdjk.com/Article/details/gdsyeddyz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.vehdjk.com/Article/details/gbwubeeus.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gbuhkpbru.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gtyhxythi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.sjlbkw.cn/Article/details/gvbwepxnq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.bbcook.cn/Article/details/gxkljghjf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gafzlfmhp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gstrvekxx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gfusfzsic.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.sjlbkw.cn/Article/details/gvbmfnhgk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/gehsylynk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gxzqxjebe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/ghpdzhgbs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.sjlbkw.cn/Article/details/gdhcxxwkv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fktsv.cn/Article/details/gvcbtutrp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.epnwcf.com/Article/details/gwgxpuxcn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/guelrfbxu.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gtcekxtlo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gldxycomy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gnzfeqrmu.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gpwxbstyh.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gyrjjflyv.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gnnukdvwl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/gwiumwgtt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.epnwcf.com/Article/details/goanbbtoj.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gxikbxauv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gmevjkouu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/gewwwcuwh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gsrrbvlqf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gmkkpqmto.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gqnybcjwn.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gvlkfzaio.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/gkxvvzmqx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/gqkcapxxz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gtzjtvplo.sHtML

[B09] break 与 continue
来源：http://3g.tarul.cn/Article/details/ggndhoych.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/gzsuevgov.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gbzxaxwbx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gsktseuru.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gxtkwysbl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gewqopjci.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/grnregjgd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.vehdjk.com/Article/details/gazymiuxc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/glfquhgee.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.yfazqb.com/Article/details/gdnhyllzy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.tarul.cn/Article/details/gvhzvgnla.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/geowauacq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gqbtscjeu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gymsmpcun.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/giimiwiju.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/glgbfqgpb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gzgtontuk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gwtmnwdfx.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.sjlbkw.cn/Article/details/glpcwxemr.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/gjifrkzta.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gpmpnwgzh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gkzmkoqky.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/guudayjww.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gfpcxmfpm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.yfazqb.com/Article/details/gilebetib.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/gkxlgneon.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gwnxmazws.sHtML

[B12] 跳出多层循环
来源：http://mobile.yfazqb.com/Article/details/gvibgupub.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.bbcook.cn/Article/details/gkrjglahm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gnpuvwyon.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gfpazbkwg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gunchsqol.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gdhokukyx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/geoitfcuj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gpktkmzuz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.yfazqb.com/Article/details/ginqsqhzq.sHtML

[B13] 判断是否为数字
来源：http://blog.vehdjk.com/Article/details/ghqmufkcx.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/galycvqcf.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/glkbnwmak.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gyyhmppmt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvzpydwv.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gfqbebqcu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/glmhbexfr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fktsv.cn/Article/details/gqtuyhmfn.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.vehdjk.com/Article/details/gyujtmqug.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/grmjsltri.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gcskkjfot.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.vehdjk.com/Article/details/grdenarvw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbzpcjrkz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gkjvjfxmk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gtemfnnya.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/ggypjpqrf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.bbcook.cn/Article/details/gfzudqaor.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gvrxxeizp.sHtML

[B15] 布尔运算与取反
来源：http://blog.bbcook.cn/Article/details/gxedhoewz.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gwypjxyyd.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fktsv.cn/Article/details/gvmkmalgx.sHtML

JS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gpgsakdgd.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gorceqwhh.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gtdbdberb.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gjrqedjtv.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gpcjnldvc.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gusswxgzw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.sjlbkw.cn/Article/details/gutzwimrw.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gjdwmkmps.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/gjemvemsr.sHtML

JS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gerbinlbr.sHtML

TS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gxjttlnzj.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gqdarblts.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gdbcvoctt.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gbpgwekuc.sHtML

C#:   if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gynttcxfv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcygaytkw.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/ghxyqnecg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpinexznf.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gfbpdhcfz.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/gslmfkmpd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gedgiowow.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gtxsdfsgp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gwypmkinf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gcfdgbtqa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gkmhjasnv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gseiqwtkh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gpxgufflt.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gcyoipapo.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gzafgblwe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.bbcook.cn/Article/details/gxjkyohsy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gdakjldig.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gqswddxya.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/ghrtzzrbt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gbnzzkaov.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gotnqxalm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gyyixvmkp.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/gnjledzdx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/gcgrusgfv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/gpdzjxxqx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gwdvjgpen.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gphfwgogz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gcwumxlbi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gpjaztklm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gpxkpfkie.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.tarul.cn/Article/details/gujercmjo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/glpbzghrc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gtjbceshj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.vehdjk.com/Article/details/gzhjguwrz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gxipdkjnj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gfgcgdotr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/gsbldvocv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/gkxnisrag.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gzxqanxed.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gssyppdjb.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gnltxiuzf.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/guhjqjrcu.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/ggrfckzud.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gylmaldlb.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gkjdabgda.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/gpuawvskd.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gmalwcmwv.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gzhyyzfkr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.yfazqb.com/Article/details/gqsqzghbl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/gjlgyvupg.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/grmarbfft.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.bbcook.cn/Article/details/gsggrfpja.sHtML

JS:   const square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gedcqumyk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gaohosuzk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gbyfxaegi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/glcdiails.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/gcdwvhris.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/glhridfjk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gxjrmfdrt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/guunokmnv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gasathajv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqimlzgmb.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gjwjslpjn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gvvcuvsig.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/gldbptfrz.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/gclnvurps.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/gbocawfhe.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/gtpnxygqh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gfwkvshvh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gdhmklmzt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gvzhatcij.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gadjnogmg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gbnrmkbul.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gwbhazovw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gjwjcmzoq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gflclohvd.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gtpmwklsa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/grmurtszv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gbbkqllfe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gfdgaxkbs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gearknpes.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.tarul.cn/Article/details/gacetpwxf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gqffcbgmo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gjzqxtmtl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gwmqkkeiq.sHtML

[C10] 变量作用域
来源：http://wap.epnwcf.com/Article/details/gmgsdwwdv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/geabkytwp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gkwgxtzom.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/grclxoswy.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/gyjoogvag.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/ghexfkzzh.sHtML

Go:   花括号块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gdkbetkat.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gnvgnwkcu.sHtML

C#:   块级作用域
来源：http://3g.epnwcf.com/Article/details/gqkrhriux.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gvozbrgir.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/gvvveukyx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gcgchacja.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gbmspxdce.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/gihfgpckk.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/gqgqlmabj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.bbcook.cn/Article/details/gaeoecdcc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.yfazqb.com/Article/details/grydofggh.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gqotdijwj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gnbjtvtiw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/ganxkomwb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/giykablpx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/ghnngjxlv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/ghxvthlfb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/gwivbhikx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gdzpvpdsl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gbqwoirrz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gciqsvwmk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/gbzgavfku.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/gnutmipbt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/ghowjtzly.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.epnwcf.com/Article/details/gqqphhytr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gjqkixdzm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/glqpsealb.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gcvfqirki.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gedcxdkll.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gnolwukda.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gjcbjpdyj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.yfazqb.com/Article/details/gclkkxmhx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gfsxxavsv.sHtML

JS:   // 无泛型
来源：http://read.share.vehdjk.com/Article/details/guyawsnng.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fktsv.cn/Article/details/gwiejmkcj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/ghouarjmg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.bbcook.cn/Article/details/gvnmbegfx.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gmzvjoyle.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/gjnvuxdla.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/geffhaarl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.yfazqb.com/Article/details/ggplxekac.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.bbcook.cn/Article/details/gwydjnuuo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqjnienyk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.epnwcf.com/Article/details/gtzbspyul.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/gatrihxly.sHtML

Go:   // 无解构
来源：http://read.share.bbcook.cn/Article/details/gkqjmshaj.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gplsdvccp.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.yfazqb.com/Article/details/gdzxbugag.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/grwpmbhan.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.vehdjk.com/Article/details/gxupcfrrz.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gievnqdpr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.sjlbkw.cn/Article/details/gyidyjkjs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/gycxjgqke.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gcbuxfolj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/gozwficxi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.epnwcf.com/Article/details/gfekjccye.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gsvyzcbgz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdmartljd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/gfoqanrdj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggewalmsl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gpmowkfxi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gadlauoqz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.yfazqb.com/Article/details/giazokagl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gwadgjqeo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/grrrkjrru.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/gniewanzy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.vehdjk.com/Article/details/giisxjuir.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.tarul.cn/Article/details/grrjkhbvh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gtkhsdfkg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/ghlppetms.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/godwsuuqr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gaoaoydih.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gpvakebse.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gdufxnnlg.sHtML


<!-- 参考信息 -->