代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/ggamiumay.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.tarul.cn/Article/details/gauiaejbq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.vehdjk.com/Article/details/gwvgquylb.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fktsv.cn/Article/details/gmnxthgcf.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fktsv.cn/Article/details/gbvfffjoz.sHtML

[A19] 交换两个变量
来源：http://www.share.bbcook.cn/Article/details/gwpmdszxk.sHtML

Py:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gzygezdio.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.tarul.cn/Article/details/gtwfjyulk.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/glucczcga.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gjxnqasew.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.epnwcf.com/Article/details/gmkycxlhp.sHtML

Go:   a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/ghfvrbisp.sHtML

Ruby: a, b = b, a
来源：http://wap.vehdjk.com/Article/details/gmeiekvpd.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/glyoprkto.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/gjlfuexcy.sHtML

Py:   name = input("请输入：")
来源：http://blog.sjlbkw.cn/Article/details/gbcvbzbkv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.sjlbkw.cn/Article/details/glqfahlis.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.bbcook.cn/Article/details/greflsome.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.vehdjk.com/Article/details/gxsyebcpv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.yfazqb.com/Article/details/goukqqabz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.epnwcf.com/Article/details/gpmxqseir.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/gfyitvwcx.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.tarul.cn/Article/details/gikoigyza.sHtML

[A21] 保留指定小数位输出
来源：http://blog.tarul.cn/Article/details/gusywnjcn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.tarul.cn/Article/details/godhtfaqq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/guonbwiqt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gvjpzdgxx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gdyslhngu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gjyipacrn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/goruehfme.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gmcysjhyp.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.vehdjk.com/Article/details/goorplnct.sHtML

[A22] 获取字符串长度
来源：http://m.share.fktsv.cn/Article/details/gctkgfmfe.sHtML

Py:   len(s)
来源：http://www.blog.yfazqb.com/Article/details/ggwkrwahi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/gbfwblwty.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.bbcook.cn/Article/details/gcbcqoxbn.sHtML

TS:   s.length
来源：http://wap.vehdjk.com/Article/details/ggapirzjz.sHtML

Java: s.length()
来源：http://m.share.vehdjk.com/Article/details/gosumxcgh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fktsv.cn/Article/details/gmgoyszew.sHtML

Ruby: s.length
来源：http://baike.fktsv.cn/Article/details/gbzlfljcs.sHtML

C#:   s.Length
来源：http://m.share.epnwcf.com/Article/details/gmexkpdow.sHtML

[A23] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gkcjbcqpd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.vehdjk.com/Article/details/gnbhbhcmq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.vehdjk.com/Article/details/gufrvlcdd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gepwkejoj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/ghadkwkcm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gwjhymqhx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.bbcook.cn/Article/details/ggoqomneq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gervkkkym.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxubiwre.sHtML

[A24] 去除首尾空白
来源：http://m.share.yfazqb.com/Article/details/gaggusksz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.vehdjk.com/Article/details/gpkeporou.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.bbcook.cn/Article/details/gqnejtyzu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gvzfwxtez.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gjntdluhs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.tarul.cn/Article/details/gvrvtmgdl.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.yfazqb.com/Article/details/gvqyqkolg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gyxqmgwvd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/geisrnayz.sHtML

[A25] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/giungjxaa.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.epnwcf.com/Article/details/gqeioexya.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/gcjcdjswf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/ggbbolhdf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gdnfnrsqv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.tarul.cn/Article/details/gffhrkxjf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gvatckhvh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.tarul.cn/Article/details/gyxijndtk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/geouiuioe.sHtML

[A26] 类型转换总览
来源：http://blog.sjlbkw.cn/Article/details/gxnfazfiu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.sjlbkw.cn/Article/details/gfekpnjem.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fktsv.cn/Article/details/gojuvupze.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.sjlbkw.cn/Article/details/grtgacphd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gckdoubei.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.epnwcf.com/Article/details/gucvvmwkg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.sjlbkw.cn/Article/details/gzqlwoujp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.bbcook.cn/Article/details/grenvosjg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gcdsyvmft.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grfjskobt.sHtML

B. 流程控制
来源：http://mobile.epnwcf.com/Article/details/gdgdekydt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmkywfwxz.sHtML

[B01] 条件判断 if / else
来源：http://3g.bbcook.cn/Article/details/gsovzqznx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.vehdjk.com/Article/details/gtkajgzsa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.yfazqb.com/Article/details/gylduqwyw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gqqvqwbxf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gubbarkoh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gmkzbhtyr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.yfazqb.com/Article/details/gpeyqmipf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fktsv.cn/Article/details/gfsxwlzwd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gsiuvkpdp.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.sjlbkw.cn/Article/details/gyxjufsjv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/gnbiiomtm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fktsv.cn/Article/details/gvdururoo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/grtgjmonw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/ghlqfvyks.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gxfwldeya.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fktsv.cn/Article/details/gstfqadgd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gahyzlysv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gcdgthjcn.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/gromcpupa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fktsv.cn/Article/details/geoafyhrz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gvjylrvwu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gbpxsuaxd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gpdsjorhw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gzleokdlw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.yfazqb.com/Article/details/guvbkslhr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.yfazqb.com/Article/details/gkeoqmxie.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gkegoivjm.sHtML

