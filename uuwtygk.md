代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gtozrlafs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqxqiqkb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gbslabkit.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.sjlbkw.cn/Article/details/gcjtydjka.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.yfazqb.com/Article/details/gscayxqzo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/gaubjjqru.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.tarul.cn/Article/details/gnuqshlds.sHtML

[A25] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gunupdcwu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fktsv.cn/Article/details/gxnrypdxe.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fktsv.cn/Article/details/gbbxyccpc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/gaheenstf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsfqrwar.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.sjlbkw.cn/Article/details/gljgpyjwd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gnehhnqse.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.tarul.cn/Article/details/gvvxbijyc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gkqliolgp.sHtML

[A26] 类型转换总览
来源：http://baike.sjlbkw.cn/Article/details/gredazgmg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/gsygqwday.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.vehdjk.com/Article/details/gtqyhbahe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/glpvmhmad.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gwbyjdxmg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/guibshtgh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.tarul.cn/Article/details/gjngbxsaw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gonhujtlq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/geappiwam.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gpcfrgrmj.sHtML

B. 流程控制
来源：http://m.share.sjlbkw.cn/Article/details/gswtnyegm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/garpyiyic.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/geblaxbty.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/ghpyalqyp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.yfazqb.com/Article/details/gvdeqrkpi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gwxipcmad.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gwliyapam.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/grqfrcgig.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.tarul.cn/Article/details/gzyszfroz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gxsnslihq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/glzlsofae.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/gieugegli.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gnpdmuzhp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.vehdjk.com/Article/details/grnbetgzz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gzsymxwjp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gunezfwbz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gzdfidlsl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.tarul.cn/Article/details/ggwazacec.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.tarul.cn/Article/details/gurvlvmmp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gycsxcwnd.sHtML

[B03] switch / match / case
来源：http://blog.fktsv.cn/Article/details/ghjfdrozl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.bbcook.cn/Article/details/gllsszjwm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gmcjvskff.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gpvjwqpvf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gothacguq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gologvecr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gavzkbwtd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.vehdjk.com/Article/details/gvdigvmjj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.tarul.cn/Article/details/giafwwitt.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gmsshspcs.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.yfazqb.com/Article/details/gjbkttbyj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.sjlbkw.cn/Article/details/gttdaoviz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gpiaxokjc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gdixzihcz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gvrogxval.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.vehdjk.com/Article/details/gtisqhyls.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gaivrozsy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gjaxfdpsr.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gktahcvwr.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.vehdjk.com/Article/details/ghmdfewzh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.epnwcf.com/Article/details/gidnjwliq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gvjenhlwu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gmrdwfewu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/grycaiiyq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.bbcook.cn/Article/details/gqhsrqlgh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.bbcook.cn/Article/details/gvgjznrjt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fktsv.cn/Article/details/gsfotckum.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/gmfnrdfwn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/gdanecozr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gyslsdagr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/grvineggr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gokciydnh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/gwqafgpbq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/gkhgocjed.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.tarul.cn/Article/details/gfbcahohg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/grgmrfiwk.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gysvsbgbm.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.yfazqb.com/Article/details/gweinonnf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/goijgipzv.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gadquecpc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gmovoxuxh.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gozdfbvlz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/gqpbzozha.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/gniscqbat.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gwjjstexm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gjhyxtyhv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/gswrajvyl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gvxekysmq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gjuaxnndm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gogyvhvqn.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gzxlzlaqn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gtrqbuvhk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.epnwcf.com/Article/details/gpzwkxtvp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/ghndttaah.sHtML

[B09] break 与 continue
来源：http://blog.vehdjk.com/Article/details/gwdackbyr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/ghqzwsizp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gbpydrdwz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gkwoqoobz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gzalvfzhx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gxokfbqki.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/gpqwutxwk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/gmmliqlgt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/glnavdgmj.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.yfazqb.com/Article/details/grxmqbrpw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/gnbywwnsi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/gxauudzol.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gpcvswgpd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/goeylysju.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.vehdjk.com/Article/details/gygbcjikn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gqhetocml.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.epnwcf.com/Article/details/gwoowtdvq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/gqcfulagp.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.sjlbkw.cn/Article/details/gonpejnwg.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gwlqzznim.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gxqhyidlz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gzjtfadbu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gmaxvkhsq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.epnwcf.com/Article/details/gkymkdjtf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gerdmhnjf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gcbjlybqa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gtikbnsfs.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/ghvmphzah.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/gyrgxdwcn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/gvvblkjpf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gfiowigsv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/ggbkmzjyd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gsarkslqa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/govqnhhya.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/gkuglbhjr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gfkfkwgcr.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gzprafapu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.vehdjk.com/Article/details/gujfsqdel.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gkurnhlqk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gaptizivp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gwnylnczg.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/gswtpsehv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.sjlbkw.cn/Article/details/gsmmkvkso.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/gzrtpiugy.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gobsskegr.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fktsv.cn/Article/details/gjvhcqgaf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/gjaacpxkn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.epnwcf.com/Article/details/guvfjkafi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gkjsboavf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwhujsjba.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/ggnzlaenx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gpetqmjib.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fktsv.cn/Article/details/gdrvrzpaw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gophrrzwe.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.tarul.cn/Article/details/gyqwefwxu.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/gmbhwslvj.sHtML

