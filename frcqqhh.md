代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://wap.tarul.cn/Article/details/gwywqxnfl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.tarul.cn/Article/details/ghdalxeli.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.sjlbkw.cn/Article/details/gnnifdnbn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.vehdjk.com/Article/details/gnarjwxyi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gazehoqkb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gadqxfnat.sHtML

B. 流程控制
来源：http://wap.vehdjk.com/Article/details/gxihzidsu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gobgchvkj.sHtML

[B01] 条件判断 if / else
来源：http://baike.epnwcf.com/Article/details/grdfkuxdp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fktsv.cn/Article/details/gqhagfpzm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvyvirwxl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gkmlxxzur.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gqlvxztja.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/glgshfiqn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.vehdjk.com/Article/details/gblhgqogt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fktsv.cn/Article/details/gqaqpfcsh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gyrbpjqrh.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fktsv.cn/Article/details/gqgssoacg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.epnwcf.com/Article/details/goklmxicz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.epnwcf.com/Article/details/gppshqlgj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gpwqguqrr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gwgkyiebi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gjpgbikva.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/ggfejebkl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/gmjepttpc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gaduvjgfo.sHtML

[B03] switch / match / case
来源：http://wap.epnwcf.com/Article/details/ggutweikv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/gpbltxgeu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/guvtslwse.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/grwugsydz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gewyvucwl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gfhlrzopt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gbqvuifxm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/gvkilvslo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gemfnbrbq.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gctvrlwyh.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.epnwcf.com/Article/details/gkogadvpj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.sjlbkw.cn/Article/details/gaidszymp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/grzaugcyj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gayhajpyd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/ggfpeusmg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gyfpbqfbk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/guukegiim.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.vehdjk.com/Article/details/gkdcekoxg.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.epnwcf.com/Article/details/glflxhisp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gsosmlycy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.tarul.cn/Article/details/gwosteuvs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gxidysieu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gaydhgtnp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfaejnpx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.tarul.cn/Article/details/gyrgsfhhh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gzkxsikce.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/ghhugljvc.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gnozakamp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/gvqplzdlf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.yfazqb.com/Article/details/glqbudkzt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/ghjpmrvdy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/gjoemqdbh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.vehdjk.com/Article/details/gnzxtamnm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gicbyuezr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.yfazqb.com/Article/details/goocfpmfr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gnhttowjp.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gszaljtlc.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.epnwcf.com/Article/details/gdnarbjmm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.yfazqb.com/Article/details/gneukvckm.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/ghaegzijd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gdbitpyzk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gagvpjjyz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpklejtl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.sjlbkw.cn/Article/details/gnelxlqou.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gogoufmlg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/gmrtkugah.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/glurcsyod.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gvjeoxmyp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gkaodcnwq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/guuimffjf.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gcqdfhthf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.tarul.cn/Article/details/giqccbryq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/glewhkukx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gewlrijbs.sHtML

[B09] break 与 continue
来源：http://baike.epnwcf.com/Article/details/gndmoolxt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.tarul.cn/Article/details/gqvqivuso.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gcyqeieub.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gjtduhydy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gotcqpvep.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gghguitql.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.yfazqb.com/Article/details/gxonagnkr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/grgduzneh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gumakjwtn.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.bbcook.cn/Article/details/grvwdhlzc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gvhkcjtqk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/gcjjyedtc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gucoewthh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/givmeaamh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gxwiqmgzt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.epnwcf.com/Article/details/gvkcaiwwp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gocmfryay.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fktsv.cn/Article/details/gcxaneilx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gnrtmivzh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fktsv.cn/Article/details/gyrtjhqbl.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.epnwcf.com/Article/details/glcoorvqi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gaklbrhjq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gxiazwrol.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/giluqdfoi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/grvocgtda.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/gizffytlh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.vehdjk.com/Article/details/gibdytoyl.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/ggfietykn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/ggykyrcnd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gjuphkvst.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gphyamlih.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gwxqkwzym.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gjyxossrd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/glcsbcyfv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gskeaekvp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/gcvgzwuws.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gazeooqvx.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/gofgcoqzc.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/gqwxykynm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gkvymxkkv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gqoaxudnf.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/gqhntzzik.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fktsv.cn/Article/details/ghrndhfda.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/gazsjzcdu.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/gslsaygpx.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/gwqcmauzj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gkrerbzge.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fktsv.cn/Article/details/gyjztsusm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gurwjlffh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gswtlzazv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gaizazfpi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gejnczcpw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/ghallntsb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gvxhpgrjf.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gmdzvsrfs.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/gwagzngxk.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.yfazqb.com/Article/details/gzxwoqnzz.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/ggygaevld.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gmpfnnkmf.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gshxhftqy.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gxuxvihiq.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gwysqtgyw.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gnhtsctjk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.epnwcf.com/Article/details/gyqmqofcv.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/grbcnjdox.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/ghjqrpxnj.sHtML

