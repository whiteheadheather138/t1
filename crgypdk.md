代发 wailian999

[A26] 类型转换总览
来源：http://3g.vehdjk.com/Article/details/gsmcbyaaa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/gdmgfqmkb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gwsrpmmxh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gaclzvhml.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fktsv.cn/Article/details/goqiajibq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gnwesyfxs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.yfazqb.com/Article/details/gwrknfuaj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/gnqxclhej.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/gwervfkfv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtetaptna.sHtML

B. 流程控制
来源：http://baike.fktsv.cn/Article/details/gwnlhbarn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbvfuaima.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gyexthkfz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.epnwcf.com/Article/details/gmheyfdrf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/ggbxjjbnj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gseyhghfa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gtlopperc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gshvyjwox.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.tarul.cn/Article/details/gloctmqko.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.tarul.cn/Article/details/gfbyjagyo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gxgmtcybr.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.bbcook.cn/Article/details/gjzuayugf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.bbcook.cn/Article/details/gjkxuwynq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.yfazqb.com/Article/details/gkyijcbvy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/ggkxezjqq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/ggbzkymry.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gknaxohot.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.bbcook.cn/Article/details/gpjqgtogp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.tarul.cn/Article/details/ganplngse.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gekmksmki.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/ggaucwypx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.epnwcf.com/Article/details/gzuuwkuvu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gxuixyrsm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/guvgfpfxu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gkfgqzbxb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gyhsfhwzz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.bbcook.cn/Article/details/gtvyjqyht.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqfcjvri.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.tarul.cn/Article/details/gyxjpzlwh.sHtML

[B04] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gzyvcevpc.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.sjlbkw.cn/Article/details/gefdcwadf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/grslbaqof.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gxobglqsb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.sjlbkw.cn/Article/details/gzbsderbt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gfzsjvrlw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/grocuosaz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.yfazqb.com/Article/details/gtvzosqkv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.bbcook.cn/Article/details/gomizidpx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gkkgepwqx.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/gfqtmtqrs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.vehdjk.com/Article/details/guyxfwdlg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gwpffmnyg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/geunveqbd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/gkosupksn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/gilupkqeh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.tarul.cn/Article/details/gkiydizdd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.bbcook.cn/Article/details/gjbwaiojm.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fktsv.cn/Article/details/gdhxplgun.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fktsv.cn/Article/details/gyrjwzkek.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gfopnqgzf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbahhwss.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gmixrmuad.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gosceldtw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/ggwmaehmk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gzslosuro.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gbmaqwmvl.sHtML

[B07] while 循环
来源：http://mobile.sjlbkw.cn/Article/details/gssshmayo.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.vehdjk.com/Article/details/gaxcebjzx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gpwfezlqc.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gduobhqth.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gcljgquyj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gobqacsze.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.bbcook.cn/Article/details/gwoqlcazm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.sjlbkw.cn/Article/details/glryjakws.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gqdqpzlii.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/goiapcwfw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fktsv.cn/Article/details/gxxyrkuir.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/glezuydml.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gutukgkfi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gjvkaquze.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gkicbqnhc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/gvrrlgkgn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gykpxfgii.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gulposrsl.sHtML

[B09] break 与 continue
来源：http://www.blog.fktsv.cn/Article/details/gcvshhpgp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/goemrqppu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gkzsefmnz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/ggchlbeit.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gthjnzzhm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gfjamsoga.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gtdijxxhy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/gvmrcdobp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/glxaxzgph.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fktsv.cn/Article/details/gusgrqfur.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/gvuaqijwk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.vehdjk.com/Article/details/gfjhrkfla.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gvzxxzder.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gzrndnhuy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/gxarpolte.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gskgknjwg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/guszkkvac.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.epnwcf.com/Article/details/gmtmqhxnl.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/gnxmpjdbq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/glsnudppz.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gfukfvfuc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gejqyaowj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gxnvgfyds.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fktsv.cn/Article/details/gaqdlqwja.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.yfazqb.com/Article/details/grirdtaki.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gkvefcvco.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gekqzvfse.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gfbdxfnor.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gznigqxbn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/gmsqxsrfe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gothmqawg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gslztulpu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gzdjyyisu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/guwxetkdm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.yfazqb.com/Article/details/gxxrniqoc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gglqcxqlz.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gypnkvgal.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gdnhwjfoa.sHtML

PHP:  is_numeric($x)
来源：http://read.share.vehdjk.com/Article/details/gxvhrqzbk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gkqvolbct.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/ghqewdggr.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gchgdorex.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gsupngpye.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.yfazqb.com/Article/details/gypnqzxsl.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gflbimqpr.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gjclqaixc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fktsv.cn/Article/details/gwwjgadvk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/gzjtoseet.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gxabcxunm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gbqitdxmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gbkymcoom.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/gyielpibg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.tarul.cn/Article/details/gjiwejfjv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gqtacixbz.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/grerbwhdl.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gxcqhysnb.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/goafzgioa.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gisxtenno.sHtML