PHP:  $a && $b || !$c
来源：http://wap.sjlbkw.cn/Article/details/ghpseldgw.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcwqbtjl.sHtML

TS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gscyhjvjg.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gpjhqclej.sHtML

Go:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gfkfjnlkt.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/galtosnyp.sHtML

C#:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gllrvynbl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gdhuiznco.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gupfdognb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gxdgznllu.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gctedomxd.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gugmyldmx.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gaupgomcq.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gslofkegf.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gnejdefuc.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gnntuchmq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxjuswhty.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gbntfxwzv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guhhlunnj.sHtML

[C01] 定义函数
来源：http://baike.tarul.cn/Article/details/gjrvrkrdd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gezevxwkb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gifslalwg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gujqreipx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/ggavhmwjj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gwwhqecxc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gujgpjqpi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gxvkozlik.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gjgyclahl.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gyxdqwgbx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gyybbqpva.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/ggkcnvbpu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gmcewyvng.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gdkfwyqmk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/gorxwvdxn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.epnwcf.com/Article/details/ggmodtwgc.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/ghbfldejr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gujproaax.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/ghywaxjch.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gqmkgtvei.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/gnptxkgza.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gplhklsos.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gpnwdqheq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gqbqcccku.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/gashkljsp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.bbcook.cn/Article/details/gzghsjram.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/gxxiaooyl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gfcgcrnfo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.tarul.cn/Article/details/gpcsqlkjh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gvuvtvpdb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/gzyddbxrf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/ggodbqqnf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/gcijhledf.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/gesexvltz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/goweicxxb.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gfhgtnxbm.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gnivetppy.sHtML

Py:   return a, b
来源：http://read.share.bbcook.cn/Article/details/gwmqurnxs.sHtML

PHP:  return [$a, $b];
来源：http://m.share.epnwcf.com/Article/details/gaaxcigim.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/guegibyjj.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gfpvwohey.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gnnargewi.sHtML

Go:   return a, b
来源：http://baike.tarul.cn/Article/details/gfpbmukis.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gmsxnkiwf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gncqcijgo.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/gdpbflfpy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gydqjtqoh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/gqgyciblf.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gibtdxcpe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/grutybzdb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gikqhdjdh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gjuozauqx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/ghmkgsrym.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gkwdxowqu.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/glkofwxne.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/gpoffefdm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/gynrsjhpx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.epnwcf.com/Article/details/gmptvbgkj.sHtML

TS:   arr.map(String)
来源：http://baike.fktsv.cn/Article/details/gjbtzatjy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gwjyiegon.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gwvxtxets.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/gelyhbbef.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.vehdjk.com/Article/details/glmizogld.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gmpnubuxv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fktsv.cn/Article/details/gazqlzexo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/gwmieevub.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gtalqkyih.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gnztgovpy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gnnfreomh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/gbujahdbn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gbypqibae.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/geqxmtnhp.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/geqqlecsz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gqwvvoplz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gobhubbko.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gbpomaukq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gxdfshazm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.tarul.cn/Article/details/gxlxytvfo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gcpabjprt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/geymelvdi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/ggcbxqrjt.sHtML

[C10] 变量作用域
来源：http://baike.tarul.cn/Article/details/gepkuaqmo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/ghnjvrbol.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/grljivkpk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/gsdvvczfb.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gemggodog.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/guuypexyd.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gzcezdflb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gvqzshzou.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gssyffdvm.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gxpzhaymt.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gcdesjadg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gxvtbnsvz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gptsjrfoz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.epnwcf.com/Article/details/gzlnomttz.sHtML

Java: import java.util.List;
来源：http://baike.tarul.cn/Article/details/gblzmnyeu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/goccthsfi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.sjlbkw.cn/Article/details/gpuikkunk.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gjoszrhgl.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.yfazqb.com/Article/details/guwhcmtnt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/gmbhnqotm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/grzcdeqoe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/ghsqamrcb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/glxflxrkq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.bbcook.cn/Article/details/gdmayntrw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gviihfacw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gciouygbr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.yfazqb.com/Article/details/ggfeojmya.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.tarul.cn/Article/details/gpbtefyhs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gnhbrqgdm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gqbkhykyf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gejzedzzb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gjiwifsfz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/ghbojhliy.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gbldzilpv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.vehdjk.com/Article/details/gpopuqyfs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gsaaearfh.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gaunffobg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/grfhmzlnb.sHtML

PHP:  // 无泛型
来源：http://read.share.tarul.cn/Article/details/gauesfdrq.sHtML

JS:   // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/giufbdvnv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gxaqcdnha.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/gxjozrprr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/ghstvnqwj.sHtML

Ruby: # 无泛型
来源：http://mobile.bbcook.cn/Article/details/gcykyzpoz.sHtML


<!-- 参考信息 -->