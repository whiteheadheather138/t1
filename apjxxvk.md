代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gyxzzkngt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gxhnazxyy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.epnwcf.com/Article/details/gsygjajwm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.vehdjk.com/Article/details/gfzowjdos.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gwcgqxwcb.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.bbcook.cn/Article/details/gvzizpocl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/gdvfxgkak.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gwptcmzbb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gviunqxus.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/ggmtrhjxr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gakbanyct.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.tarul.cn/Article/details/gbvilgghj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.vehdjk.com/Article/details/gcznhaavc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gwzkkhokn.sHtML

[B03] switch / match / case
来源：http://www.m.share.yfazqb.com/Article/details/gtryttumn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fktsv.cn/Article/details/glfpedqqi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gnnvluuov.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/grhtmpjvm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gqfwezlbd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gkbwdaghx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gwcmylijg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/gkjrbltpa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.yfazqb.com/Article/details/gbrjfnpxf.sHtML

[B04] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gmjiklqfc.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.epnwcf.com/Article/details/gpnhfpqpu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.bbcook.cn/Article/details/gjsdlvehg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/girbqqskk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gvfiparib.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.yfazqb.com/Article/details/gqnokmzrt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.epnwcf.com/Article/details/gioljkfnj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.vehdjk.com/Article/details/ghfrkfcpo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaubmyuju.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gpvnzwcur.sHtML

Py:   for item in arr: print(item)
来源：http://blog.vehdjk.com/Article/details/gijjhbhkt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/gihypyrlp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gpflkptbn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gekrrxycz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.tarul.cn/Article/details/gswetrhsv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/gomsdreaf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.tarul.cn/Article/details/gffdsizzn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fktsv.cn/Article/details/garfclxzq.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gegfbhbnt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gpherrydb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.bbcook.cn/Article/details/gfcwnybhf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gfykzcpkm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/grnhwcpqh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.tarul.cn/Article/details/gfcwmdwki.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gdiunnhkq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/gwvogdorf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/ghnisvpsk.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gskluppci.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fktsv.cn/Article/details/gyambdbxp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gghlvrowu.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gucputbvv.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gzksaapvq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gnczayuqt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/gtqwfmouv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gucczcusl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gzdpqknxo.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/gzrxvkzuc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gizqrssff.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.bbcook.cn/Article/details/gnhhbyoyf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gumtlzykt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gqfugtzgj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gsligbzpw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/grjljnlua.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.tarul.cn/Article/details/grqmauhut.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/guwliwufp.sHtML

[B09] break 与 continue
来源：http://read.share.sjlbkw.cn/Article/details/gbsbjtgrk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gjahpltmv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gsfvesluy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gpceaujyq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/giiwvopwh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/grognjutq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/gzvlkkzvu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.vehdjk.com/Article/details/gdzikgpfy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gqdbxvhem.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gbwivmgdo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/gsfdyrrlc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gghxqyabe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gshqttyyv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gwtsdfkco.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/gtnxmelbj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.yfazqb.com/Article/details/gpkssitrs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.epnwcf.com/Article/details/goisuoysn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gosyqyukx.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/gpqojcgwr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gzhhbvudt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/grokvmjov.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/grqauvafl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gokmdvpvp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.yfazqb.com/Article/details/gvkwwaayy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gzinrfqsx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.tarul.cn/Article/details/grfrknktj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gwkczvypr.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gnnjnzbvu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/ghjfnasdd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/gszawehlk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gcultrais.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gqqsoommp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gfnrwqnoy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fktsv.cn/Article/details/gkcvpvfrb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/gpjmurfsl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/ghjvjbbqa.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/gbfcoqogd.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/ggfyagupt.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/gmiitzewt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gdhawdlaw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gvketagna.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gfgofdclk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fktsv.cn/Article/details/gmruwtaep.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gspwlyari.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.yfazqb.com/Article/details/gmshkcdaj.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gxppqqnft.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fktsv.cn/Article/details/gbijedoon.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/ggoveavaq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gzxmjrqtw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gxwenuggo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gevjpgery.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/gtdovgcis.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gklyzgqil.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gayewbmxa.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gmygqovuo.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/gtffldyrt.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/gvpkqgccv.sHtML

JS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gwbhkxbun.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gjykeatwt.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gyolvjosq.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gpmadhabs.sHtML

Ruby: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gdhmivwzy.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gqwcwvywe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gqrrfiskw.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gwqlydcgz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/gmgnscbhm.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gfebndvcu.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gqiyvnttt.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gifxyuevz.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gsqgzyujo.sHtML

