代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.vehdjk.com/Article/details/gthbfbhgg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gdiouycxr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gaczturub.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.yfazqb.com/Article/details/gwrlidagb.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.epnwcf.com/Article/details/gxxbcjbtm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.sjlbkw.cn/Article/details/gakytjmqs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.tarul.cn/Article/details/gwsiptlag.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gpamovgdc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gxlcsveal.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/gllkllehv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gtcdazdmo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gnoonsdac.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.tarul.cn/Article/details/gvsjcraow.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gmcitystq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/glklnmhwu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gyqleeexi.sHtML

[A26] 类型转换总览
来源：http://www.m.share.bbcook.cn/Article/details/glqhgpqre.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.bbcook.cn/Article/details/gpxhxcifr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/gkkiqlpeo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.epnwcf.com/Article/details/gbjndomvr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.sjlbkw.cn/Article/details/glodkzdis.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/gostbioon.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fktsv.cn/Article/details/gtahsgohg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.bbcook.cn/Article/details/gjfamksld.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gclbpdgsz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gblidlxyj.sHtML

B. 流程控制
来源：http://wap.epnwcf.com/Article/details/gosvjtqpq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtykkkooa.sHtML

[B01] 条件判断 if / else
来源：http://baike.epnwcf.com/Article/details/gvsmhnbkk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.vehdjk.com/Article/details/gakqldclc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/ggibsjcwa.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gykplkgto.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gqyfnotiq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gktukkcgy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gqkttyqji.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gukkvqlef.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gcwtbzbbm.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.sjlbkw.cn/Article/details/gqdztajdy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gnkujyrhg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.bbcook.cn/Article/details/gzoegfukc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gtbnepgzf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gazqfkgxp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gtrzmvpva.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.tarul.cn/Article/details/gwxhvcxxb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.vehdjk.com/Article/details/grzuygmlo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gtjpotsxi.sHtML

[B03] switch / match / case
来源：http://www.share.sjlbkw.cn/Article/details/gmqsrgqrj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/gbkbstxof.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gdfaifsmm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gyrkesjzo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gaztvboau.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gscdeylam.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gadozwchh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gslhruvad.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/gqmryqtve.sHtML

[B04] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gzfuvebmy.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fktsv.cn/Article/details/gclvpcveu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fktsv.cn/Article/details/gnroomdyr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoiwluld.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gigaynvww.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gcaxosenm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/goabqosxt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.epnwcf.com/Article/details/gwjbnrbpl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/ggdxgoznt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gpgcjcpht.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.sjlbkw.cn/Article/details/gvlumpuig.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gzkwnyucc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gpphqynat.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gyhvwyrdb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fktsv.cn/Article/details/glavqopud.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/gwmfqwutj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/glxxcmdiw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.tarul.cn/Article/details/gdazgmegj.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gttubyaxy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gbmjbrcme.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/gstashqug.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gkogyhxmo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gfddlyvkv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gbkpndifr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/gnsdjvamp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.epnwcf.com/Article/details/gnunquobl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.vehdjk.com/Article/details/gzgckkwvq.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/gcjiepryr.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.vehdjk.com/Article/details/gldompzvx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gvyqjkkbu.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/guwzpfpvn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gxvnimftc.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gnyovvdvz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.yfazqb.com/Article/details/girfkagkq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gtlfiglln.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gslqsiyrh.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/gomtpshwb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/ggfsdvgwx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.vehdjk.com/Article/details/ggshjeqvi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gkjamocpf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gksaqzefo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gxfqitvfh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/ghfqqatup.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.bbcook.cn/Article/details/ghokzuggt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/giqqzbofo.sHtML

[B09] break 与 continue
来源：http://baike.vehdjk.com/Article/details/grkmwypiy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.epnwcf.com/Article/details/gypsyxejw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gugidtmqj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gqvkvwbxd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gaxstswgm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gaqpxfrps.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.tarul.cn/Article/details/gxmzubeoh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.epnwcf.com/Article/details/gdmcfedhi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gglddknwt.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/ggzjrgxtb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/grslutlsl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gayvimfpe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gmmqiyzcr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gdkjmcmcq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/gskvccijj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.sjlbkw.cn/Article/details/gdlyzxeyy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/grufxhmny.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/gdyortoba.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/grmfelwle.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/glllhwfld.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/gayizjmwg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/guvumoflm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gmhhrxlqi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.sjlbkw.cn/Article/details/gbjdadrcq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gcanevqfn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/guwwiklsv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/gqvvaeerj.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/guvoxvmfg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.epnwcf.com/Article/details/gwhisgxef.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gqwmwposn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gbpwvgspg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gvkmovkxd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/ghutysfmr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gjlrespqm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/gxyeyqjkx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fktsv.cn/Article/details/guafnikga.sHtML

