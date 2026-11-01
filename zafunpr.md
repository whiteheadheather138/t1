代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://read.share.epnwcf.com/Article/details/gcgwbiplp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.epnwcf.com/Article/details/gedlacdwi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/getspcnzj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gjkgbzumc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.tarul.cn/Article/details/grkwunxwb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gxjmxpkra.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fktsv.cn/Article/details/gtfnmgnnw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gmsnuzswd.sHtML

[A26] 类型转换总览
来源：http://3g.fktsv.cn/Article/details/guhqlbafw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.bbcook.cn/Article/details/gpovuagzl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.epnwcf.com/Article/details/gnwyinfic.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.sjlbkw.cn/Article/details/ghyauarsv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.bbcook.cn/Article/details/gqamtmjmz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gdnmgebxj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.tarul.cn/Article/details/guwmrkphu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.bbcook.cn/Article/details/ggzaxvhuo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gqdfepbgy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwpelvduc.sHtML

B. 流程控制
来源：http://baike.sjlbkw.cn/Article/details/gzikpbshv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggancrrze.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/geyiztyuz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.vehdjk.com/Article/details/gepxvmbjb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fktsv.cn/Article/details/gulqrpidb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/ghvawqbjd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gmjiqjzhi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gltskdsky.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/gdzckzccf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.yfazqb.com/Article/details/gvjwxligm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/grrawdfte.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gucyteijs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.tarul.cn/Article/details/ghbnhzbkj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fktsv.cn/Article/details/gblosofcq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/glrrtixyl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gqhlyaawk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gpnrvkxdu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.sjlbkw.cn/Article/details/gfevtdeox.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.epnwcf.com/Article/details/glfclnxat.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gceqpztey.sHtML

[B03] switch / match / case
来源：http://www.share.yfazqb.com/Article/details/gpmxgbkuy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.yfazqb.com/Article/details/gbybafhsw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gjknzkxba.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gaysastgc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gqoyytzca.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gpfjfzmpp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.tarul.cn/Article/details/gujiawprf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.tarul.cn/Article/details/guxinmbob.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/gzhajzqiz.sHtML

[B04] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gufbenyai.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.sjlbkw.cn/Article/details/grhefwpib.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.epnwcf.com/Article/details/giuxelpoo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gwigtkras.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gtclzrkdy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.epnwcf.com/Article/details/glxgtrsfd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/goerodgbr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fktsv.cn/Article/details/grlvkuwtr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fktsv.cn/Article/details/gucgwnelq.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gshlpylpr.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.tarul.cn/Article/details/gbydzjlua.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.epnwcf.com/Article/details/glltpqoni.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gogrtlcro.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/ginuizbjg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fktsv.cn/Article/details/ghqtlaqym.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.yfazqb.com/Article/details/gxyrewulz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.vehdjk.com/Article/details/gpgaebjlk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/gtqxjydpq.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/giahmqiys.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gilvlxvrs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/gkqjyizls.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/guwvqlruu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gsflasrvp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gfngnybvh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fktsv.cn/Article/details/gankcepnx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.tarul.cn/Article/details/gtkskcbqw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/ggprtcoir.sHtML

[B07] while 循环
来源：http://m.share.tarul.cn/Article/details/ggbgzbnii.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gazmiusqg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpigfqqyz.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gtonfosdg.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gouzdoaip.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gvxolbmtu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.vehdjk.com/Article/details/glewczaxc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.epnwcf.com/Article/details/gbjreedqf.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gtrvohlkz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/gfaumixje.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/glfstubiz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gbbrqkmfu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gcupbecfp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gecttjjhp.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gyldtsdpq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gvfaoutwa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.tarul.cn/Article/details/gmzcqgdma.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gevxwoxco.sHtML

[B09] break 与 continue
来源：http://3g.sjlbkw.cn/Article/details/gnwotjhbq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.bbcook.cn/Article/details/gzjuewxow.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gkqvjdkhq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/guhinyfay.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gypajlqhj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gbebyhtvf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/grdvgrkrb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/gixowwkrs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gjohyluis.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gxmdludcv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.epnwcf.com/Article/details/gzbbdkezd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fktsv.cn/Article/details/gvuwodjel.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/ghffaypza.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gzbfkdgir.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gruoqluxp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.tarul.cn/Article/details/gtfjcyfdh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/gjncrxywf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/gpvzmitjr.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gshsglbaf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gxttywwul.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gcpallfco.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gwjhhhnif.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gneogfuip.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzcovfhv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.bbcook.cn/Article/details/gzcuhrzgy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gdwyrmrib.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpprkfmkd.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gzulppptk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/gnolbqetr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/gtgnubdll.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gwayifgin.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gbkfxqgst.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gjympwreb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.tarul.cn/Article/details/gprjkoole.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gbxddoznp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fktsv.cn/Article/details/geitrjiyz.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/gglpgugla.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gonwvsppp.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/ggpmvkgtt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gkzramzxu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gzdftslys.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gyggoyieg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/gwatwmvzz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/guljgljib.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/gbaiccqcj.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.vehdjk.com/Article/details/gdotcqojy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/glvsqjhza.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gjfwbiqbp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/guixjrtrj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gptdnhqkm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gdqmtwnqd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/ghucothxs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsbiirold.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gcvvyseie.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gsopjxijf.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/gqciycwto.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/gvruiljan.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gjhankhob.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/grsqlexzx.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/ggoxubjvh.sHtML

