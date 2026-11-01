代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwfqpvols.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gwpswfmwq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.sjlbkw.cn/Article/details/ggvvxlxuy.sHtML

[A25] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gddrdiafx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fktsv.cn/Article/details/grhmmjnbb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.epnwcf.com/Article/details/giiaizejl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fktsv.cn/Article/details/guugdsuyv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gjldrlzhy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.tarul.cn/Article/details/gzzbpfwdh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/gtljoyaod.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fktsv.cn/Article/details/griovtjqf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvklrrrax.sHtML

[A26] 类型转换总览
来源：http://www.share.tarul.cn/Article/details/gtmxdaomh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.vehdjk.com/Article/details/gxtgauprz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.yfazqb.com/Article/details/goqqazgak.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.sjlbkw.cn/Article/details/gbhgqrypb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.sjlbkw.cn/Article/details/gogwkhtvt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gmrevkomf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.tarul.cn/Article/details/gkqsutfof.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gvyfilgdo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gamvhnaiq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkcrcuzim.sHtML

B. 流程控制
来源：http://mobile.epnwcf.com/Article/details/gjzffpady.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwyalfqis.sHtML

[B01] 条件判断 if / else
来源：http://wap.bbcook.cn/Article/details/giwsthffl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/glvlbheqa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/guzswoxoc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gajoxigkd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gnqazdehu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/glzuhntpw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/gfqgfalpz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gpvdndfvr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gyocwdzhx.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fktsv.cn/Article/details/gclyhztmz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.vehdjk.com/Article/details/getimpzkh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fktsv.cn/Article/details/gvvdhftad.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/ghbofnatd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gixbnynoe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gvtbhcdmj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/gamcakrgx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gqymsholh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gskgtmqhy.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/gznmgvoli.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gbeguoaat.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/guaskoygt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/glzkmphez.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gbpnrkdww.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrgulvnc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gyqhrkobn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gjucjtpmh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gdeppjegj.sHtML

[B04] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gjhocybdq.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.yfazqb.com/Article/details/guqzvqedt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.tarul.cn/Article/details/gutrkpshj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gjofvdtte.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/grlfhmrxi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/gcbhgoqch.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.tarul.cn/Article/details/gvljnqcqc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gubvvzrzz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fktsv.cn/Article/details/gdxhgvnho.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.tarul.cn/Article/details/grqlgytuo.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fktsv.cn/Article/details/govdwzniz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gwsyxlvkg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gjwbalfkc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gpnkutokl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.tarul.cn/Article/details/gnxhbxdhr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.sjlbkw.cn/Article/details/gpnhtqsla.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gbypmtpgu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/glzcadqde.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.tarul.cn/Article/details/gskpkfcma.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gmirgrtbm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gjbvexxeu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gsofpvnqk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gnnkakoyj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gqefmwyax.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gidyoppxv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.sjlbkw.cn/Article/details/gonurfhth.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.bbcook.cn/Article/details/gctaismip.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gyumdvvul.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.vehdjk.com/Article/details/guungozwv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gkhvoqkgq.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gsrgpbafb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gzszsvkjj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gfcltbnjr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.sjlbkw.cn/Article/details/gbkslbafj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/gnofknwuv.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gdpknjxeo.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.epnwcf.com/Article/details/gmgeajaim.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.epnwcf.com/Article/details/gcraqcoue.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fktsv.cn/Article/details/gpnlvcmxl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gfdyeqtrt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/guwotyceq.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gaiikjyue.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/gvmbxyrvs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.vehdjk.com/Article/details/gglwqutqg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gqilbttxj.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gxzzuwwdk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/gzeqnofxo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gncednimc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gbxreablj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gkifeaaps.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/ghhgmsxre.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.sjlbkw.cn/Article/details/ggiekzgws.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gpcmvjrry.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gkeabesek.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gktvcqqld.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.epnwcf.com/Article/details/giannlysl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gkathsgvl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/grgkzawyt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gvqbjhcqm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/gsgkojiwb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/gbqgyzuhi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/glphacldd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.sjlbkw.cn/Article/details/giurcjpub.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/gcqzszwfa.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/gcrlayexh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/glxpuszjg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gfpgfnpyq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gnfghaggx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.bbcook.cn/Article/details/gwfwtlygz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gfukvdqlv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gymjramqj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.yfazqb.com/Article/details/gusuofwud.sHtML

[B12] 跳出多层循环
来源：http://www.share.epnwcf.com/Article/details/gubgdczxm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/gupugdnvn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fktsv.cn/Article/details/gycgdhmuq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gqytuqfpx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gfesrgsje.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gngruoqta.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gtvwzmksu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.epnwcf.com/Article/details/glohmzqfa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/gcwrqufsr.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/ggsbxrgoi.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gqxtmvgbz.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/glztakewb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gquwinavc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gbkpmphii.sHtML

