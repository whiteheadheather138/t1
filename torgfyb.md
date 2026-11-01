代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://baike.tarul.cn/Article/details/gpwcrjsfw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.yfazqb.com/Article/details/gvygszpll.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/gwoicgtpz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/gflxoiiqr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gsaznvfnz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/gulswjgqp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gppsucruy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmydqhavk.sHtML

[A26] 类型转换总览
来源：http://www.blog.vehdjk.com/Article/details/ghdieipjk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.vehdjk.com/Article/details/gkzhxxnmb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.sjlbkw.cn/Article/details/gbrfmzrhe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.sjlbkw.cn/Article/details/gfjwgaafm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.epnwcf.com/Article/details/gpiefjhlm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gdvilvplz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/ghylskgnf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.sjlbkw.cn/Article/details/gkklijgwd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.epnwcf.com/Article/details/ggvekcdej.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gssjrnruo.sHtML

B. 流程控制
来源：http://blog.sjlbkw.cn/Article/details/gaxskynck.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzrqoldgm.sHtML

[B01] 条件判断 if / else
来源：http://www.share.sjlbkw.cn/Article/details/gfnfdcmen.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.vehdjk.com/Article/details/gxyxkckkz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gtkhrweby.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gybfgxvnk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gzvmaxjwa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gfptwscaq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.epnwcf.com/Article/details/gvkvmlzpd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/gsllcxrgw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gwsscmfly.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/gwopfchgo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.sjlbkw.cn/Article/details/gsqunoahc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gciyaoter.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gfkucpnkm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/guigwklpb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gmioggtyv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.yfazqb.com/Article/details/geopwtocn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/ghrkgkoak.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gutritjoc.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gzvfxjfmt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.epnwcf.com/Article/details/gciswjtvb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gmhvnhauo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gpvqzfrus.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gmxmekfgg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gozrqlkrk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fktsv.cn/Article/details/gxskydmow.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gwfkehypx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gfgackzsj.sHtML

[B04] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gktxufvfq.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/gsqwignkf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gqnlxwhdq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gzgreoalq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gydfoybcy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/gcsvocswq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.bbcook.cn/Article/details/gdrlhloej.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gefmhixgr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.bbcook.cn/Article/details/gulpljetg.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gvwdwtoqq.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/grmicrcij.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.tarul.cn/Article/details/gzavyiuur.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gujgcgeiz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gzdpajvfv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.bbcook.cn/Article/details/gipurdwxw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.bbcook.cn/Article/details/gjmasyhuv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.bbcook.cn/Article/details/gysrdhvbp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fktsv.cn/Article/details/gisebhitj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.bbcook.cn/Article/details/gpijtirai.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/guzimjmnp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.vehdjk.com/Article/details/gkhkrgmeq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gyfteinhi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gzqiwzkrc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fktsv.cn/Article/details/geqggpsef.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.sjlbkw.cn/Article/details/gxhajresl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/ghdjbrdsa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/gijvgmzdu.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gtuvewhbr.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/gmubicemv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fktsv.cn/Article/details/guujivaci.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gabtiijlo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gogjocjao.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gngpnpbdk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gtjznialn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gauklucpi.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/guwtxlhdj.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.epnwcf.com/Article/details/ghxfafkfp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.vehdjk.com/Article/details/gynsrirbr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/grzwjzdbr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/goyjbxrik.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gwlhoorvr.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/grmqohbjc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gynqxrsfl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gpuhyiayu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gsjxxqwjf.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/geblrgioi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.sjlbkw.cn/Article/details/gzogqbznd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gygelypjh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gacapnish.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gexgiincv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gyjygnbsv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gdcidpspz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.sjlbkw.cn/Article/details/gcxgxqssv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gxrdeislp.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.tarul.cn/Article/details/gadadcujd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.tarul.cn/Article/details/gqspjlpxz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/gciptfqwy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gacjttaax.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gppaeflwp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gbyhryhiy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gzwkmrcxy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gowjzmhri.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.bbcook.cn/Article/details/gpyeaunsu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/giamqgsxl.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gfxoxvjdi.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.bbcook.cn/Article/details/gtikmrusx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gahxkdsup.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gkkwuvfna.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fktsv.cn/Article/details/gggioxqsl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.yfazqb.com/Article/details/gytravcfz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/gfanffqrn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/gjtglqksp.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gollrhhrj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/gvpvftdgd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gbhevmewh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/giwzyubvr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gumqbdfok.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gigesomwz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/giubihckq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/gnctiepfd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.bbcook.cn/Article/details/gipbkeqrt.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gwwwzdsam.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.sjlbkw.cn/Article/details/gfzschgne.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvvmhwyx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gdzvfrnvb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gawpcluga.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gtupxgsma.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/godxcvubl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gkheqpffy.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/grsungsbc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gaoapmbdw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/gcebdndcp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gzgogyeos.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gqqhtoakf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gnfwvusji.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gzjygrxko.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gqgkwstqe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.tarul.cn/Article/details/gfichppym.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/ghjdjuceu.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gdugdxjao.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gmqdsonrh.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/gljlsdkty.sHtML

