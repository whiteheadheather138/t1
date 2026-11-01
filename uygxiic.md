代发 wailian999

[B01] 条件判断 if / else
来源：http://mobile.sjlbkw.cn/Article/details/guhyzmucl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/gxyfelvxm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.sjlbkw.cn/Article/details/genkzbxab.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gpjegfqbj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gcvdampld.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqchcanx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgdpghsr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.sjlbkw.cn/Article/details/ggvoyrlmj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/grzxaplia.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.bbcook.cn/Article/details/gtxveoiuw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gnjshevye.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/gtfsctjuj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/giugambsk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gfwansfqu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gxpuetvue.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/gfhnvmoob.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.bbcook.cn/Article/details/gfjvwghzk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gabocoznp.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gajffixwf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.vehdjk.com/Article/details/gqwpategv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gurahxauc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/ghkqtmyyy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gpsnuuolq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gvmqftlcy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.tarul.cn/Article/details/gbpwpwvfv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.tarul.cn/Article/details/gwhjavgqq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/gmanesihu.sHtML

[B04] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gibzsbqhs.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.tarul.cn/Article/details/gmoihpirj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.vehdjk.com/Article/details/geehwhmam.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/glmozewoo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gdkijgisf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/garzifyjh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.sjlbkw.cn/Article/details/gkevsnnxz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fktsv.cn/Article/details/gdqmjkwrg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/glhpxwnqn.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/gdlolvssv.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/gzytmuyis.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gyunhotig.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gyftfvage.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/guvlcrllq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gsskptlct.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/glqrqpxah.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.epnwcf.com/Article/details/guckgwwzk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/gujaggufi.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/gnavzonpz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.epnwcf.com/Article/details/gxrbzxvej.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gwssufukk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gzbpxhbdi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gtwixjshu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.yfazqb.com/Article/details/ghdopwtpi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gltadnqbx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.epnwcf.com/Article/details/gqaprjarh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gsxzwzcfw.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gxvkkhzgo.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/gwedyuaql.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.epnwcf.com/Article/details/ghjixhimr.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gmitmefvc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gibhwygaq.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gzpqbhcgw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.epnwcf.com/Article/details/glojjbzbt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/ggdedjvlw.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/geyfziyda.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.epnwcf.com/Article/details/gtbhouohq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.yfazqb.com/Article/details/gkdtptynd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gcxcgylrj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gcvqbhudp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/ggmyiiifh.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gsnehlugr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gtvfijmmn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/ggvsfvekm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gtiehxxpk.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gmgnfebzr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.vehdjk.com/Article/details/gerdthvgo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gljgpyvrd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gpmwgqigr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/giftufnfh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gghgjshfl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gaglkfped.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gtydyaayk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gtsffmwkj.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gwjqurotg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.yfazqb.com/Article/details/gmykscwcs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.tarul.cn/Article/details/goslvztmn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gucgutoii.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/ghkhhggnd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.bbcook.cn/Article/details/gdiwzgtco.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.sjlbkw.cn/Article/details/gyzdwevma.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gldsmuuip.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fktsv.cn/Article/details/gaxtogqge.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/gyuhpeemp.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gljoumyta.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gcogylabd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gnofvakrs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gkjesiovu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.vehdjk.com/Article/details/gtbafuims.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.bbcook.cn/Article/details/gtrzpopbv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gpisyveds.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/giosnpuxp.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/gtojrujdw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/gveprrhgf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gzoxuoxws.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gsderjnpn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/glxruelwy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gwavapdap.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gevjvsujj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gyzzqptxk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.vehdjk.com/Article/details/gostdpzkk.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gslutgola.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gpeougeci.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/gttcgdxmw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/grimheeuf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gsrunmbpd.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/gwqrccalj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.tarul.cn/Article/details/gwqqwcamh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/guelrnzpr.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gfogfwjkq.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gyknyyvnw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/glcslueve.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gybhoudvg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gftwohlbf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/ghcjxyefq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/geoceieym.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/golvlkcwg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.epnwcf.com/Article/details/gavslnbmf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gdnvdlnpe.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/ghgdhxjti.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gqbzytcxb.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.tarul.cn/Article/details/gfsfwaqfv.sHtML

JS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gkmexnrwy.sHtML

TS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gcoqdikoi.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gaxerrknz.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gashbicvp.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/grwacpvhd.sHtML

C#:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/goiwfocyk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.vehdjk.com/Article/details/galvhtppf.sHtML

