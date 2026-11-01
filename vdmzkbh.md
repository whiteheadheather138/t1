代发 wailian999

C#:   s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gebkbjcsr.sHtML

[A23] 大小写转换
来源：http://blog.tarul.cn/Article/details/gkotzxdrk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.bbcook.cn/Article/details/grdhvcgrx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.bbcook.cn/Article/details/gcbgqvpuj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyupgggzj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gpkeapvzd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gtcxwwhxg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gmxmzjhem.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.tarul.cn/Article/details/gllnjifmy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/grgipmlcr.sHtML

[A24] 去除首尾空白
来源：http://blog.vehdjk.com/Article/details/grqvldfhl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gookkbejg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.tarul.cn/Article/details/gawvcggxf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/gbfcmplgl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/getjvpoxv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpsfutbt.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.tarul.cn/Article/details/gmnlsyxlp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.vehdjk.com/Article/details/gdvenawiz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fktsv.cn/Article/details/guoxgomxk.sHtML

[A25] 字符串比较
来源：http://blog.epnwcf.com/Article/details/ghnagwbdv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.yfazqb.com/Article/details/gcfmszngj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.bbcook.cn/Article/details/ggyqyoolb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gabycrsht.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gbgavautf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gkujbptcu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gfgiizlpw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.yfazqb.com/Article/details/gioqesrqm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gmamnbgqr.sHtML

[A26] 类型转换总览
来源：http://www.m.share.bbcook.cn/Article/details/gxmlxyvtc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.tarul.cn/Article/details/gikskweeq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.bbcook.cn/Article/details/guvtpqyxp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.yfazqb.com/Article/details/gevkbploi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.vehdjk.com/Article/details/gnxrtonnj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gvgfnbelp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gthjyptvq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gtabnwssd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gpyhrfgvm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gltrdgqju.sHtML

B. 流程控制
来源：http://www.m.share.bbcook.cn/Article/details/gscrjfztz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcazzqdkn.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/gqfwrxzus.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.epnwcf.com/Article/details/giiuukaqc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gumbzhdll.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gqijajclb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/ghdyzlgda.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gofymfomg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gtjofvocv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gagnqpbkm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gmtnjjajq.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/gztfpogdq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.tarul.cn/Article/details/gzvtfirar.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.epnwcf.com/Article/details/ggesallte.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gqwsgbxte.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gaglrebir.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gdkkapkta.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.bbcook.cn/Article/details/glsvikimu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.epnwcf.com/Article/details/gjwrtqgfc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gckiuftmt.sHtML

[B03] switch / match / case
来源：http://baike.bbcook.cn/Article/details/gnhbmnchj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fktsv.cn/Article/details/gmxxxdqjo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfamjxqwh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gtmrkqiap.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gcvhpkgob.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gqrvwvsuq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gidkwgcxc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fktsv.cn/Article/details/gfgzomlxj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.yfazqb.com/Article/details/ghbligwed.sHtML

[B04] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gfsjpsmys.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/gxwvpmznu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.tarul.cn/Article/details/gjhualunn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gqjdkosyn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gvrlvkjtm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gafnvdogg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.vehdjk.com/Article/details/goqpvnsyd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gbrsetmfj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.vehdjk.com/Article/details/gddrhjmnq.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gaffyevhm.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/gnbsxgesm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/gwavoxikm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gpgqyuzkv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gdeuaywqe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.tarul.cn/Article/details/gbkwibxef.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/glpvvgxac.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.bbcook.cn/Article/details/gybfhongd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/glkxaqszt.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.sjlbkw.cn/Article/details/gvtdzarpd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/geltdsmvu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.sjlbkw.cn/Article/details/gmdcylsvw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gpojrtgly.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gxhdxhzkx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmazjtkv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/gnkmjhzzq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gppdqrpfb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/gaunygniw.sHtML

[B07] while 循环
来源：http://wap.sjlbkw.cn/Article/details/gzincijyu.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtyujrqy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.vehdjk.com/Article/details/gbwzdyjtb.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gryrmkipb.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gpffdxwkp.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gcuotuatl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gjvcoxqjf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gmiofhais.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gbnypewzd.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gdxyinxea.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.yfazqb.com/Article/details/gfgfgkonh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.bbcook.cn/Article/details/gqwiqseit.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gobkhwawh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gtluvyxnq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gcngyhijy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gcrnhnlol.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.sjlbkw.cn/Article/details/gpykeueao.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gzbzptote.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/gsgfhypek.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gfdhnptom.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gychrqtta.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gplqadmcd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gjzfqzgym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/ghviauhek.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gdowgzsjs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gpmupxuga.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gesnrousr.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/gxbnfvvsf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/gjmjhqjlx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.bbcook.cn/Article/details/gebremnvs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/guuykftis.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gecklewhs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fktsv.cn/Article/details/gjevqphmg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/glibekpcc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.epnwcf.com/Article/details/gftlxsmes.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gekcdpiyz.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gxnukrhlf.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.yfazqb.com/Article/details/gulrhkxhs.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gsbttmjyx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gzmblhxbf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gfmugfehq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.bbcook.cn/Article/details/gdnxqlzvu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.sjlbkw.cn/Article/details/gjlgbgnao.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/gxyymyuzb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/ghrejtrzd.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/gnrvrpugq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/ghdyfogjx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.tarul.cn/Article/details/geewobctw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/glewqvwfp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gmjsqoccn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gslcccfkc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fktsv.cn/Article/details/gcoukttxe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gbuowllhb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gtbqlhfur.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/gukywgsyu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/gkvbmcfwf.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gbsauiuut.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/giutplkdz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/grqxcbxvx.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/gpkylyhpd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gkdpkyqdv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/getrgunzv.sHtML