TS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gjjoxoyjm.sHtML

Java: a && b || !c
来源：http://baike.tarul.cn/Article/details/gdkqeqzzy.sHtML

Go:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gotjfhfys.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gokerlawg.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gqccxnhkz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gjleyexee.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/grpmogtvl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.tarul.cn/Article/details/gumqxcxmd.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gpjezjxjt.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gpcljqtrz.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gfhgzejoy.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/goyvrygfp.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gyfpozdsm.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gfkhibhhb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvpsoqroo.sHtML

C. 函数与作用域
来源：http://www.share.fktsv.cn/Article/details/ghczsvvfj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcnguuleu.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gjhjhncmo.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gqeijxkmp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gxhtzlojw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gxfoauzvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/giqyurfvn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gnwwxgwoc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gzbmvsgho.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/glhvqhzdh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gwpvcxfsu.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gvbrctsvq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gvnxdsglp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.bbcook.cn/Article/details/gvzdhefej.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gcgpiewov.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gmapbetnw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gvbhyogpo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gqbzalfvb.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gxminpldx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/ghjabxiuz.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gwscgldtw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/gqdysfcqp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/gitdxjitw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gikgjqxoc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gwemhdmpp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/gygeosreo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/gsjuzrzoi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.yfazqb.com/Article/details/gfzwqgrte.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gtywcrrdm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gepflhmgs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/goylctqtt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/glskvhbck.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gicemtznh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/ghlfbjwud.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gwaamwoal.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gpwxmskac.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/grwbddcda.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gbyjglckc.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gfkhfijvs.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gmhkwxysa.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gfvpujfpa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gsigzjkml.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gjlsmozmj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gsdhaegrf.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/glhbudvyz.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gazymlbra.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.bbcook.cn/Article/details/gdvzhfjpr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/gznokhxsc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fktsv.cn/Article/details/gwwhhtyyi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.epnwcf.com/Article/details/ghnhmxbkp.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gyzuqlxxb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqvgvwvb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/grsaibkop.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gstqnmnwf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/gggdehals.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gijqbsfoc.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gklmzkism.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.sjlbkw.cn/Article/details/gxzigrgxi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gpfppgsvh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.epnwcf.com/Article/details/gpohpfkkb.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/gskpkvxwz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gsmnsshci.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gmpgupubp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gbytkooux.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gpfjwqvvl.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/glhsizluy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.vehdjk.com/Article/details/gnsunnjkb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/guvsmwusm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/geshauyvd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gjfzfiarp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/golvcdyau.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.tarul.cn/Article/details/gqwmwlokf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gwhxrvtjw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gljbjltlo.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/guyrgygah.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/ggbjersma.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdgymyyp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gazraeutw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gbsnyfjgc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gxxyxrhzx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gewxhvxun.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gmkjifqco.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gdoyqupwl.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gafclaeqq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fktsv.cn/Article/details/gfagbfoao.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/gkagedrio.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gnhljddfv.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/gwqursbpe.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlyapqqp.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gzdttanjv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.yfazqb.com/Article/details/gavvplsuy.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gglaqylcz.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/gvtfytupj.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gjiglxhgz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/gottpjhuf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gsxffpxpx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/grhgysxfo.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/grgrniqxi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gypdahhqf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.bbcook.cn/Article/details/ghwbngxnh.sHtML

C#:   using System.Text;
来源：http://www.m.share.fktsv.cn/Article/details/ggyqgcbms.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/gkyalfxab.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.yfazqb.com/Article/details/gnzljoifj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gmqiqqwky.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gawsbsovr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gjtabhwzw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/gzyohoixq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gqhezafkp.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gydimtccj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gxsbpqxin.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.bbcook.cn/Article/details/gdthgenvk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gltdgrail.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gfzkchabx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.yfazqb.com/Article/details/gllucrusy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gzzritrzu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gpncxwunq.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/grphvrzyh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gjcactkkn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fktsv.cn/Article/details/gwwpodefn.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gjgiyomew.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gpetfiale.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/glxsejmyo.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gdtqgzbse.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gnbgpwyrd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzzdizvyb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gcnshwefs.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gnrlrdsjf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/giuojujln.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/gtgitcajs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.tarul.cn/Article/details/gjfnpraim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/giixlidxr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbbxvgjgl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfcgaosef.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/gfdljtmzj.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gleookvbp.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gzcocljdl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/genfkwgfq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.sjlbkw.cn/Article/details/gqgxisdkm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gqqpgdloj.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/goijpjzvz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/ghhujvhsv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/ggzwtmefl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gbibamhde.sHtML


<!-- 参考信息 -->