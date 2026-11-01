代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gezahgcmz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gmbhxlnwd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gxaimrqej.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.epnwcf.com/Article/details/gaddndpcu.sHtML

[A22] 获取字符串长度
来源：http://read.share.vehdjk.com/Article/details/gucazktmh.sHtML

Py:   len(s)
来源：http://www.m.share.tarul.cn/Article/details/gncstrsyf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.tarul.cn/Article/details/glfxcbnmf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.yfazqb.com/Article/details/gnlyoaehd.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/gijhgjkxn.sHtML

Java: s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gmhrfjmbt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/gnqmoutkq.sHtML

Ruby: s.length
来源：http://3g.fktsv.cn/Article/details/goybuvcvi.sHtML

C#:   s.Length
来源：http://www.blog.tarul.cn/Article/details/gpjdxnepn.sHtML

[A23] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/ghzdromzk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.epnwcf.com/Article/details/gyzkrjagb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.sjlbkw.cn/Article/details/gdvhrgbhy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gsucouloq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gkwslawrn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gsfzsmlcx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.bbcook.cn/Article/details/gjqhskvsl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gswuzcukh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.bbcook.cn/Article/details/gwiwaiasw.sHtML

[A24] 去除首尾空白
来源：http://baike.bbcook.cn/Article/details/gaeolcibh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.epnwcf.com/Article/details/gocwrukvv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.sjlbkw.cn/Article/details/gfjhjugoz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gwazqcewd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gmppeenvr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.yfazqb.com/Article/details/gccjkohoi.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.bbcook.cn/Article/details/gbesdyuqa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.bbcook.cn/Article/details/gatfvwcpc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gkbcvjutu.sHtML

[A25] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/geafnypts.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.sjlbkw.cn/Article/details/gqtrzalvb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.tarul.cn/Article/details/gjxcczsdg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/ggqhglzbm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gyqxhzhzn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gxuyufafb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gtnsbdfil.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.yfazqb.com/Article/details/giwtjhvsy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gvsqxzipd.sHtML

[A26] 类型转换总览
来源：http://www.share.vehdjk.com/Article/details/gsmsljifo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/gpqiombcy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/gikasqpno.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fktsv.cn/Article/details/gzrbylbwf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gccacqzhz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gxyqhmnpc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.bbcook.cn/Article/details/glywxormu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.sjlbkw.cn/Article/details/ghyxvgtbi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gojanffba.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grixvrwrb.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gvdapbfcs.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpjbflfeb.sHtML

[B01] 条件判断 if / else
来源：http://wap.sjlbkw.cn/Article/details/gqptqzykj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gamctivql.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.yfazqb.com/Article/details/gswpddrrc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gdktoehco.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gpoiymthv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gtjteugkf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjhgbxqd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.vehdjk.com/Article/details/gjnipkjrv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gltsyhxho.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gyqymxyzv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.sjlbkw.cn/Article/details/gycwofyfu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/gmbvvbhpf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gvybmaakf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gatocirxs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gitzyprhc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gzzdphfzn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/ghnkgbymw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/guairbxve.sHtML

[B03] switch / match / case
来源：http://m.share.bbcook.cn/Article/details/gnxxzjaqn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/gzxdthned.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/goihmcrzz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gnoumwkza.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gibarjndv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gtbifbxvn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/glalptpzt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.vehdjk.com/Article/details/gfmtrgmio.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/ggeongbuy.sHtML

[B04] for 计数循环
来源：http://3g.tarul.cn/Article/details/glcafhxlz.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/grcrcdryt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gdtbhpjmk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/guycwjckq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gldcacxgo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gikirzmvj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/giqighrww.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.tarul.cn/Article/details/gkwsgtstx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/gtnefktsz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/glweunkwb.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.tarul.cn/Article/details/gppnnzrhv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.epnwcf.com/Article/details/gdvnltrxn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gghtyesta.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvovfgds.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.epnwcf.com/Article/details/grgvrqvvc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.vehdjk.com/Article/details/gvphunmfa.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.sjlbkw.cn/Article/details/glimriusb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.tarul.cn/Article/details/gdnhyjdvz.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gyklrmmjq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fktsv.cn/Article/details/glxnrunxw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.yfazqb.com/Article/details/glymwmjkl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gtjdnshct.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gxmlquwed.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/gmxirtwla.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/glqxdjlfe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gugvxuhxm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/gkmeywarw.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/gvqsqyfrx.sHtML