C#:   x is int or double or decimal
来源：http://read.share.bbcook.cn/Article/details/gqriiejfj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/gztqahmqy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.yfazqb.com/Article/details/gspdkztlm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.vehdjk.com/Article/details/gpibxccma.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gifyatmut.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gonyafktn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gczdqadrn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gtqlzoyaf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/geavdpjaa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gcdktviey.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gdegmqugw.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/getzhgyiv.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/glgsoiqwr.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gpvbnjxir.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gqvndwhlv.sHtML

Java: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gdsucldzk.sHtML

Go:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gugxlwgrk.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gsbmswkbd.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gvegrnbzb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/gesntkhgd.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gxsjofryk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gajisxnzh.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gpipbmvhk.sHtML

TS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/ginplkgkb.sHtML

Java: if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gvybrndnc.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/gfhagwpcw.sHtML

Ruby: return if data.nil?
来源：http://baike.tarul.cn/Article/details/gnybnixlu.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gktenmaio.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwycbwrst.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gdscqhaad.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwlidjbnv.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/ggrsjjeas.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gecvbqile.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gmtqcaohw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gzbtebtfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gltqvpgzq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/guiqaaxad.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gecimzuoj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gqgtydznn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gqgpljwpy.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/glnmepghf.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gxcthzdnv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gihyoaowb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gwtwdeymy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/ggfurvpcc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gpstskmnw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/ggearlhjx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gbaepulqd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gbeesegtr.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gyduwrggk.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/grzdkctkq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gnezggprr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gmrnaygjb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/glquakhim.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.epnwcf.com/Article/details/gjeaublry.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gdjkztsrl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/galvxybtr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/gmhihtfwz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/ggscpmhyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gezrfnudk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/grwnnajtf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/ghfmhmktn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gfpkorxiw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gnzhrcwpc.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gvvaokvzs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gltwnmadx.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gqnnwarri.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/glqecywda.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gxliebdse.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gfegwguvm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gizlrgkrf.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gxipytndi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gihuacyhb.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/glfpgwouz.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/ganhptjzx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/ghvdyetdx.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gwzqynslw.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/gfxkmxvjc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/gbbulbnuc.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gpzadnfuu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gbxliatsn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gdubvkgwx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/ggtofimsj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.yfazqb.com/Article/details/gudpmqegz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/golayxnlz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.bbcook.cn/Article/details/grdfaurwp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gaghwnwee.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gdyrajtjc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gkpcsmckp.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gzzfniueg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gpcvumswz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.vehdjk.com/Article/details/gijznlfkv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.tarul.cn/Article/details/gqnxgnwip.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/gctxanbso.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gtqvlswgx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gwbcpquiy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gxvbdayzi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gpwrkxhzz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gmwfnrcfa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gvtxmvfdv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/gnellvqjg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/gtmffsrth.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gryilruqr.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gvocpnraq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gucocsnzk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.bbcook.cn/Article/details/goihftsje.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gxjnmezyf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/ghpbhtjwd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gygsndzib.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fktsv.cn/Article/details/glrvxezyl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzbsufosc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gculwskko.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/grrrusnfy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.tarul.cn/Article/details/glnkbrvba.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gynkkihdq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gssmkvrwn.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/grnixfmvx.sHtML

Java: 方法内为块级作用域
来源：http://wap.vehdjk.com/Article/details/gbszaezuv.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gvdyinvml.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.bbcook.cn/Article/details/ggroindqn.sHtML

C#:   块级作用域
来源：http://3g.epnwcf.com/Article/details/gtiuyvgeb.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gurejvivy.sHtML

Py:   from module import func
来源：http://blog.vehdjk.com/Article/details/gdjnquhek.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.yfazqb.com/Article/details/gduwdqsno.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gehpmqmbn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/gfuqbmcsd.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gslydpaog.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gwgmhqwve.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gdejvdosw.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/ghxdftmvr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/gaduyubig.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gyujyhkhj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gocdulyjh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gxcgovksz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gitatohms.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gihdozrgs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.sjlbkw.cn/Article/details/gwdolneqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.vehdjk.com/Article/details/gekeucpfi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.yfazqb.com/Article/details/gyeiwijwo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.vehdjk.com/Article/details/gxnyebtkw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gcqdouemb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/ghudmvvsg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gocynofap.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gbhbgzafa.sHtML


<!-- 参考信息 -->