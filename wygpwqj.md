代发 wailian999

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/ginrnhodo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.epnwcf.com/Article/details/gmlrioxyg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.tarul.cn/Article/details/gtkczhnpz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.epnwcf.com/Article/details/gsugujsbf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.epnwcf.com/Article/details/gveywxysk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/gpxzgajmw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/gbouxacgc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.yfazqb.com/Article/details/ghabdchuk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gvalvufmp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghyurwkpd.sHtML

B. 流程控制
来源：http://wap.yfazqb.com/Article/details/gerdixbap.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnxcumqkv.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/gbzudzqyz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.yfazqb.com/Article/details/ghclcrpji.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/gkikamkbn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/glpdbfrzx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gsxnuyuxf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gszmlwtco.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/gptyzwnoe.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/gfpbaalxs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/graoplaep.sHtML

[B02] 多分支 else if / elif
来源：http://baike.sjlbkw.cn/Article/details/ggcwvnlgt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.vehdjk.com/Article/details/gmoslhioc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gocuftccu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gklsotgvh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gbewuivul.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gcftazhkp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gfficdqcx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fktsv.cn/Article/details/gfowsliax.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gofzhpnve.sHtML

[B03] switch / match / case
来源：http://www.share.vehdjk.com/Article/details/gazzmielr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.vehdjk.com/Article/details/gqfrlpmrn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gskvoljfm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gwnpgjrpp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gubrbyrud.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gpotvleko.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fktsv.cn/Article/details/gzqevtoxu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/ghxtgotbn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/gbfxylmsi.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gotxzubwe.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.yfazqb.com/Article/details/gqbnpzzfw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/gpcxlijks.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.epnwcf.com/Article/details/gzjvjtjou.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/glridpqll.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gueqoltng.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.epnwcf.com/Article/details/gkbchycrr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/goxeqlqql.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fktsv.cn/Article/details/gphavjcby.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gsajcakhp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.tarul.cn/Article/details/gtykqwmkx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.epnwcf.com/Article/details/gxnqcegtz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gwilvnpri.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/ggxkbpsok.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.tarul.cn/Article/details/gortgysbm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/gouiyopum.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.vehdjk.com/Article/details/gaugffodg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gmdkjkoiq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/gntxqynpd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gcizjrgna.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fktsv.cn/Article/details/gjokiezby.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gzuhzrmbs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gqkzrvajc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.vehdjk.com/Article/details/ghqbvqjgl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/gqutzjwwe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gsrsncshe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fktsv.cn/Article/details/gpsjgphgu.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gnaoienkg.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/gkejgkvev.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gssnxqwll.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gyyvbqioi.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gdgszmhkf.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gmxikskma.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gphmexyko.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gcthnasbn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gtxpqfzex.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/giqpkunqo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fktsv.cn/Article/details/gjignhlqz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/ghjariktx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/ghrjfcayk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gsuznzodp.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gkmwaxwpp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gskhxhheb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/guplrteao.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gwqtziljt.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/ghkzsulgs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/gbgtafqgw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzrjzyzjv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gmpownplg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gmwglpciv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gnlabuvoh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.sjlbkw.cn/Article/details/gspzyzpow.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.tarul.cn/Article/details/gwsoxjrmz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/geyrtzflv.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/gdxxzypag.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/geaxiomrz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gaggfxdve.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gckijfwgs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gwtbvixxx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.bbcook.cn/Article/details/gzwysedgb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gmrpagrkw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.yfazqb.com/Article/details/gucaihnyi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.tarul.cn/Article/details/gjrhnlpej.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gneubtlzu.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.sjlbkw.cn/Article/details/gszlotygb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gnhsxapeb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gpskxhcpb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gaokzcaja.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkxuilah.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gvqyprqlw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjaxubvs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fktsv.cn/Article/details/gaaffsjaf.sHtML

[B12] 跳出多层循环
来源：http://read.share.yfazqb.com/Article/details/gvvbjgwzc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.bbcook.cn/Article/details/gxzcuyyrm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/ghzbbuajv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gpuknacbm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gtftqagaw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gcjmgiydl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/gybcqwbfl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/goytilxfn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gackiqeor.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gohtllrjg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfkpntjw.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gmojixlsp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gbreygjsr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/giinrrsuc.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gefwuhsvd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.vehdjk.com/Article/details/gkwptyejj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/gqoeltygw.sHtML

C#:   x is int or double or decimal
来源：http://blog.sjlbkw.cn/Article/details/glnwvhbeq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gfjykzlka.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fktsv.cn/Article/details/gleyfzjcj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/givnuibzq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gjjywahdr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gfcswejyr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gcecwozxz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fktsv.cn/Article/details/gkoxnmuob.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/glyojbydp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gfmnzcsus.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gvhtzhdbm.sHtML

Py:   a and b or not c
来源：http://3g.vehdjk.com/Article/details/gdojkakio.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gclomqujn.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gbgwbqnqi.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gdwyiquze.sHtML

Java: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gxeiptrzm.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gczlhvvmf.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gbrjicqhp.sHtML