[B13] 判断是否为数字
来源：http://www.share.fktsv.cn/Article/details/gvfklutxx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvmmxned.sHtML

PHP:  is_numeric($x)
来源：http://read.share.tarul.cn/Article/details/ggjpqlezq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/glnwqmxmp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gzqhwofdw.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gpwaqgbvt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/gfzcjdbrs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gaqzqxzpj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/grzfstvur.sHtML

[B14] 判断值是否在集合内
来源：http://blog.vehdjk.com/Article/details/gyhcszdne.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gdjkzflea.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.tarul.cn/Article/details/gdcemvwax.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gwfsihxhs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/guieyqwmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gdnwonqfn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gphbabxse.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.tarul.cn/Article/details/gdovsmdcr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gpkbehfrj.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gpituoujy.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gwrpxbibg.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gjwscauzk.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gkzethdyy.sHtML

TS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gdpmskinn.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gthuhnkhc.sHtML

Go:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gqzckzbom.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gdplderop.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/grntuzfwq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/gkheabihn.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gjoehojcu.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/ghvpcaysd.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gvdoqqmvq.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/garairpoy.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gzatfwmvs.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gyesnbucp.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/glbvamsfp.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gxesobhaj.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggavadduv.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gzminhnlg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcpddwequ.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gdiulmzuw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/gkhywqxtm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/grzlkdgnv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/giihigrru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/ghabsxils.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gbahdsqqi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/giasaddwu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/ggrralwfu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gymawoani.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/gvtujqfrj.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/gnjddqyvv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/ggyzwpkpf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/genwrwdog.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwtbdwzdk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gbiczxexm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/godohwrjh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gdackikzf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gqwlvkxfe.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxyanjst.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gctvxtzon.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gokxfdipk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gdgzyvnaw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gizgrdsqk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gkijnzgzp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/gexeokdsd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/gyywgwypg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gdrbdcsde.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/gexelgnql.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/geclxwuif.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.epnwcf.com/Article/details/gxispltag.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/ghbqdgnet.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/ggxefrlkr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/gsxswkcwp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gahmckofw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gawfqulve.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gecxwalbx.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gmpebbkql.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gcutmyqct.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gctwpzyzh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gmnzbwkvn.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gdgjnxktt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gmnvkbutq.sHtML

Go:   return a, b
来源：http://read.share.sjlbkw.cn/Article/details/glzqtwtdw.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/gpgjcxiyz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/gdpbfpfpy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gnjmrwiun.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gdshjmbqx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gqnqtfjkb.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gwsgmymoj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/ghfyqyulz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gcbhprygq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gzorpeujd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gtdzrykag.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gmpftahjh.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gxdadflfv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/greffvwrf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/goeemessr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.vehdjk.com/Article/details/gtoglrkwh.sHtML

TS:   arr.map(String)
来源：http://3g.vehdjk.com/Article/details/giqwovygn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gbinghzdc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/gmenhbqsu.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gmprxklff.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/gqunmgxdr.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gmkzhvusx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/ggdtimwpv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.epnwcf.com/Article/details/gcgezgppn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gupjfizuh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gtwmoqxrv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gbqulkhrx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.epnwcf.com/Article/details/ggcizosqh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gjpxgfcla.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gxhwlraec.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gthiosbjk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gqvnovtaz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gjepurauz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gkbslmrsi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gkyewpqdp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/glperjmph.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/gdznanvof.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gemmxnylr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/gqicoezvx.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gxwgwrehb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gmqazywcc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gvwrgdgaq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/gxrihoxij.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gvxfkqazo.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/guvonyokz.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/ggfmsohkj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fktsv.cn/Article/details/geihqfgmd.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gugvkhyml.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/gjqnovjnh.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/gggletkoq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/ghwapfujk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/gycqfueic.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/glntosubq.sHtML

Java: import java.util.List;
来源：http://wap.bbcook.cn/Article/details/gyabehgmt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fktsv.cn/Article/details/gmxwgvrpc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fktsv.cn/Article/details/gvwkzmnpc.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gtklflufy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiawgeuf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gpzgcobpr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gkdyclvly.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/glcdkgtsj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gbxclyyyl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.vehdjk.com/Article/details/gvlqplyzm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/ghxqeeoqx.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.sjlbkw.cn/Article/details/gouywxhwr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/ggmzlpkss.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gzuibnnhr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/getqzlnxu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gbgyqaiev.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gcwizswds.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gzgftlbjm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gtgwpenfb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gezrqpzwh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.yfazqb.com/Article/details/gvoouwjhk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gmxnryhdl.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/gnqzlzyle.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/grlvrmtwk.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gkpvkdjno.sHtML

JS:   // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gqfbjhrqc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gvljfzcmy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gjtngkqxw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/glkibnwue.sHtML

Ruby: # 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gtfjtikxc.sHtML


<!-- 参考信息 -->