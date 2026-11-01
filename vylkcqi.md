代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.bbcook.cn/Article/details/gagnwbihu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/ghrdhxpna.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/ghfzosrpk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.bbcook.cn/Article/details/gqzypztyc.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/goawxfcin.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.sjlbkw.cn/Article/details/gdskzkqil.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fktsv.cn/Article/details/gmeuhnzgx.sHtML

[A25] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gsgfypkyp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.epnwcf.com/Article/details/gomcwepfo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/glgjamaqr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/ghaqkjneh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gvpesnfnl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.bbcook.cn/Article/details/gukxowjen.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gwhyyjarl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.bbcook.cn/Article/details/gavlhjmyb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/gzdzvyrrj.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/ggcasjkkw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.vehdjk.com/Article/details/ggqqthdpt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/gmfxmmfgw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gprcgjvvj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.bbcook.cn/Article/details/gjscowaur.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gbmnvkapj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.bbcook.cn/Article/details/gkehlhtew.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.epnwcf.com/Article/details/glbkwgheo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gzrbivmmq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvzyfvzpy.sHtML

B. 流程控制
来源：http://read.share.sjlbkw.cn/Article/details/gahnxjbau.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gaxrgfrzk.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.vehdjk.com/Article/details/gqljpqaou.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.yfazqb.com/Article/details/glwzbulae.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.tarul.cn/Article/details/gkdxhkvpd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gzqdgqfxt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gtghfrynz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gxplqpekq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.tarul.cn/Article/details/ghqfripwa.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fktsv.cn/Article/details/gjaxhlrns.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gysjqspdw.sHtML

[B02] 多分支 else if / elif
来源：http://baike.vehdjk.com/Article/details/gfapmxhir.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.bbcook.cn/Article/details/gwokyhngp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.sjlbkw.cn/Article/details/gtszrjgpn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gmjtxduui.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/grpiagmfa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/glcvhgpca.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.tarul.cn/Article/details/gvwdyvysv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.vehdjk.com/Article/details/gylhunsqs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gkhmhgkfr.sHtML

[B03] switch / match / case
来源：http://www.share.vehdjk.com/Article/details/gnuunbxal.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gdtzrlcjm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gribczjje.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gyvbjpcxn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gafscfonw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gepasgjys.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.epnwcf.com/Article/details/gcvhxvzvs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.tarul.cn/Article/details/gobschuhd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.yfazqb.com/Article/details/gmeiniwgg.sHtML

[B04] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gtvzcfxiu.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.vehdjk.com/Article/details/gsniopssf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/grtmzzxzm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gzyvxsvyx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gishtnxzv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gjohmnqwd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.vehdjk.com/Article/details/ghvjkwcdy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.bbcook.cn/Article/details/gggsehpkd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.tarul.cn/Article/details/gthonfqfo.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gpwgeikzx.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gijtnqhwq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.yfazqb.com/Article/details/gzamxxvxx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gelhuccwp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gxqpdiogf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.tarul.cn/Article/details/glkmdakxg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gsflfzqra.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/gdizupekq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fktsv.cn/Article/details/gceeaeifg.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/ghxxiywjl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.epnwcf.com/Article/details/gpkkzisow.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.vehdjk.com/Article/details/gvzshrmnk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gpowyflnz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/glwblhfxg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.tarul.cn/Article/details/gtoyxzqzr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.vehdjk.com/Article/details/gonwumncb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/ggllfwgln.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.vehdjk.com/Article/details/gclfrrzke.sHtML

[B07] while 循环
来源：http://www.share.tarul.cn/Article/details/gkkfrgpev.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/gowjfbayi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gsmdchvxv.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gwvqkktwl.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gnczlccvj.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/giomfprnk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gamwyfwui.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gmztpxqeb.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gemzrljfm.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/giuzyfuhn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/ghobwplyx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gijnfjapl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gdewvionp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/glrustidx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gadytrtnp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/gkiqjrmfa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/grvjmbtlx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gxtoruajf.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gjhsnueka.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gkcxxctno.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gjdtesijs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gwdkljmyo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gyhfswfjy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gtarcqplj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gtehenryj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.yfazqb.com/Article/details/gtrrtgbpi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gfsdbzyhv.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gbwqaioge.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.epnwcf.com/Article/details/gurkmzdlg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/gsgowyukm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gaeiwngni.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjjbodqm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fktsv.cn/Article/details/gjajnfekr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gdoraexhu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/gdmejkhvg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fktsv.cn/Article/details/gpuaieimf.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/grxdrvuyf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.tarul.cn/Article/details/gbizgsdzz.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gakxcrqqg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gucbqhqko.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gpmrmsert.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/gbrytefwg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/gqwdxjowr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/glruvauzk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/gxvedjlwy.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/giskewxvd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gxddxprmc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.vehdjk.com/Article/details/gzvynlymt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/grdfnjqlp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/grxvajiys.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/ggmzyqfvs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gbfmoayno.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gsqrfvljd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gcmztklsd.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gtqaprpfq.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gyneymyqv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gkbzrfsza.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gzjfbdkft.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gcexxucqz.sHtML