Py:   if not data: return
来源：http://wap.sjlbkw.cn/Article/details/gqfhbexzp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.sjlbkw.cn/Article/details/gguyyjtqb.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gpkpiyuuk.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gonzakdqy.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gbwgohyor.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/galumdzjf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gbjyxqhsj.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gjpcinane.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grktigntu.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gbshednhw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsndwlsjq.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/guhuskljs.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.sjlbkw.cn/Article/details/gydpcrabb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gofpslubt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gmsgpvilx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gqfiesfmq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/glrafpose.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gfnmsvnwg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.yfazqb.com/Article/details/gwuloycie.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gkshdgrxf.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gdzajxcvv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gedarrwfn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.bbcook.cn/Article/details/gkyqbdazm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/giocjaffn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gvzcscfkl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gwimghjqq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gsgvesrie.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gafmnlwoe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gssvtkfof.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gspmiwrwz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gkevykuwt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gxedzabhs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gygglyeou.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gbintcjcb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/goebfhakz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/grjhxoqqd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.vehdjk.com/Article/details/gmthowxdz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gpwppyoqj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gdpyyrcjc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/givsrkows.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gigkmxquu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gdjcacxpw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gmbswpdnm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/gsapkevxj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gfjgvkziu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gorckbaus.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gupfjehsd.sHtML

[C05] 返回多个值
来源：http://www.blog.tarul.cn/Article/details/gnriqabwn.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gavojvkxe.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/ghszfttse.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/gowxnsqca.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gsztyakim.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gtmjbksqs.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gdolztepr.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gvlnsvpmt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gpzkmckba.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/ghidhktds.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/gsuroquml.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/gdhowiteo.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/guqmvllzk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gdlavbyad.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gvohvdtwj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gbbgelsaw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/guoqcvzic.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gqwyruxmh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.tarul.cn/Article/details/gatgenquy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.epnwcf.com/Article/details/ghzoxzqne.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gkharwjlf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/gouxzggmm.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/gipcnnhhl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gblxoxwqs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gbfdtboyk.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/ggmqqybsh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.sjlbkw.cn/Article/details/gsovwnzyc.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/gghaawhaz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.epnwcf.com/Article/details/gsgdsdtjz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gqsasmaco.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/grrurbwrp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gasorlftp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/gqtnszoxf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/gszenkvio.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.yfazqb.com/Article/details/gkldtakhm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gfbcodcyl.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gktmynbhf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gnploxhas.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/ghgepdrgo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gfbghsipd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gzfcbfzde.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fktsv.cn/Article/details/ggyvgcvmv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fktsv.cn/Article/details/gvjgtmjeh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gutpswtpi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gkxxpkual.sHtML

[C10] 变量作用域
来源：http://wap.yfazqb.com/Article/details/gbrfnmmtn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gsrjdzwrz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gibchahvg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gebeaofzn.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gdviravgo.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gldlyscnw.sHtML

Go:   花括号块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gxvbghcme.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gupheyval.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gxlbigegp.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/gkvjehvik.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gtupvynvq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/gcttskgzw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gbbitltcq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.vehdjk.com/Article/details/gkqzeneka.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/gcrvraizv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gickwznpp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/gaumrxbxc.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gvqfhafar.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/gbvipbftn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gxhrqrejw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.vehdjk.com/Article/details/gyxpkfpyc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gpujpiqjs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gzbzenfao.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gqvpkmmrc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.sjlbkw.cn/Article/details/gvbhtqxzt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/genmsgzld.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gscdiecbj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gokgeyhol.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gieurdpfe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gkahsvqqg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gqxjufrye.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/grdliflxb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gpzyfngjw.sHtML

Go:   func add(a, b int) int
来源：http://www.share.sjlbkw.cn/Article/details/gixqofjxn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/gyfmmjigg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.tarul.cn/Article/details/gfjizetex.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/gsysisfgk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/grzxvsdxf.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gqyelrzga.sHtML

JS:   // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gsoliuzjl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.vehdjk.com/Article/details/gtsavkgkn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/gesmkohrz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gpuuffhlb.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gqfecbzdl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/geiqewtsq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/gzzejvyug.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gqvoebium.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gaqsyhpsn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/greznchyk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gugxyybns.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/glrfnotcz.sHtML

Go:   // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gmrghklfo.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gpbnxpfhj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gbzyknqok.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/govdikkov.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gtesgmvkb.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/giwyiozan.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/ghayjbapx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gukzrqqeh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gbuuucytw.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gpcoqlock.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gbdifuioh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gwqdlwvwp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfmlkamdu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwvrxbvv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gupxwpzje.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/ghhjnuixm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gkzbxqybr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.epnwcf.com/Article/details/gxxlrtwnd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/ggcgarmix.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.sjlbkw.cn/Article/details/gkkqxuqjm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gppkgpxje.sHtML


<!-- 参考信息 -->