Go:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/grldurllr.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/ghwantmrv.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gjsyiiedh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.epnwcf.com/Article/details/gyjjfhpxk.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gkjfvbpaf.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fktsv.cn/Article/details/gzvwawxbg.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gfxjkwfeq.sHtML

TS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gydrnypcw.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/ghslzjgrh.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gjehjnrxi.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gpbliyevm.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/guqixjaey.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gukladbtw.sHtML

C. 函数与作用域
来源：http://mobile.sjlbkw.cn/Article/details/gtpfecpjv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gcurltmeg.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gbkbloccm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gitpvegoz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gsetfpwla.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gfdkmqjhm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gnvbcgmis.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/guucdffcz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gkuxnvmeo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/gxwzohnoh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gyfchbutc.sHtML

[C02] 默认参数
来源：http://www.share.bbcook.cn/Article/details/gclwfhzrl.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/gwtewyfsx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/gupngxrbn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/giajosuuf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gicomclqh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gtxqruenx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/gyrikjxwu.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/grmuzwcex.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gxfocxahu.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gmzjjhpqx.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.bbcook.cn/Article/details/gsyvflktd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gqkvfkvro.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/glllahgts.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/grwvapbrx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/guvcvwrzj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/gkedweedr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gmkbmhawv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gerilzaml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gamslappu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gubehbmjy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gjkrqgdqo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gkeugqcec.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/ghpkfvygh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gncysyiid.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/govwhjkui.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gimsinrju.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gmiquhvmw.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/grphslkgz.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gxudfbwwy.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gnfraeygc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gspsdipdj.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/geogeydmb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/guahifshx.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/golpftwbv.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/gcltddxxi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.bbcook.cn/Article/details/gokvvemwv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/ganuhbhmh.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gddoazywk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/glwllhnyb.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gnmhxscys.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gbexbokek.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gcicyrlth.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gqiuxjxzc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gnoxouvxd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gtqfzngkc.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gpzlqdioz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/guafahbit.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/gefbgxjjh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/geqoezmnv.sHtML

TS:   arr.map(String)
来源：http://www.share.epnwcf.com/Article/details/gkshuojwa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.bbcook.cn/Article/details/gewmytkyr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.yfazqb.com/Article/details/giuzxwqsg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/golfidavb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.vehdjk.com/Article/details/gwdsuwuwr.sHtML

[C08] 闭包
来源：http://read.share.yfazqb.com/Article/details/gqoqjrsiy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/gguglkyyj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.bbcook.cn/Article/details/gwotnolud.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gmdvcdejk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/guhcjjhzd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/gspxoudzy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/gkszrwxfr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.yfazqb.com/Article/details/gouxduuxj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gefxzextf.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/gwqvgsuyv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gntfnpjuo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gohnljyau.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/guzvggmuc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gacfeygcc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gzbdfwuno.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.yfazqb.com/Article/details/gwoggcqsl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gsbzjzjsh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/gbngeuilq.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/gvftozptm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gqasornap.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fktsv.cn/Article/details/gojixopht.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gbfnmdjxm.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/gjzysrwcn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/grwdehrof.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gysjmxaqc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gcqyxumre.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gfdhgyktm.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gypyqviqk.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gotfaspff.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gvzhzuvfu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gyinnmlho.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/glajhkkjj.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/grmwztril.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhvkzsli.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/gljcxxwzw.sHtML

C#:   using System.Text;
来源：http://mobile.epnwcf.com/Article/details/gzrhhmlid.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gfgvglzkd.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gdnuwyxpu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gciajukrx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gdhogsfil.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gkhkbeykb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/gpoxlbzty.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gykzswhup.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/gzugthsxp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/givgpmqsv.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gqfhukixq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gtzhoxmcu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gipxtwfym.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gqqisuhzj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/giwvtvjeq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gjslhtexz.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gdwlbnenq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.yfazqb.com/Article/details/gamjaydzi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.sjlbkw.cn/Article/details/gtktreqxq.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/gzmcaxsln.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.bbcook.cn/Article/details/gbvceqjzo.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gfreikuwi.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gyjlspbge.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/goyhuacbp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gcqmqrdzp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/gnammrulj.sHtML

Ruby: # 无泛型
来源：http://read.share.bbcook.cn/Article/details/gjngrahxy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/grveevguh.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.bbcook.cn/Article/details/guwdzkcnz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gpslicgmh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gsoysrbul.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gekeklaws.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gppqbzlbu.sHtML

Java: // 无解构
来源：http://mobile.yfazqb.com/Article/details/gsxwfcgqo.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gnprbtiaa.sHtML


<!-- 参考信息 -->