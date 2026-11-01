代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.epnwcf.com/Article/details/glkqwdlkr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.yfazqb.com/Article/details/glnfdkruf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.yfazqb.com/Article/details/gnyfejhwq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/glekklnfk.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/gldljrbai.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fktsv.cn/Article/details/gzurbkxmq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.tarul.cn/Article/details/gawoinblr.sHtML

[A25] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gpggjyjsj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.yfazqb.com/Article/details/gbomhjxmu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.yfazqb.com/Article/details/gwqtphfjo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gbhbsdopa.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/geikxyyfc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fktsv.cn/Article/details/gdcvkvnai.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gfcgavlmw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gqappgaeo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gfdazahah.sHtML

[A26] 类型转换总览
来源：http://www.m.share.sjlbkw.cn/Article/details/glvtgkjqb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.bbcook.cn/Article/details/gjerctitv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.tarul.cn/Article/details/gxlzeqebw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.sjlbkw.cn/Article/details/glmunrpzl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.tarul.cn/Article/details/gsntgkaay.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gpordwwge.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.sjlbkw.cn/Article/details/grxkazseq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.epnwcf.com/Article/details/gazlqucmd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gsnwxhfqr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggaxqmnvh.sHtML

B. 流程控制
来源：http://wap.epnwcf.com/Article/details/gusfwvykh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzjmoteqa.sHtML

[B01] 条件判断 if / else
来源：http://3g.tarul.cn/Article/details/gtaejjvom.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.tarul.cn/Article/details/gnexouhjm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/givwslvod.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gdtqzywil.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gcdvtnegc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gfptbtdyx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/gygeviytb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gnlhlixit.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/guhhdmajy.sHtML

[B02] 多分支 else if / elif
来源：http://3g.yfazqb.com/Article/details/ggrxvlxan.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/gusifhdxx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gmiswiltq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gqgbympxy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gsgqybjav.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gjyexlbnl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.tarul.cn/Article/details/gzctqvmiw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.bbcook.cn/Article/details/gsiubydcv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gliijjmwf.sHtML

[B03] switch / match / case
来源：http://read.share.epnwcf.com/Article/details/gkctycnpc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.vehdjk.com/Article/details/glkvoqwax.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/goketeskf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gyfihevuu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gqazpbvtl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gskwifzwg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gpjfbbejx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fktsv.cn/Article/details/gsejspszd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.bbcook.cn/Article/details/grjmxnebg.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/ghixroprk.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.yfazqb.com/Article/details/gmitfvxqk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/guzqnazzz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gmmfpriwi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/gocfawyel.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gnsgjzmdo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.vehdjk.com/Article/details/gyxcrulfz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/gtqalbtwt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.bbcook.cn/Article/details/gkhemzjyh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gsshlodgk.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.epnwcf.com/Article/details/gocollutt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gltvpappf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gnrvebutb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gwbnapcyj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gmrvozydp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/gykjumgaj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.yfazqb.com/Article/details/gdoxoaffo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/glyxlfnel.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gosakvyof.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gaerssbkk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gdkzhbpte.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gftzbugwk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gtgiaebgi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/guivdqilv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/garwjqdxk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.vehdjk.com/Article/details/gdxogpvnh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.vehdjk.com/Article/details/ghyhabbos.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/gjlizzssm.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/gyjmqaeiz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.bbcook.cn/Article/details/geystsuti.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gacdkgzdy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gfsmqxfeo.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gjwasxwzr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/gzwjjvsue.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.sjlbkw.cn/Article/details/gkpayhlgo.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gvarvbxhl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.bbcook.cn/Article/details/gbuahzjvm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gbnjatwth.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.tarul.cn/Article/details/gjkgclvkd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gbznjtwqv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gmjvfmwbz.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gafrhyjpb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gxzkattix.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gpojzazws.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gyligimzx.sHtML

[B09] break 与 continue
来源：http://3g.epnwcf.com/Article/details/gfuxtyopg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.bbcook.cn/Article/details/gmszkcahd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gnkavvzkb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gnylhczjd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gbirkioqf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gkrzvkrju.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.vehdjk.com/Article/details/gulaonkcf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/ganqjexsc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/geyrrwjme.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gzbtzdmzh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gmrjpjkle.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gtsrlgibv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gdhtwjcgn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gphsmfodt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.yfazqb.com/Article/details/gwmpcqocg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gmxhrlszd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.tarul.cn/Article/details/ghskdmkdc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fktsv.cn/Article/details/gyhlchmla.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/gyobmqgpe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gllhcugnd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gwjggvavb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gypkdcqdg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/goctmtnnu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/gtiejywbt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/gtpkbmrrg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fktsv.cn/Article/details/gvfkhnjls.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/gznrnimts.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/gliccjvbd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gopympkyn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfzcnvmq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gqdtpopzh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gbksgsstc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/geegcquyj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.sjlbkw.cn/Article/details/gyjjnoiqs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/goqemfkyd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/guhawyasd.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/gmqtvwbdc.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gzcgeeadz.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.epnwcf.com/Article/details/gchqzllei.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gdftpeela.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gavvqnjlb.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/gpgsbelkz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gfaiczzqi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.bbcook.cn/Article/details/gkreveccd.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/gajvkwzzu.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gniuuatlo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/goccxfuqy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gjjvdjblz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gfvpfpdcj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gffntihzd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/gpsjrsqoi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/gzeztvwez.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/gjboqnqxq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gvkqovrzt.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gcnvdkwlo.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/gckcfkumd.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/ghyxcboyq.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gfbdsokhx.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/galjnvanm.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gakkybscu.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/glwegmaga.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gniobvzff.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gbcagrzyo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gfgvcbzwj.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gwnbsvaxg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gfvprmftg.sHtML