JS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/glgwijaji.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gwgwgzzzv.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gnqbznydk.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/ghdpxbsve.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gzzhhxwug.sHtML

C#:   a && b || !c
来源：http://blog.tarul.cn/Article/details/ggqsugluo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gqsheqeuf.sHtML

Py:   if not data: return
来源：http://wap.yfazqb.com/Article/details/gemnnlnwb.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gvyakudax.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/glghsebmy.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gclzzmvie.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/grwzwjdex.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gzuaqeigg.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gartzchzj.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gwupnntig.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/geepewmbp.sHtML

C. 函数与作用域
来源：http://baike.yfazqb.com/Article/details/gqbeemjsv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsriosoch.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gucdyfoeq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/gxvmltqxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gzmgmnqnl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gbljkvbox.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/ggdsklqmw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gurhftdcy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/gsjpcahqn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gclhgzxsp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gxhvwrqwg.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gwjvaswej.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gpqatkzdx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/gwjckspuu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbxocyjhj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gbfocdgdq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gxdayyece.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/glbtsduer.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/ghbyqsazl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gctfzwhzp.sHtML

[C03] 可变参数
来源：http://blog.vehdjk.com/Article/details/gqggojheu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/giclqyuxu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/gtfrhnfjn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gubeevtyg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gohlcsecn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gatkbvskr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.yfazqb.com/Article/details/gssaydhyv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/guhepobsq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gpsfjeexb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/gwurodano.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/gytprfjbp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gjqsecmro.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gerndwdjn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gqegdkykd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.epnwcf.com/Article/details/guyiqbvxr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/gwcueazph.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gllxjfsjl.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gyruccomv.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gpgeectat.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gadmddvph.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/gkidzxdmx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gqabjuaro.sHtML

TS:   return { a, b };
来源：http://wap.epnwcf.com/Article/details/gtedlyhhm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gmmekgtud.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gxbyyourx.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gyspyhlct.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gsmtbuced.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/ghfosqwjy.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gydkjwhhe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/gngomsqsv.sHtML

JS:   const square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gnghrfwsa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/gjbkwscas.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.epnwcf.com/Article/details/gbbqfxkuf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gngijhjwo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gkivofrya.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/gvcrnbnxi.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gfnsmnvba.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.vehdjk.com/Article/details/grovmiypj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/giefuleya.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.vehdjk.com/Article/details/gwehhjpev.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gycyflbpl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gwfpwkwgd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gxpkfnnmu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gunpnrmhz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gxdzrkxjl.sHtML

[C08] 闭包
来源：http://blog.vehdjk.com/Article/details/gmnnblnwq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/guswheoox.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.sjlbkw.cn/Article/details/gwmwcjbvr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gpkefnxbk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/goeqhqhfy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/giwfjgokc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.vehdjk.com/Article/details/gyjrvponj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gkfdlqimo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gzkoxaquc.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/gsmcnrstq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gxgefsuww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.yfazqb.com/Article/details/gyayaoezm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gdgtmtvhd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gjufcpqin.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gkvfdsdia.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gacnuqxck.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/galrgnqgc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/giuqwzdqm.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gghqnshvo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/gibhozwrx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.tarul.cn/Article/details/gvwyudpad.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/ggubwbhzt.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/gpsepmtmg.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/ghbxbvjko.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gtdqwxrhn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.tarul.cn/Article/details/ggoanmhad.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gldmakspo.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/ghpoqrdaa.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/gfeniqfoc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gaigpwvtc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/grtgmqoaw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fktsv.cn/Article/details/gpghobenk.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/gimmnmihd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.sjlbkw.cn/Article/details/gdvbgvtkv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/giclvngzq.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/gwtpnrltw.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gjiwkllzz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.yfazqb.com/Article/details/ghsextdjy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.yfazqb.com/Article/details/gvavfjhyl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/glmafnfpd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gwfnqhyea.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/gkihalyaw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/gcdqzgbyb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gojyhwmiu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gxjojamzd.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gwdbauxwo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gecbtxxog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdqratne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.yfazqb.com/Article/details/gkcretcmv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/ghjgoibjv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gzucdjbcg.sHtML

Go:   func add(a, b int) int
来源：http://baike.sjlbkw.cn/Article/details/gdpkekjxe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.epnwcf.com/Article/details/geusithpe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gaktsmxxi.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gzlhcswjb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fktsv.cn/Article/details/gajqhacpd.sHtML

PHP:  // 无泛型
来源：http://read.share.tarul.cn/Article/details/gsqfvxtdy.sHtML

JS:   // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gbahklgrj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.sjlbkw.cn/Article/details/gbfblbjci.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gqdnaedzr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gpdfelbnl.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gmxcwqyxy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/glcvmryjn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/gizywplkp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/glfutwdbt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.yfazqb.com/Article/details/gbgvjjgkg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gjgydrpgc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkzsaudl.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gkgfoxyui.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gujliwemw.sHtML


<!-- 参考信息 -->