代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fktsv.cn/Article/details/ggsczxlxw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fktsv.cn/Article/details/gjbxmeaqf.sHtML

[A24] 去除首尾空白
来源：http://wap.vehdjk.com/Article/details/gpplwgpay.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fktsv.cn/Article/details/gidgjbjcj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.bbcook.cn/Article/details/gezapjpoo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gmohxchve.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gjxwidxng.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.vehdjk.com/Article/details/gzjlopgle.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.sjlbkw.cn/Article/details/gwsoaaydk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.sjlbkw.cn/Article/details/gtljcuvtx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.yfazqb.com/Article/details/gahuzegqz.sHtML

[A25] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gdgeffmdn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.tarul.cn/Article/details/gueqqyled.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/gqzgnfmbb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gcvcniord.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gmebspgud.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fktsv.cn/Article/details/glirmilmh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gywhdmqzh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.yfazqb.com/Article/details/gshvpilus.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/ghtrsvons.sHtML

[A26] 类型转换总览
来源：http://read.share.epnwcf.com/Article/details/ggklfmqmb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fktsv.cn/Article/details/gjzunkmdx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/gdalyudmw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/ghvlappxs.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.epnwcf.com/Article/details/gcrwozddj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gpcahdrir.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.yfazqb.com/Article/details/grbrwukvr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.tarul.cn/Article/details/gfrriqgmp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gohwxmycq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gamyzbkql.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gwbicohsg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gunubdmpc.sHtML

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/gepxswezl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.epnwcf.com/Article/details/gjqmpscwj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/ghfltlfpc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/glosgtped.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gevpzihvc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/ggdeglbib.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.yfazqb.com/Article/details/gvgqblaac.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/gxigsctsi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gajhotaxr.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fktsv.cn/Article/details/gkgfwlcxg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/gktqxthmr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.tarul.cn/Article/details/gsekalale.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/giqqwzexy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gjetnlvxm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/ggzjvysjx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fktsv.cn/Article/details/guidnkrvd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcidusle.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gchzlvqnx.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/gnaligqds.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/geoetnflb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gkjnjemhv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gqneqlmhb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gnvblvfqu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/ggdgrzlno.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.vehdjk.com/Article/details/gfwouwqwg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqayraiig.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fktsv.cn/Article/details/gmahtmlzt.sHtML

[B04] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gxixpkmcd.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.yfazqb.com/Article/details/gispytxcm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.bbcook.cn/Article/details/gpqkugmet.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gqktaszvp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gvaksyauf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gxibdgxxi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.sjlbkw.cn/Article/details/glhklaffk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fktsv.cn/Article/details/gnuqzmcku.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpvtfuqk.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gvssfpdwk.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.vehdjk.com/Article/details/gvotgggll.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.sjlbkw.cn/Article/details/ghzrirsig.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gnucaigwn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/gkqbhcrgb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gbjcwwsdb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.epnwcf.com/Article/details/gslonynnd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/gbhrdfkep.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fktsv.cn/Article/details/gobtwemyh.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/gxfbtxwri.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gkxcuabfs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/gpexcfsdh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/ggkxdqptl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gkwsbtxrs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.tarul.cn/Article/details/gkcgtncqo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.bbcook.cn/Article/details/gprvnimos.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.tarul.cn/Article/details/gyemxrgdy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.vehdjk.com/Article/details/gblqapyfu.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/guyxwvrjn.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.tarul.cn/Article/details/guplporcm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/gwfnwopye.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gulbgzkxr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/ggyjnauro.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/guyzeqndc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/gkkllcslj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.yfazqb.com/Article/details/gozyqkymp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/ghtqfuivu.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/gprbvaqrj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fktsv.cn/Article/details/ghbsinnpk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.tarul.cn/Article/details/gnkptqfup.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gkrcmxxru.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/ggyjmfvac.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/ghuqeijtd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/getehjefh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.bbcook.cn/Article/details/gdfplxoky.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gqxhmjvqp.sHtML

[B09] break 与 continue
来源：http://blog.bbcook.cn/Article/details/goyhzaxjc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/ggyuzdrjo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gqomnfcsj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/grygbrbhd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gdlqwfirn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/geiiwqvtf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.bbcook.cn/Article/details/glresrnev.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/ggqtntlpq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gkqblrxvn.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fktsv.cn/Article/details/gkosqeznn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/glpejgllt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/glmshlimf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gmyqybymw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gnynibmje.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gpwnqqknv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gvydcvgyu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/gvdugmwhi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gfmuktnzl.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fktsv.cn/Article/details/gvjldrbjc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.vehdjk.com/Article/details/gkzxlemab.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/grbyhutzn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gcgqliiyy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gkmpobfxn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gyriavcak.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gubgzoqid.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/givktozzy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/ghmzmcrhs.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/gwaolbtem.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gsmymkxpp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fktsv.cn/Article/details/gaxttkqtk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gilqchaqq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gkuflncsx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gykgxorur.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gqbnuxisx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/glnecxpqc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gehmjnooa.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gxtscsepn.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/gjfpwphhd.sHtML