JS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/genydbwsf.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gzfkoriyz.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gulhgtnoa.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gaxcdnvfw.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gdncutyiy.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gniljmmhg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmuugwvzd.sHtML

C. 函数与作用域
来源：http://read.share.yfazqb.com/Article/details/gzdpylugz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcxmvkqga.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gfncwgroa.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gntxkiwiq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gtcjdgjcd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gaepianhp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gayjlzwth.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gimqujhxw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gqdwzampb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.bbcook.cn/Article/details/gdqoybwjp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gntchksmc.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gmlusmuzx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.yfazqb.com/Article/details/gctebtekq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.tarul.cn/Article/details/glpsbmadz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gqobzropk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/ggnkmjkce.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.vehdjk.com/Article/details/gmmsjzrdt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gnoqekvzs.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/ghsuvxgmp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/ghccwcxvf.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gdcymekwi.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gfjfycwsd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/gxgjjnlvf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/ghuqknxzi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/glhnrubzp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gjwrbmvmi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gjdjvaizx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gscikfrca.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.sjlbkw.cn/Article/details/gdemlozwt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gkdixevfx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/geydmnltf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gqrcqztur.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gahtmhaue.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gewcsgjdm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gxxrjzgqh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/ggwshkiio.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gjxnnqbnb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqluemyu.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/grxfrafjn.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gewaolwfd.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gbjesjwvr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gyswalsro.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gobhizzpu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/gebzskhvz.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gubkaixnq.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/grcznetvq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.yfazqb.com/Article/details/gzfzverlq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/gaznwpoie.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.vehdjk.com/Article/details/guzicssmk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gmxqtncwi.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/givovlmsf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/giyojeowz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/ghgxaqjgz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gjdhzwoek.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gjivnkquk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gqgsgyova.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.yfazqb.com/Article/details/gxvfktoia.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.vehdjk.com/Article/details/gqhqrfhcg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/ggucybvqp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/giasuaole.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/ghjjqsqxb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/guldnjail.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gclbzuqia.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/gikzhcvwk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/ggckslmef.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gnqetskmi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gzwfqortg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/gqihtyajd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gwxnzkmgj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gxjdhhbjy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/ggwwrdeng.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gamjvahmp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.yfazqb.com/Article/details/gszjgwsvx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gouxrxoia.sHtML

[C09] 递归
来源：http://www.m.share.vehdjk.com/Article/details/gxsetjywu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gczqshdmw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gqthbdngs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gikuorvek.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/glewxlsco.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/gdccfdbry.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gcnccmgqd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gdfanzbcq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gcbayncvx.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/glxhjokzt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/ggysybahv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.sjlbkw.cn/Article/details/gnoglfgkn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gnwmhaccf.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gsjgnxwtd.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gsyjwswwa.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gftlftofx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.tarul.cn/Article/details/gskcifbqb.sHtML

C#:   块级作用域
来源：http://3g.epnwcf.com/Article/details/gfwahokks.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gdvfzsxms.sHtML

Py:   from module import func
来源：http://mobile.bbcook.cn/Article/details/gqioxofbt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gqjqkuusi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gqhhvtere.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/gukvsrhbb.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/givpidwqe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gpzgbvdbk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/gluhpaems.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gscbuayoq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gnmqjopfk.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.vehdjk.com/Article/details/gyvctaeph.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fktsv.cn/Article/details/ggcfmbyte.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gdmzfuwvc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gvwskcpqj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.yfazqb.com/Article/details/gfxfranvm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/gzhmjokdu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/goqnvncot.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fktsv.cn/Article/details/gmxhyzusk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.tarul.cn/Article/details/gjznvljhf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/goeodzoop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gyromsnbc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/ghrpndfoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gbvmtlycl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gmuveaens.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/ghlnlfblc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/gphiiwkkl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gjiokslwp.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gmavavjgd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.epnwcf.com/Article/details/gmkrnjotf.sHtML

PHP:  // 无泛型
来源：http://3g.bbcook.cn/Article/details/gnjcsowus.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gjfjiqpzc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.tarul.cn/Article/details/gaydxodnx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/ggzragxka.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.bbcook.cn/Article/details/gdgcjzara.sHtML

Ruby: # 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gurmurkmv.sHtML


<!-- 参考信息 -->