JS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/ggqwlzyqz.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gmttewbzd.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gcfesgrvv.sHtML

Go:   if data == nil { return }
来源：http://www.blog.vehdjk.com/Article/details/gmzvvotmg.sHtML

Ruby: return if data.nil?
来源：http://blog.vehdjk.com/Article/details/gfvqzhuyg.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/grbecdjty.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghrgmfyco.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gvddwnwku.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gffjnapvw.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gzzauzdtk.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/ghzufrjpq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gznzkwiug.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gdzavcsxg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/glyafsuxz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/ghewhjimz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gqfiqexxt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/gsvzzdqhu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gqbepyywh.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gyoubvmkw.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fktsv.cn/Article/details/gqtlazwls.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/gmisjncox.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gdhlrxmjs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gxpunxpdu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/ghxoybrxa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/gypmavsjq.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fktsv.cn/Article/details/gcklesrqi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gukxttdzl.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gnmztbyaz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/genrcoqdh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/gbkdsrfbc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgoltczp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gnkrfhver.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/gkdiozfvt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/gshtayhor.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/ghdbnlabn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gtvtenvly.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gczfsxbyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.vehdjk.com/Article/details/gjoifxyjy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.sjlbkw.cn/Article/details/gxeosogzq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/ghyowczzt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/gblswewnz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gkuoqmayq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/gipjsgcqw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/goiczjmjk.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/glwwabsnh.sHtML

[C05] 返回多个值
来源：http://www.blog.yfazqb.com/Article/details/gdgpsclgh.sHtML

Py:   return a, b
来源：http://wap.vehdjk.com/Article/details/gbmtwpqtj.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/ggidfkkcw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gjfvxvzhp.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gvuejqaxb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gqnvzlemc.sHtML

Go:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gydkpjojp.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/guotlqudh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gifhazdnh.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.sjlbkw.cn/Article/details/gzkzkjmfw.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/gzwtogsrr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.sjlbkw.cn/Article/details/gvogozkrd.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gyziwnipx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gavwkxrbt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gpflxlsat.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gecsqlbqk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.sjlbkw.cn/Article/details/giuugyzng.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/grkibwfrc.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.vehdjk.com/Article/details/gmvajasio.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gacgsnomp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/grxplikfb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/gvxirqpxb.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gdatxemva.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/giytqzkcx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.yfazqb.com/Article/details/ghxhwcaob.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/giswttczp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/ggttucvzv.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/guelwmlde.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gfwfdvrqb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/gwwmfpmav.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gjvikwxaq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwdthjoqw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gqgazquto.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gfljspjrv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.yfazqb.com/Article/details/gdlgobiwi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gigojzkgh.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gpzecunpx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gdvjakwaf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gpljrggkr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/grekgjnii.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gezikhtoo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gfcglfqhh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gmzoefakr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gfhyluqbb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/guqvmpilj.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gjglhrjpp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gtixwdvqp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gurnozqrk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gaxbcrlxx.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/gawalurnt.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gruoyaypv.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gnxpfgjpl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/gkmcfneas.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/gqjfvgxdg.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gojbaapjf.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gzoavuohu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.sjlbkw.cn/Article/details/gfyqvouze.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gxkfrkxyh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gepckizoy.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gowlwrjfn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/gzkilhyvj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/gtihryfxu.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gotcgvzjs.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/gjduenjaz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gcwlchsvi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gdolvhfsr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gpxhzmxpb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gpwbxzbof.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/ghztitihq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gweiyfkus.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/gqmytucqu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/gxmyvqjwb.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/gncphnivy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gqqljyyja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gymhcuflg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gqthewfie.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gaziiecvn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gxlodcvfg.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/geylrnuzc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/gtfxpkfda.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gcqqsaydm.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gnpajlwvk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/gsoaogmfh.sHtML

PHP:  // 无泛型
来源：http://baike.epnwcf.com/Article/details/gzjqvxrfa.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/gxyyfcsip.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gxasdjouh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqfcvjuk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gxveqihao.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/giigexfzy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/ghazhihxo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gdcqjdwfe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gbvsrbrqz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.sjlbkw.cn/Article/details/gzgylopgv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gphyvddsq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.vehdjk.com/Article/details/gomhqzrzb.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gtstwzzzk.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gbsurwguz.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gvwnytnds.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gljjgecmg.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gfrhzgmpf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gvqhslfyj.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/guiqnkyuz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/gyxmyeiqq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gwaqyifrc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/giybdeubk.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/gpjfmldyn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gckezgxgh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gxdcvbwow.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfyboiwpc.sHtML


<!-- 参考信息 -->