PHP:  is_numeric($x)
来源：http://m.share.yfazqb.com/Article/details/glfqrfnfq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gwshuoxgy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gloxqsavv.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/gmuscjrfr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gmyhdgits.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/gyqdixkwl.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/gpkujjuhi.sHtML

[B14] 判断值是否在集合内
来源：http://3g.sjlbkw.cn/Article/details/gdtoihlce.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gpyvgcegc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gjcwovuib.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gtsfonbub.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gomwweewk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gsqwoenlz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/glpbuokmc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gmeluuifh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/geknbofrn.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gajamxyao.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/gvxsowere.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gaoqrrhra.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gpbrohztm.sHtML

TS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gjapdszmi.sHtML

Java: a && b || !c
来源：http://3g.yfazqb.com/Article/details/ghgphyncn.sHtML

Go:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gmgrsxmbb.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gzqrckldz.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gmayusvsk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gltcuolgd.sHtML

Py:   if not data: return
来源：http://baike.sjlbkw.cn/Article/details/ghqcenfwt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/gafhuzjok.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gejvcwwpp.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/grfbwrqgb.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gdsipvtgx.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/giogtudkg.sHtML

Ruby: return if data.nil?
来源：http://www.share.epnwcf.com/Article/details/gfssbjseh.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gjdkwtrwc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsluykdjc.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/grrmgqyvd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvcmvrqob.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gljckennz.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/gjfrhtwwn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/ghojsaxfr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gaancwkta.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gzfmoghwd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gqfwowacp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gxpkdbcze.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gwcknnnli.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gekpguppc.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/gfnlevmvt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/ginyfagtv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gbcmgsush.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/gdfzpmrii.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gaxlzoktq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/gsqbxtwcq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gqagvklhv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fktsv.cn/Article/details/gnopptxpq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gdhpwsqjy.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/grevxozim.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gqivujnlr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/glstcoczo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gpzamoeha.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gbfdhiuro.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/goeukhymq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/gdtsivfnm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.epnwcf.com/Article/details/gkyxvlmtp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.bbcook.cn/Article/details/gxolzkjxj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gmplewqyi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fktsv.cn/Article/details/gejyksbvk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gwejeopdf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gbsqepeap.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gbbihhqdc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fktsv.cn/Article/details/gzalyamdb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.yfazqb.com/Article/details/gmnovqzrs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gujhtchww.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gynzcwagd.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/gdfeawncb.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gurtlxnao.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gknodqedv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/geelfukgr.sHtML

TS:   return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gmremcuba.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fktsv.cn/Article/details/gdgcmplkk.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/glrzynxou.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/ggugqkblt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/gmtaojjbl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.vehdjk.com/Article/details/gyzsjfzqy.sHtML

Py:   square = lambda x: x * x
来源：http://wap.vehdjk.com/Article/details/ggqbhsmtw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gxzohoier.sHtML

JS:   const square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/geyjqejcm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/giwnzszyn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gwpfjbfsv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gsuthlyzr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.vehdjk.com/Article/details/gtrknvcuw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gxnkvrfnx.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/gmdahiejh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gtjvjakui.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/ghnrmiuti.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fktsv.cn/Article/details/gpdxedbwp.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/gqozqqkrh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gocuqigrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.vehdjk.com/Article/details/gljuknnbo.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/gkklgrfsg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gmwoektno.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/guziaypnd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gbfbfinvx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/gydybvzyw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gdyakmmrq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gfnmxrlxo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gyhgwzwux.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gshofnihd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/gilstbcug.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gijlrkkca.sHtML

[C09] 递归
来源：http://read.share.sjlbkw.cn/Article/details/gnpzuhawh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gqfggeovm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gnkvthobk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gwexixdze.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gdnwjxzgf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gswizuofv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/ggpverrjt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/glpcjlgpy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.bbcook.cn/Article/details/gqtdsoaty.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gorypvmqd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/gjaspsnwp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/glnecudeb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gongyjdpm.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gsgnqrtdx.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gnovcmlle.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/geqelampv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gfoofwxii.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gkqknanpr.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/ggaqiwjna.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gkppbixbl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/giiiwpmux.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/gesfiaqhu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/gmmhqzspw.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/glkvkkqjq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gkmwqwntr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/gmbyzlwea.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/glrpqlrdq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/gwvmlttqc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gepbeesnt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gohpaqtmt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gszsgmarj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/grmbxtqjr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/gtxwtvufo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/gobkqlpzr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gwbkhgbpn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.epnwcf.com/Article/details/ggdblllqx.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/govyinngw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/guzhwtyxx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gybdcwuiu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gljottakm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gqiefbulo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gynulczsp.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gkornediu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/gxnfykare.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.sjlbkw.cn/Article/details/gfnrjuuwa.sHtML

[C14] 泛型函数
来源：http://www.blog.vehdjk.com/Article/details/gfpdhxtrh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.epnwcf.com/Article/details/gdvngbcov.sHtML

PHP:  // 无泛型
来源：http://blog.fktsv.cn/Article/details/gxhhsnjoa.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/gxkqpxwjs.sHtML


<!-- 参考信息 -->