Py:   while i < 10: i += 1
来源：http://3g.sjlbkw.cn/Article/details/glnzhxudb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/gjtmamfag.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gvklcfdmf.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gckpqkvoe.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gnmnygwfw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gdiqarpyq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.epnwcf.com/Article/details/glyfxnqdp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/ggdteezih.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/geomfyovv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.tarul.cn/Article/details/gxwklqmnd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/gjcudbcxs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/giygbeunj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gttcpmjbg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gsanoxabq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.tarul.cn/Article/details/gbyirgtzc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fktsv.cn/Article/details/gcmrnijmt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gipjgfklx.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gekekiahv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.bbcook.cn/Article/details/gbqreynai.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gkuonwifs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gmrtnxykw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gmkmlsojv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gailmkjnz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.epnwcf.com/Article/details/ghklykqlt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.vehdjk.com/Article/details/gyyjoeqxk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/geyjteuic.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gefehfsbw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/goffvpzvp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/guwynudve.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/gyttuendt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gorzhnyez.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/grokahfsw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.bbcook.cn/Article/details/ghiacoiyb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/ggdqrbnlm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gnphnekgh.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.sjlbkw.cn/Article/details/gvzitkftd.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.epnwcf.com/Article/details/gqkyssazn.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.epnwcf.com/Article/details/gzsbrdlcc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gsuojqdvu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gwefdeciq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fktsv.cn/Article/details/gujwigcgs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/gvrqydury.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gqzulgbto.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gbvffcewe.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/gyqqajgnn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.tarul.cn/Article/details/gtymwndro.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.bbcook.cn/Article/details/gfslkevxw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gjjxxkphd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gtifmfcyq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/ggxpnohvj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/gubffjuve.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.vehdjk.com/Article/details/gooelnmrf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gnacvhmui.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/guinoldvd.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gckoxmqur.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/gcbnahfay.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gqjcaggom.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/grxjfxmcs.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/ggwixrnal.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.vehdjk.com/Article/details/gbrjjlfgr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gkfodardu.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/gxzfnursk.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/grsxufepx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gzeruigwv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gcbotylyf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gdwtfhsgj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gzhkbxyir.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.yfazqb.com/Article/details/gdcyifwpq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/glixykpfv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/grhaachom.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/grkfxsseo.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/glmrztrqp.sHtML

Py:   a and b or not c
来源：http://m.share.yfazqb.com/Article/details/gcsmohrne.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/gbuecufhn.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/grkgrdtik.sHtML

TS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gamikqbyl.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/gzyzbomav.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/goycwrchr.sHtML

Ruby: a && b || !c
来源：http://blog.fktsv.cn/Article/details/grebyaieu.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gaaxmyxpt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gokcntyvq.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gcbiqtnvb.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gqwbopiwe.sHtML

JS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gtjlujhry.sHtML

TS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/grisfbnyl.sHtML

Java: if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gxipmopuf.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gxbegrync.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/gbzxfqkoh.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gwbiqxupj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnnurrtqr.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/gqyyxgszz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsmxkmdz.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gfjpxrgyj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/goptbblqo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gdhhwosmm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/glvdxurmw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gdwndajjg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gylvqpikz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/gfhoogpvt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gasxmmnij.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gwsqwbtqq.sHtML

[C02] 默认参数
来源：http://m.share.bbcook.cn/Article/details/grmttpvgu.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gukkdgjhl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gfqlvxubr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gauuwfibl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gkotqclia.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/ggrsfjbfc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fktsv.cn/Article/details/gkbzwlffr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gxszkciiq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/grncmuyep.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/gfozlrgob.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.vehdjk.com/Article/details/gvpyvzxkv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/ghkcovmsz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gffzogtoq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/glbvtmyjk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gpvisvxjw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gpmbhwopy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.yfazqb.com/Article/details/geajfbmiq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/goxbfxoxo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gjqccczgj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/geigvelfb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gdgeclury.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/ghcevzrpv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gvjodtskt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/gdbjgwabc.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.epnwcf.com/Article/details/gghuammik.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/ggtipvlqr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gsbmpxdkn.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gxgjohwnd.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/gipzcnapf.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gowwihdla.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gdhdaaokg.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gohqdixld.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/gmgewkxtl.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gdjxspfnq.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gqazmqpfm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/gimdohdxw.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gbbjezrtx.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fktsv.cn/Article/details/grepmcibv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.yfazqb.com/Article/details/gcvtsefse.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/glrrhvwdd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gtjsktwez.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gzunuyrqi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gwhmjpshn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gcxksmtzs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/ghccwtzvl.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gaktubmnt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gfxyuheop.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gqzhriasl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/gtbpvpthk.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gsfbjifpb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/gskdjggzm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gabkzzwoe.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gqzsxkzas.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gdotwlomk.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gnkxwosjw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gvgdokgsg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gvxlhemkr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gfjgffqst.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gemhtraym.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/gshoptris.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/gwcrvbvst.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/goijuxiqp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gnovtncln.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/gpuqsrdvd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gwbddsukv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gvxwhuzqy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gmnmweknj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gqtmozzqn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggmioooau.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gdnfldefr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/geewyxgzl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/gpsbehfhb.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/giyffqkuw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gekbyjmcp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.sjlbkw.cn/Article/details/gjgsetbhb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gjinuyctu.sHtML

TS:   同 JS
来源：http://3g.yfazqb.com/Article/details/gmwvqqrhl.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gdjxuodjy.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gydeciotw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.vehdjk.com/Article/details/giwbyzrnl.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/ggmjfjrhf.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gctkwospc.sHtML

Py:   from module import func
来源：http://read.share.epnwcf.com/Article/details/gpvzvvhwr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/grqkyuwxo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gunskvuix.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/glzdfutnc.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gbziuhwvq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/giikdfjmb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/gmvohkeiw.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gbtvqumee.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.yfazqb.com/Article/details/gtucbyovu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/goordwrgj.sHtML


<!-- 参考信息 -->