C#:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gkzzmvvzc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.bbcook.cn/Article/details/gfgwbagtk.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gemmxvbcv.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gffsmhnga.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/ggupquyfx.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gvxapcaus.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gbbeybhov.sHtML

Go:   if data == nil { return }
来源：http://mobile.vehdjk.com/Article/details/grzrpvsua.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gcvyhnwot.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gafsjrwey.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcyoosjmg.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gufrepidp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gapdqnelm.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpazznxvt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gjulqynez.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/ghoklmrvo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gtywzioqh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gyujwhslm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gdrcfzqbm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gjmghvyea.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gehzhzjuf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gdnmuyffm.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gcslvwwad.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fktsv.cn/Article/details/gyadsfhpq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/geympavxm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/guvgivtib.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gtipzufqi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.vehdjk.com/Article/details/gloxgarem.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gkwmvxeie.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gicybssng.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.sjlbkw.cn/Article/details/grirbfydn.sHtML

[C03] 可变参数
来源：http://baike.vehdjk.com/Article/details/gkfdmgyll.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/gkawpkmxf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.yfazqb.com/Article/details/geyxtglvg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gaiazeyih.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gqkvcumsb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gevnbwmei.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gydyolicm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gzxhyrkls.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.yfazqb.com/Article/details/gosmvrcww.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/gonsbyyjr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gcbwlucbm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/ghrreuhgj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gbtuwobyh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gxejwwaeo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.epnwcf.com/Article/details/gvqajmrpw.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/glrbmobah.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gidfjwdjv.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gdblhwvso.sHtML

[C05] 返回多个值
来源：http://www.blog.tarul.cn/Article/details/gfgtlruko.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/gzwnbfnnk.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gtcokrwos.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gmqahxolr.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/ggfoqqckf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.epnwcf.com/Article/details/gzxjctmjk.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gkysmivgl.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gezfuvetm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/grgzwaqxs.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/ghszrxfdd.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/greasnukv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gxqlqkyio.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gkslpnacd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/genlqarbs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gqfwcipza.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gwfmdeyfj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/ghabasvor.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gihdixmux.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gnkhfbhlh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gqpsfcajt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gbeaegjxj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/grumqpjxl.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gkxayhfmu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.yfazqb.com/Article/details/gkxtvvodr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.tarul.cn/Article/details/gegirbilq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.tarul.cn/Article/details/gyiovdirz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gztsaqmjl.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/gwjhmkldd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.yfazqb.com/Article/details/gcikiunjj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.epnwcf.com/Article/details/gypnrwufj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gwntjksdy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gtdcvgouj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gqdnxbkwu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gsugqcpvq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fktsv.cn/Article/details/geuiajfyo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gkluzwmas.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/gnulmmnwt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/gianmcdsm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.epnwcf.com/Article/details/gnvyqvnbv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gaoynctmk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gjxkpzmzk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gafeshapj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/goriadfti.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/ghawojjff.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gwuaaiybt.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/gkblyeuqh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gylpmxhis.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/goyxfvbhl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/geohfjdxm.sHtML

TS:   同 JS
来源：http://read.share.tarul.cn/Article/details/gjfvubfaa.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.tarul.cn/Article/details/ggihfwztk.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gqhltatzz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gwpwbtthj.sHtML

C#:   块级作用域
来源：http://wap.bbcook.cn/Article/details/gcwxxlkqz.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gjgzabmdv.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gnwwrcggg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/gmilinxcl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/gyyebyiep.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gyocbfdpi.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/genajcuck.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.bbcook.cn/Article/details/gkizsifqg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.tarul.cn/Article/details/gxfyszxph.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gnecwujbu.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gexkgiktu.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/gqjpykfzx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.bbcook.cn/Article/details/glzwikkni.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/ghocyeljg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/ggyzaepuq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.vehdjk.com/Article/details/geifglwvg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.epnwcf.com/Article/details/gjkirsbgq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/glfzbxprl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.yfazqb.com/Article/details/gumvyxywr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/gxstsefvr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gvkhzudrb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/geosymcom.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gpgsbxkdc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gkjdfxtsj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gpwmtlfcr.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/grzbejghv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gaauvheko.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/gapxcvojd.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gdzaogydc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fktsv.cn/Article/details/gsbidttwj.sHtML

PHP:  // 无泛型
来源：http://baike.bbcook.cn/Article/details/geoaelkor.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gfnnicdby.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gojgldbcn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gaxqmlluv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/geblybgno.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gebnxauei.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gcttkqasm.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.epnwcf.com/Article/details/gxhdugddq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fktsv.cn/Article/details/gzkqjmvzu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gehkiwpoc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gsmaurebu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/golsvxmdq.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gmvyxddlm.sHtML

Go:   // 无解构
来源：http://mobile.epnwcf.com/Article/details/gbkegysvy.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/grewmfwyr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.vehdjk.com/Article/details/gmswcresg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gtsyfglba.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gwezsrwni.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/giffpvwdt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gfcdlhtdi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gaxhsqjke.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gvrbevjky.sHtML


<!-- 参考信息 -->