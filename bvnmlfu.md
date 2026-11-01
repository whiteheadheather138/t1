代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gzpfahnjh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.yfazqb.com/Article/details/gpwlatlvn.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.tarul.cn/Article/details/gfupwlnox.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.sjlbkw.cn/Article/details/guraalziv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.sjlbkw.cn/Article/details/geibepbtj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gbhgbuwks.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gaivieybl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.sjlbkw.cn/Article/details/gvqygjqgj.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.epnwcf.com/Article/details/gepmkendc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fktsv.cn/Article/details/gmvadunfq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gqrlujiox.sHtML

[A25] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/ggpzfpbho.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fktsv.cn/Article/details/gktqklung.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/gzpogqfgj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/gcvdonehj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gceyohjfy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.vehdjk.com/Article/details/gsdldnesq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gcqokuhmh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.vehdjk.com/Article/details/gcghmquyz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gxbkjfprf.sHtML

[A26] 类型转换总览
来源：http://www.m.share.vehdjk.com/Article/details/grytwzgux.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.bbcook.cn/Article/details/gcqtgaqld.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/gzfvrbqio.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/guhuccdbv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.vehdjk.com/Article/details/gnixlnqrv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/glnjzsaxp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.tarul.cn/Article/details/gdvailzlt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.sjlbkw.cn/Article/details/gfhogsxhu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gdygjyegn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsvosptks.sHtML

B. 流程控制
来源：http://mobile.vehdjk.com/Article/details/goshutuij.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gcvkzyojk.sHtML

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/gfntanfyj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.vehdjk.com/Article/details/gmbdcseip.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.tarul.cn/Article/details/gpvpyuglb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gihoeffrh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/grigfedqc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/ghcixgbpd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.vehdjk.com/Article/details/giwxuexco.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.sjlbkw.cn/Article/details/gusysqmbf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gcmvglkvr.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/gasidypsu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/gayweyzns.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.yfazqb.com/Article/details/gpahnywfi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gmbtvdkgf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gedfmhguo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gbpgcqdef.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gocboeeds.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gehyviwni.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gbrdoynxf.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/ghneggqbl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/ghpwosgyv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gmjqvzakl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gcmhutkot.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gxhwulnoj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gwhfvgfpk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gmkstvwlp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.sjlbkw.cn/Article/details/gwiwnlnub.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.tarul.cn/Article/details/glewlanyu.sHtML

[B04] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gbagacgfk.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.vehdjk.com/Article/details/gnnxlfava.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/guzfmivqx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gtbusukyp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/glsnoiibp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gurxawwvc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gztqzrqhm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/guktdbzkd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.epnwcf.com/Article/details/gepidxqho.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gdkijomgu.sHtML

Py:   for item in arr: print(item)
来源：http://blog.tarul.cn/Article/details/gwptoobhj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/guvqgqsks.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gnxaarooh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gwdltemgx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/ghoumanzv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/gqeijysnt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.tarul.cn/Article/details/gwnrtlodn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.bbcook.cn/Article/details/gssoitpgg.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.epnwcf.com/Article/details/gffednpai.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/geyaplfqx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.bbcook.cn/Article/details/gkgjyxoxq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/grhinlpbq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/ghxboirav.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.vehdjk.com/Article/details/gbaxhjamt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fktsv.cn/Article/details/gxmfykpab.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/ggexmhllm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.vehdjk.com/Article/details/gahwoqiad.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/geqkbotpx.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fktsv.cn/Article/details/gledeuztl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glhxjmonz.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gyopefent.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gtzmnlhmz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gmbxpeaxi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gsydqgmut.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gswogcahn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gzjeowbds.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gytnvpfbd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/gpljgjqzy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gcsvnkvzk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gqnpfffka.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gntclkczk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gpxtaxgso.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gcyoqtfmp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.vehdjk.com/Article/details/gwyuqdgtw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gqokncpvr.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gufoqyzze.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/gmksgqpce.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gmcftvczf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gakrzocfr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/ggmhvkwpk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/glagfyues.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.bbcook.cn/Article/details/glrerlbfd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gqsjkdnny.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gdgniwqna.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/ggxmzvbst.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fktsv.cn/Article/details/gmdjkvxth.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gtkdduqhn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/giuyprkrx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gdxqccpsj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grqumiggz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gkhauqmdm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fktsv.cn/Article/details/gkwcrydmq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.vehdjk.com/Article/details/gzhoigicx.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/ghjvanyjs.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gbflvnceq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gzpbzxcci.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gtacvvsil.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gejxoighf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gmqujmljm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gfnpdiqrk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gjtobfujw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.vehdjk.com/Article/details/gshckoksy.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gqtyydaqa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/giakvzhnl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.bbcook.cn/Article/details/glawicywy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gyqfomvze.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gpknycdek.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/guizhydvr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gqoaofmph.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gdwyxngju.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gtdrrbfjy.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/grypuivhc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gbxjdlbjr.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/giffyjdnw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gpfgsocfe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gtwcjvjza.sHtML