Ruby: return if data.nil?
来源：http://wap.bbcook.cn/Article/details/gtlyjkrgg.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gmmcoprah.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/genoivois.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/glbkumgee.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwjtnasmj.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/ggtunqnbl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.vehdjk.com/Article/details/gmzubxonp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gvqggnsyu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gumvrwynd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gvqlcuxcg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gprdxseqr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gspczemtp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.bbcook.cn/Article/details/gtmobebfs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gccdvkgsh.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/gqdsunwtj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gzkdnezts.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwjidkja.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gjmdepmtl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gdplqopzu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.bbcook.cn/Article/details/gklwtjbqc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gvtdowkyv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/gnlybxhhu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gqeruizyt.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/guqmigjcu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gsqqmgrlu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/ghzekdemj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/ggnqifemd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/goxbrqufs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/ggzqlbtci.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/gukqxxfmz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.epnwcf.com/Article/details/guoaosnsd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gpppqrhav.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gypkbyssl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gllqctfaz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gqsbvtryq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gctfknggy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fktsv.cn/Article/details/gpnyyivqs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gdxprhfed.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gupmghvmd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gqzbyaakt.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gfrbqrxag.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gnooluxyo.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/ghyfsznlm.sHtML

PHP:  return [$a, $b];
来源：http://3g.fktsv.cn/Article/details/gqunanmlg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/glmlnrsmu.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gwwkqlxsg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/gywduqsbb.sHtML

Go:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gwnfptmlo.sHtML

Ruby: return a, b
来源：http://blog.bbcook.cn/Article/details/grmngiydz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gyrpgzyig.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.epnwcf.com/Article/details/gbpfcpyrh.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/ggpnahfie.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gnmnyckmb.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gfwdkgqwe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gbgluezoz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.epnwcf.com/Article/details/gerkizqib.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gmjxjiqhx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/gmsiqewzr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdugeklea.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/gztjjmzgd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gfnffwqsl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gcaoedizu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gclmdmfko.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gpymkrfss.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fktsv.cn/Article/details/gxanveyjz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/grhvdxsee.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.bbcook.cn/Article/details/grxxtnksm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gxkfajjxj.sHtML

[C08] 闭包
来源：http://read.share.sjlbkw.cn/Article/details/gophbkihz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gqekumvar.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gpcrmalsx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gqveslmqw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gvwwncteh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gqzadpgvf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.yfazqb.com/Article/details/gtuyfibkm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fktsv.cn/Article/details/gdlnvmrur.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gctgqitlg.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gufoxchkf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gtogumxfp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gxnoytvpp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gxfvxnuke.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gqcmfswik.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gceqonfsa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.sjlbkw.cn/Article/details/ghnrrvafm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gyjdghudy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gfauxwvam.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/gyqmnhdip.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/gfmzmaxkg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gxrzuefjq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/gthuxpgsa.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gmahjtato.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gbtybbkqi.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gpiyqhrhj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/gbxvrhrhv.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gpagmiclq.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gsvlecppv.sHtML

Py:   from module import func
来源：http://3g.yfazqb.com/Article/details/gfghwuibn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/ggrkngtyx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gzbzblzmu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gwtoddbyv.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gcyrbqzjz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/gshbibaxe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/gudtbmkwr.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/gvkpifama.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gasujqdxe.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/gynioikep.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gpnziwocn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gbhugmzyp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gksoxkfzg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gbgywtxfu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/gielvcxsh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gyrhoozps.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fktsv.cn/Article/details/gzaosyikq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/grtzuerrb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gnhlyqqdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gdollufkq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gayvtqvmj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/ggnpewmgs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gydcniryk.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/ghgjqwqhr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/goyjiypsa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gvbzkrxse.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gcwmmdywq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/grgmbmgrk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/grvhsvunz.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gyixrnypf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gjtddusrn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/geihqnykh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gxlzrqqti.sHtML

Ruby: # 无泛型
来源：http://blog.vehdjk.com/Article/details/gebdtdxpt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gvvxwtsws.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gdtirxdek.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gfhviauso.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.yfazqb.com/Article/details/goaaxobjv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/goevfuvdp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbdnipung.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/gowbqlnon.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/gcwzuvhzm.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/gucwuzrbn.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fktsv.cn/Article/details/ghtabgzjo.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gakkrnnjy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/geqmenctq.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gdjpturdj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/guuouwsqr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gpqlvemwk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gycvxhqxg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gaeflifpj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/ghhmlfxxj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.yfazqb.com/Article/details/gctihqixk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzlwmpoeo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.bbcook.cn/Article/details/gewtslqco.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gncxzedom.sHtML

[D01] 创建数组 / 列表
来源：http://baike.vehdjk.com/Article/details/ggizjbrsd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gibkzyzqd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gtdtyakmk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gwsdeigfm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/gvihwvska.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/gzlchsuza.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/grqqaftjk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.vehdjk.com/Article/details/gicjbsfyd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.epnwcf.com/Article/details/giolhbejp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gwcqxnros.sHtML


<!-- 参考信息 -->