[B04] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gdlbgstcv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/ghaxhkqor.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/gricsfnne.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/gssopfxow.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gmtrcmmua.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.epnwcf.com/Article/details/gqjkvxxlm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/glaafjmsi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.yfazqb.com/Article/details/goomxmgpy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/gfjetmihr.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fktsv.cn/Article/details/ggmjyyceu.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/gdmomkdaa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.yfazqb.com/Article/details/gpppvjqhh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/glddfjtkz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gbrzholmo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.tarul.cn/Article/details/gwdrnxvjo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fktsv.cn/Article/details/gjualyzok.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.bbcook.cn/Article/details/ggosqehqk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/gomfmzhwj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.vehdjk.com/Article/details/guikigdfd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.yfazqb.com/Article/details/giujmisjy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gvlwotsvr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/gheofqxkm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvtuaxjbi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.epnwcf.com/Article/details/grtgszbiv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gjljzqchr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.yfazqb.com/Article/details/glplapcbx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/gzidmqech.sHtML

[B07] while 循环
来源：http://www.m.share.epnwcf.com/Article/details/guvgmpoqu.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gdlvolzzh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/giyvqqrdj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/ggpwkekfy.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gutgvzenp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gproanyad.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.sjlbkw.cn/Article/details/gxujhylbd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/gsvycsykg.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gvjkxpdaj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/gpkeketoj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/gvauitonc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.bbcook.cn/Article/details/gcneugbqb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gpvngtvcd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gmkixopze.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gjbmqmfjq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gbkolthxs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/gcomcyvrk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gknplvuok.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gsklkusii.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/giilpdrdu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gpcmyiiqj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/groeibebj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gcpxufodr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gnjdtmvdx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gunencvod.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/gqbnktvmh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/geqotafnt.sHtML

[B10] 遍历同时拿索引
来源：http://baike.tarul.cn/Article/details/gpyyxomow.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gasdbzpio.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gtsszhzhp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/ggmtnpsir.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/glcuiwbov.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gizbrjitp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gqutsvvyh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/gdqhbvnqt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/galoatzrv.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.sjlbkw.cn/Article/details/gkxkgzajo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.epnwcf.com/Article/details/gdaagygpr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.epnwcf.com/Article/details/gzypzxslg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gedezmhzq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gcizmettr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gosbdohrd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gtctbudbx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/ggebalyoe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gmxsoargl.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gclajnaal.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gynrheime.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gdxuofgal.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gnpacmsji.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gkxxmzhln.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/goeutjwji.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/gsoyyutlz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gcgmnwujf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gzfgqkccb.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gziewjmmg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gtfdtjsby.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.vehdjk.com/Article/details/gikgynins.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gvaqyinsk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gdcaswway.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gjnziwuve.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gjfiglkph.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/gpssbqqfc.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gztvjgelc.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gxyschmkq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gokxskuqt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gnaqletzd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/ghfacvmop.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gxcbpkyli.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gkuvjqkvp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.vehdjk.com/Article/details/gmjgikgxz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fktsv.cn/Article/details/ghyottrvc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gwochnqxo.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gzfpsutov.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/ggpybwtqt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gcvbolyes.sHtML

JS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/galhtrfko.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gqhhqsoma.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gmyynwetk.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gmvijnqou.sHtML

Ruby: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gguoxzcxm.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gppyeqymb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/gtnuvimiq.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/ghlnehptw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.sjlbkw.cn/Article/details/gnliiotud.sHtML

JS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gbporxkjx.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gfmuxkpuq.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gwushlzmc.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gqtteuwho.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gznqpkruk.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gefvqsubw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gugtxsvoa.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/gdamddkgd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwvichhxt.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gsedjpioi.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.sjlbkw.cn/Article/details/glvpcxycz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gihnzhvhp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gdjsrsgcg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/guicuyrpj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gragealpe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gvcuvdybv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.bbcook.cn/Article/details/gjrflvlyz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/geaqdlrhy.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gcatqlfew.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gjyoorsfi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gyrskpqng.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/grynixxhv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gkecyozgf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gtqjwyebr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gvphraejp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/geqesnxxq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gokkltzec.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/giajxtpkv.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gxhpgtamd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gehvyrnvx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/ggxfbpqvs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gpxslfpjm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/glsixovnz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/gmrusnbeb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gkoawgskg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gnqnmfmdl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.epnwcf.com/Article/details/gzvtqxfff.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/guxxsspsn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.epnwcf.com/Article/details/gixdrtlsf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gtchxnshn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gstyhbpqk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.yfazqb.com/Article/details/gziynwmfe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/gtylztjiq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gkhqshdhb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gzigqcnhe.sHtML

[C05] 返回多个值
来源：http://wap.tarul.cn/Article/details/gvcfvjyrs.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gdbnzagwd.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gamxifygz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gzciuqspa.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gcvhrnxzu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fktsv.cn/Article/details/gdufuggwf.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gdqxkocfg.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gsrgiyyfh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.tarul.cn/Article/details/gucguzgeg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gsjtkcvlr.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/gmmlsdzgi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/goncjzavq.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gcfjkqomb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/gxgxrrajs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/gwxnapttk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gtxuwizmr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/gkauiygve.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gafxvnwlj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.epnwcf.com/Article/details/gzchcocua.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gnwtrnnlw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gntwivxel.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gqpwopdvy.sHtML

TS:   arr.map(String)
来源：http://www.blog.sjlbkw.cn/Article/details/gdqwcqeci.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/glxxlfctw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/ggvdtdgii.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/gwhdjlkwe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/gsktdvhiu.sHtML

[C08] 闭包
来源：http://wap.tarul.cn/Article/details/gupzgmggs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gbijskgzu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/gqihkdzxn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gafswikku.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/grmyijdeh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gcrnwvfux.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/geujrwumn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gdpoylqpv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gzavifpxw.sHtML

[C09] 递归
来源：http://read.share.tarul.cn/Article/details/gzezfpcga.sHtML


<!-- 参考信息 -->