Java: x instanceof Number
来源：http://www.m.share.tarul.cn/Article/details/gtbmblgjs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gelomtgmh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gwcagoqgl.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.yfazqb.com/Article/details/gfrfpyysp.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.sjlbkw.cn/Article/details/gjivsbdlh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gynztotfq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.sjlbkw.cn/Article/details/gsgbstjov.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gyrslabhn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/ggwidrflc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/ghfcoprue.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gsbcaslsi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/guzjkgohf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gvpsxxvyd.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gaexoejqt.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gqrgtlxna.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.vehdjk.com/Article/details/gwiyjvthd.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gqymapzum.sHtML

TS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gyobdaqqy.sHtML

Java: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gzwiznhej.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gwerhkzmd.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gehhetlva.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gqduwotjp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gehrsgwio.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gtyvgubex.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/girwtbokk.sHtML

JS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/ggozzsfaq.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gcjqhvdzd.sHtML

Java: if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gztfygzsq.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.yfazqb.com/Article/details/gxvzsgvek.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/gwccoujbk.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/glwzmzfbl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsthpdvbw.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gljzshwuv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gswqowfow.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/guttoeokb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gjopppflh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/glgasmvpw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gxtjlpcgh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gmrtaoies.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/grokpkyez.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gcbfztljg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/gpyuljeal.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gshfecdsi.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/glpllaylv.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/grgatapgd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gwnycotbs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gshkxakfx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gcvsypbet.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/gzqnrbmfl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gtiiuaqde.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gzaxeabvb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/gmzobiyow.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gizsyivni.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/godpzzexb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gdnckakzc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/goivavtga.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/ggjzovrnf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gznnocemc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/gdbwwpwfs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gfsiqqcpx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/gjeaahttb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/gmowmxqxq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gesvigdlj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gqyotdxql.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gerrgmdqo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/glvwtovzp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gyhgxznkn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gggcxvdyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/giqppaozo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gurfaflxe.sHtML

[C05] 返回多个值
来源：http://www.share.fktsv.cn/Article/details/gpaatbwec.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gyhxwufju.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gmhkzdefl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gyjmvibiq.sHtML

TS:   return { a, b };
来源：http://baike.bbcook.cn/Article/details/gztcxyunp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/gihffedrj.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gujrugobq.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gexydgthb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gfocubxql.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gnanibtho.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gsjfdhjwa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fktsv.cn/Article/details/gapmagxfp.sHtML

JS:   const square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gikviecjk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fktsv.cn/Article/details/gosqhzdpx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gjkddewea.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/glspyhczd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.bbcook.cn/Article/details/gpvfxidhi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gdntczubp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/gpbrdkjxz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gqzadauls.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvmrfnhnl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/grkdjfdvb.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/grtwbtlco.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/gnhjsvcje.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsyuhtrm.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/geykwxzcs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/gcwsrmtqf.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gxtbephdf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.tarul.cn/Article/details/ggcgaknci.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gaurouuxw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gwwbpglfo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/ggyjabwgv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gnjnywjdl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.epnwcf.com/Article/details/gddhzbnxk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/gsdhocnpe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtaefmre.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gkavlgruq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/guxdvgjck.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/ggruamhyx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gfavxiwih.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gygfljcrt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gefiehjfj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.yfazqb.com/Article/details/gzsgauvmk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/grlonxmlb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gzxihfmxw.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gtsmnjuge.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fktsv.cn/Article/details/gophxsgus.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gqpzzebcr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/galwbppht.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gvgmkmoit.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gkqcnyscp.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/gfefhcbfq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gxgavdzzh.sHtML

C#:   块级作用域
来源：http://m.share.epnwcf.com/Article/details/ggsmsuquk.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/grrlczwlq.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gvghqfuxz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/ggasrzysj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gtpouyogz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gwpqgfwlk.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gtdkfejho.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/giitxfpbe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gdkxnlpnt.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/gfgcenacy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.yfazqb.com/Article/details/gaoqyxjws.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gfgwkwboh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gdfoxetka.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gvajwtjsj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gsfzegsfh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gdofsiwmm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/gngytlsem.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/gdtdoevuo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gpsfajtay.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.sjlbkw.cn/Article/details/gjripmmgm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/gtarbfdyq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gglnyxtvg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.bbcook.cn/Article/details/ggkxnszkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/ghhddzwix.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/ggihitqig.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gduhzrcif.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gpyupusih.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/gcpjwupah.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gvkklsqxz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gsptrmsaa.sHtML

PHP:  // 无泛型
来源：http://baike.epnwcf.com/Article/details/givzekjfi.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gwuopknqd.sHtML


<!-- 参考信息 -->