Java: x instanceof Number
来源：http://read.share.yfazqb.com/Article/details/gjhhxfkxb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gkcgmouef.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/gfbmqpdvr.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gcfnfxtze.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gwcgunyru.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.vehdjk.com/Article/details/gxrtlqmko.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.bbcook.cn/Article/details/gysrsmbxe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gdogfwygn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/giwepekja.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.tarul.cn/Article/details/gwgrwikwb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gxvhrtshd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gdfhidzhf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gsijzzkbz.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/grnnmezma.sHtML

Py:   a and b or not c
来源：http://blog.tarul.cn/Article/details/gshhjldob.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gfynwjjch.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gtxruslhf.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/glwmjoefw.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gavnrnvux.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gqfqpowsc.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gcazpadnf.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/grjslrouc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.yfazqb.com/Article/details/gezduezfh.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/gyqutaqhe.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.sjlbkw.cn/Article/details/gqftzuxxs.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/ggmguzyin.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gpheaihmt.sHtML

Java: if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/grywzevzf.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gdewukbld.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gugfxlgym.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gctqdeyou.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghnwumggx.sHtML

C. 函数与作用域
来源：http://www.m.share.vehdjk.com/Article/details/genmcchac.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzdrwwhik.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gzsckptfs.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gjlcincdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gwvvqcxvs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gqaigbxgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gcjtesrzc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/guqfxspiw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gomikoywz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/gerpotvsg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gogzgaypm.sHtML

[C02] 默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gbofzowcs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/gqkphziyn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gmcqrqmvb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gsayguwuq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/ggcspqznd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gpywuolld.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gtyhrbcgw.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gxsntkmas.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gzlvrxfkd.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gtztwjypx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gyzpravno.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/ghqcnsjns.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/ghlvxiopb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/grlycjnbt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gtgpxuvou.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/gdahsptac.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gqujdgsch.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/gqxusopxe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/guwagrakw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.vehdjk.com/Article/details/gycspzckz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/ggkvtpywy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/gcwojuttu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/gjslsgecr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gljyrsmcr.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gufkqabbv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/ghebaegtk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gehljkbjc.sHtML

[C05] 返回多个值
来源：http://www.blog.vehdjk.com/Article/details/gereyurus.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gfrbncaxq.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/gdgnvchju.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/gvkpoyfxv.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gdwzetdwd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.vehdjk.com/Article/details/gpdlqbbjl.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgfvbskk.sHtML

Ruby: return a, b
来源：http://mobile.fktsv.cn/Article/details/gszgwwnjb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.tarul.cn/Article/details/gcldfvxwd.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/gqvxckvrk.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gswwlmxwh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gacdjlczp.sHtML

JS:   const square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/ggnvjmpii.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gyzzfhubo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gktotrbrf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gmotfpwcj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gjzrephcq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gzacoktvm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gheqibapb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/guhyahezf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gfgxxbfpl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gkfqwfsvx.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gnziedbvg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/gmwhkzbag.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.sjlbkw.cn/Article/details/gykbqrxxb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gagccxffv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.tarul.cn/Article/details/gyysxonbq.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gmgrjfvge.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.bbcook.cn/Article/details/gmrgkpbuh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gnnuegvpo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gdvzkiodu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/glnqyqafj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/ggtjxnwkp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gwvxmggvz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.yfazqb.com/Article/details/gnuuapmll.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gjmwmngwl.sHtML

[C09] 递归
来源：http://baike.bbcook.cn/Article/details/gwclfjqsi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gtufkyuak.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gochhsujl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gedwxsqni.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/guurywfof.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gvpwaowrw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.yfazqb.com/Article/details/glvknqtnt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gsrayogcz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwtqkwyc.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/gspgsnrhe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gfvepjkda.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/grorrgtrw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.tarul.cn/Article/details/geqoppjcq.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gmonadujk.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/gtktwxjpu.sHtML

Go:   花括号块级作用域
来源：http://baike.vehdjk.com/Article/details/gegghlmbm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gqngfoses.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gcxgqtjkz.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gvpbillmc.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/gqxassipu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gwqcsashw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/ghhiygikq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/gbonpvhgr.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gphmtvcnv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gindyxalu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/gyhcsicgp.sHtML

C#:   using System.Text;
来源：http://blog.sjlbkw.cn/Article/details/gkxxykuvf.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/gqntbihsw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/gaaxkeuxc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.sjlbkw.cn/Article/details/gmgwpjbur.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gbrsnmjgn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/gaxzmccyl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.vehdjk.com/Article/details/gtepcxidq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gpahiueqb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.tarul.cn/Article/details/gylnkcquo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gqhkzrrzv.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fktsv.cn/Article/details/gsgxrpsyb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/ggenvayhi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gtjpicoov.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gdltmnpft.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gmhjvypac.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gybzovjfp.sHtML

Go:   func add(a, b int) int
来源：http://mobile.sjlbkw.cn/Article/details/gnxicghfh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/graoppnxx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gobuhquhp.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/goszvepwf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/ggrptislb.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gxmgmapcr.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gigubuoxw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/gvdcnnhqp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/gusxnyosp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gxizexmme.sHtML

Ruby: # 无泛型
来源：http://baike.tarul.cn/Article/details/gjumtoruw.sHtML


<!-- 参考信息 -->