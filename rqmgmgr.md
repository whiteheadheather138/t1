代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gecufklgy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/gqhidhkcq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.bbcook.cn/Article/details/gysqjeobi.sHtML

[A25] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gxgfmmmey.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.sjlbkw.cn/Article/details/gvvhvppuq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/glqfminvf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gdhdvqjbv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gvbnvqyac.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.epnwcf.com/Article/details/gyrdcsqch.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gudrscdyv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/gvzdzoamc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gxirbggsh.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gbfokifrs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gyvtqxqkc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.vehdjk.com/Article/details/gbuknzvnc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fktsv.cn/Article/details/gicklzmtp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fktsv.cn/Article/details/ggiapgnkc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/gtmxybjyw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gjpdgcuaq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gkxcrkzqm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/grwcsyoiu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfuoeqgxu.sHtML

B. 流程控制
来源：http://www.blog.epnwcf.com/Article/details/grazhxcyg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmpxluwyg.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/gauhpecti.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.epnwcf.com/Article/details/gvrfpxuup.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gnmvoexjb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gtvvwewgb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/ghleuprnq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gpbfhobwj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/gerrotufg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.yfazqb.com/Article/details/gcuzesguo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gvrifxjni.sHtML

[B02] 多分支 else if / elif
来源：http://blog.bbcook.cn/Article/details/gptfrxglz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.epnwcf.com/Article/details/guygrtzrz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.vehdjk.com/Article/details/glbvzhmdd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gzwiefblc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gobszfwpg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gqmenlbtk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fktsv.cn/Article/details/gozrznwdf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/glluhkwnr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/giggosmtu.sHtML

[B03] switch / match / case
来源：http://www.m.share.fktsv.cn/Article/details/gyvhhtsih.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.yfazqb.com/Article/details/ggvqsdmyj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/glrvbslpz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gadydsnal.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/grlpqeovl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gttfqpdsg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gndwbkovy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gbwzmixny.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/gsmacfujv.sHtML

[B04] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gjswrxrjs.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.tarul.cn/Article/details/gtstfmnoe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmlmkplz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gemuzucgl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gzjphoxqq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.vehdjk.com/Article/details/gnvclvvde.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.yfazqb.com/Article/details/gjqzwdnjg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdakxpsln.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/gdmqgtfir.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gjvapzvcp.sHtML

Py:   for item in arr: print(item)
来源：http://baike.vehdjk.com/Article/details/gsfwotjpf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.epnwcf.com/Article/details/givpwbaeu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gilobzmax.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gerrbbwfk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gzcdanarp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/gxzxbgiqd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.sjlbkw.cn/Article/details/gyzwlzqgc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gidifvmpk.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gbkwkkxcm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gitetumjv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gmcxzleoi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gduorrgaz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gthvaoctm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.vehdjk.com/Article/details/gkvceuflk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gfukbzfby.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gcfoqvove.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/gcbnkzyzc.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/gvdqupoos.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.epnwcf.com/Article/details/guxitgxgr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.tarul.cn/Article/details/gaovrrums.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gdxzcdlvz.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gwuulaqrk.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gunsgvitd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.vehdjk.com/Article/details/gqpoqmmym.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gilsbbabu.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gpddpnaas.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/ggfiwuyum.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fktsv.cn/Article/details/gygjyzhyz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gztzlsosy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gavzlarsx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gncbrmpxc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gvbwwpcil.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gslqedtda.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/gviemmbze.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gnvydomeh.sHtML

[B09] break 与 continue
来源：http://baike.fktsv.cn/Article/details/gtuvlugmc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/goppowlcj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gfsczfeuc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gchsuvkyb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gxdqfzqnr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gsfbpsrsc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gxoostduj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.epnwcf.com/Article/details/gjtnqwile.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/glyptzcxp.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.vehdjk.com/Article/details/ghzgwcnqf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.epnwcf.com/Article/details/gjhbhfzti.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gjyxbxfpt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gcuqxfdmp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gusritgdq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.tarul.cn/Article/details/gnjzvvqbl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/gvkghveej.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gtdgjbawb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/gttesjctt.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gpdqzlceb.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/grwkyeujg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gyakydeoz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gmlfggbes.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gjmdjmmzx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gcamahref.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/grcadaceh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.vehdjk.com/Article/details/gdopwpasg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gujykjufu.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/gcotbujvd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.sjlbkw.cn/Article/details/gnineoeto.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gmttbpoiw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gbuqjcbhn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/ggkuflcue.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gozoulxke.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gjkegzepz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.tarul.cn/Article/details/gpkuhrjeb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/glcklbvbk.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gpnjergtv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fktsv.cn/Article/details/gdlksrdlr.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gokuktmay.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/ggdlnfbgk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gnwsxpxes.sHtML