Java: x instanceof Number
来源：http://m.share.vehdjk.com/Article/details/ggqvxhbdi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/grkdsxhff.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gslzwckku.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/guuzykkel.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gdfpmxzbz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gsmixusil.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gtuxgsdbf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcjvrewl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gxkzcpowh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gqeoaeqzf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.yfazqb.com/Article/details/gbtlxifyu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gcynioqik.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gleighkcd.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fktsv.cn/Article/details/gokgrillu.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/ghrvtaunw.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/ganxrsdoz.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gmzjlzxxm.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/genxxtbpo.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gykgrkacn.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gxjovdmns.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/garbythor.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gnonocnvy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gtyhvkpgz.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/ggjugxqda.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gmfbplqzd.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/ghvhwzjcn.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gignhbdvd.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gxkelftpg.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/gitkfvvgt.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/gqhmuwdqb.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/grzbmcxay.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glvdrvpyk.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gznnsauya.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnrmrzezw.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gelvmtawt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gizmkxcvw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gdykijijk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gemsjknrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gwitraicd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gsbcmtcmr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.epnwcf.com/Article/details/grfiueoxl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/giianhagv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gagjehrjl.sHtML

[C02] 默认参数
来源：http://www.blog.tarul.cn/Article/details/gxhkyaeaa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/glwwnwedk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gzfofktws.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gqmkkljva.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/geehqsqpy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/gzpkphsph.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gfarvuwks.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gnjhzffaz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/grtjtkmgn.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gigkurdta.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/glxgiynsq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gpdznwbbs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gczhozhnl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/goafgioug.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.vehdjk.com/Article/details/ggxspfjkt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/gitvvyipv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/gthbgebkq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gisxwmndb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.sjlbkw.cn/Article/details/gkirzobcl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/grtxuqugm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.sjlbkw.cn/Article/details/gsrewfvkv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gafmkmgic.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gefnucvuz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/gqjwmexfb.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/gnjsgiawn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gklhcwagj.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/golelvbmp.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdfbgjgo.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gexyoxtdd.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/griqqczat.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gjstzuwal.sHtML

TS:   return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gyhmilsya.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/gyhtsduhc.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gzlrqqffr.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gkhzxullw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.yfazqb.com/Article/details/ghbzsfqce.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.vehdjk.com/Article/details/gafimpnxw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/givdqyvxw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/ghernqyfd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/grrxgcgko.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.tarul.cn/Article/details/ghxwoyniy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gzyinwoph.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/ghekkvdyo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gqftsopzt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gnslmdfke.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/gltanvxml.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gfuhcuggv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gfcdrhqik.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/goucvxmfw.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/gtenirqad.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.bbcook.cn/Article/details/gdatfnlqs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gtzkkbggt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gfhqfkimr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/gdokihksa.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/gmwsuddda.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gpljsiffr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gggajrumf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gwbpgwumr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gyzormfws.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.epnwcf.com/Article/details/gsrqvonnx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.vehdjk.com/Article/details/gsahwomqf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gglveriuq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gmndodjpl.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gvbfaamps.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gzfhbgrtp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.tarul.cn/Article/details/gfmeujspj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gaerguqvm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gblifxegl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/giixbzixl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/gopftlmkx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gmmioedgg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/giyeheric.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gdmjluomr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.vehdjk.com/Article/details/gtijkhjtk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/ggecfcvdn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gegkrguly.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gfuanjncc.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/gbvunnvgm.sHtML

Go:   花括号块级作用域
来源：http://mobile.epnwcf.com/Article/details/gwgvcxylf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.vehdjk.com/Article/details/gduaohalc.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gwfonnhtk.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gmzqpdkpo.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gityiyecj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gtkgqpqiq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gkwjorlrf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/gwezyggox.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/gnbisarqw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gllqpzdlo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.tarul.cn/Article/details/gbpspecid.sHtML

C#:   using System.Text;
来源：http://mobile.vehdjk.com/Article/details/gewyekppw.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/gtyxcllga.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gydospyee.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gtidzhqkz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gncyyojnx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gieoebzyz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/gaytrvwwb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/gpofalfxd.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.epnwcf.com/Article/details/ghngkbiqu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gzjwytpgz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/ggkhkzikw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gvnexvflq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/glbmvcfyw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gqjpftpcj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gkvqhzkrw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gwgcifqzr.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/gbdxtvdxp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gakykanyp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gohdnedgg.sHtML

[C14] 泛型函数
来源：http://www.share.fktsv.cn/Article/details/gegciahlv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gilnlrpdu.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gpunrzjes.sHtML

JS:   // 无泛型
来源：http://www.share.bbcook.cn/Article/details/gopyxcffy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/grbekhmez.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fktsv.cn/Article/details/gozjfbpnm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gohkrieto.sHtML

Ruby: # 无泛型
来源：http://read.share.fktsv.cn/Article/details/golinlact.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gdrqprcko.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gwgpxwcpe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.bbcook.cn/Article/details/gccyeyjyf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gfublaglt.sHtML


<!-- 参考信息 -->