Java: x instanceof Number
来源：http://read.share.vehdjk.com/Article/details/gxganbqfw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/ggpdzgeru.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.epnwcf.com/Article/details/ggpbjakkb.sHtML

C#:   x is int or double or decimal
来源：http://read.share.yfazqb.com/Article/details/gojqcvnmy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/gmpqupvec.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.yfazqb.com/Article/details/glncayqif.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.tarul.cn/Article/details/gbeobdsog.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gizievasf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gqncytont.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/gbytifhzs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gkqlnrmzv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gpovdfaem.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/glbxllkms.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gwlecmpfl.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/ggupffvkd.sHtML

PHP:  $a && $b || !$c
来源：http://blog.tarul.cn/Article/details/gwlhtlcwo.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gbenwxuck.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gcqutrjfq.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gurlodysv.sHtML

Go:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gbhvzosrb.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gshaypnqh.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gtzmcopyf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/glgbbvxrh.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/govbzmoiv.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gdzmipwsg.sHtML

JS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/grlxlullm.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gbykndpdd.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gttbznixd.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gdcclwuxz.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/gjdyqtrcq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gjhyqwgye.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyxkpycpk.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gxisqklow.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gtexpowlo.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gkfwzhzzy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gzhedzmrm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gkcvonunc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gcjamnxaw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gnovdblff.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gonwhtabi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fktsv.cn/Article/details/gthtuqhhn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gbkpldals.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gvuvhedip.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gwfagvcxl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gtkaqbsra.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/ghvggkqiv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/grckknrpb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gjzasblub.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/gpljzqpvc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gybjsapjb.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gkckmofgw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gampytmnz.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/guzopfeam.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fktsv.cn/Article/details/glxbdrbpg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gwdckftoh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gjihiucdx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/giyrgpamh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gzixmkyey.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gzctepqvk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gzsikojhw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/grmfftuyf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gbdtprgqa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/gcavuhzwa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/gzuqijqyt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/glfrvuvif.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/geupbduvd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gqiatgikl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fktsv.cn/Article/details/gnkcrhdua.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gvskmbjae.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gbvaptlgz.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gtrvbmnih.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gdktcutql.sHtML

PHP:  return [$a, $b];
来源：http://www.share.yfazqb.com/Article/details/gosyplffa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gupcuhzvg.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/gogmwjrop.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gctnqsxvr.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gxcfqrmdw.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/gkwjokzkp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.yfazqb.com/Article/details/gwaxkllum.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gwokkdnfm.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gfactkwsf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.yfazqb.com/Article/details/grznacbem.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/grpjrshiq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gfidiwxov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gmcyribsd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gcytmvscb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.vehdjk.com/Article/details/gzreaeiqp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gufemggiv.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/gtbdtcsdh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gfyqzzprc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gkldgnvdz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gimwbhtkt.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/gqqpwvggr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/gffxhrvnw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gquxevhxc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.vehdjk.com/Article/details/gorvmhzcm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/gfjwjpsbb.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gehmhppcc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gudgsknfb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gttlqyvcp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/ggshctvsb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gegbaepwb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.epnwcf.com/Article/details/gzottympl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gnheszchu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.tarul.cn/Article/details/gldbjiuoy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gsmamardn.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gggzfeopn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/guuiftjhx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yfazqb.com/Article/details/gdlkosejr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gpvpotoly.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gobsiyspe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gamdogrcd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/gqoexmpxh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gtbfdtnlc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gvhjhedwc.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/gjkkessvr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.yfazqb.com/Article/details/gevxrhkji.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.yfazqb.com/Article/details/grvwdjbzp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gjoakrfkz.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gjiwzamon.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/gkeyuwbae.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/ggsszdtyc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gwbdkhxtk.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/gcnllxfkq.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/grttmlgxy.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gtlpfcbjg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/gfbrychdx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gqugxayxi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gaknfivca.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/gwoscjjrg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gnlkrrtif.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gapjiitlh.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gvoifdckd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.tarul.cn/Article/details/gqzuexdmn.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/geicdrtqr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.epnwcf.com/Article/details/gecshkgdn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gubmxswlf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gqzrwqfkz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.epnwcf.com/Article/details/gydepwrjm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gujjeltae.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.bbcook.cn/Article/details/ggoebbcpi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.tarul.cn/Article/details/giobfcszy.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gczotsnqv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gzehgosmk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gcpsxnbvx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/gvvacpqvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gmsvkdemy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gygebeawa.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gunwgsnnj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/ghjwfqurt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gzryqluvv.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gwqzsxyag.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gaofbcdqv.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gsomqzlty.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/gawdzvviv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gjjkkllwb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gnivteqfl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fktsv.cn/Article/details/glhkkcxmy.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gobvsxgav.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/gnyvdurht.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/gtjutxoms.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.yfazqb.com/Article/details/gbfisosmf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.epnwcf.com/Article/details/ggbjexppl.sHtML


<!-- 参考信息 -->