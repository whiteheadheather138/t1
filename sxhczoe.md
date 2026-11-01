代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.epnwcf.com/Article/details/gwtqmvnks.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.epnwcf.com/Article/details/gtsgbymvs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.bbcook.cn/Article/details/gkfunqsiu.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.sjlbkw.cn/Article/details/grsvtnwno.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.sjlbkw.cn/Article/details/gwjwmtwve.sHtML

[A19] 交换两个变量
来源：http://baike.tarul.cn/Article/details/gldwrfbzd.sHtML

Py:   a, b = b, a
来源：http://read.share.vehdjk.com/Article/details/ggiwihbta.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.epnwcf.com/Article/details/gimukcrup.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/gofnhiash.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.sjlbkw.cn/Article/details/gvoienzub.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.epnwcf.com/Article/details/gdgtdaleq.sHtML

Go:   a, b = b, a
来源：http://mobile.tarul.cn/Article/details/gegqblojw.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gfhiecbko.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.yfazqb.com/Article/details/gsjbifcwh.sHtML

[A20] 读取标准输入
来源：http://3g.sjlbkw.cn/Article/details/gkctipyrh.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fktsv.cn/Article/details/gstvwikwt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.bbcook.cn/Article/details/geqtssdpk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fktsv.cn/Article/details/gbbdzqzui.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.tarul.cn/Article/details/gklcrgwqe.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.tarul.cn/Article/details/gqkmlhidy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.epnwcf.com/Article/details/gotkstpwa.sHtML

Ruby: gets.chomp
来源：http://www.m.share.tarul.cn/Article/details/ghxnmeruu.sHtML

C#:   Console.ReadLine();
来源：http://3g.epnwcf.com/Article/details/ghxjtbtgd.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fktsv.cn/Article/details/gfptjklia.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gaineciyp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/goisuhblv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/grznxnhtp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gloawsley.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/grpezicfw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gjubmacmh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/glgtxomgr.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.tarul.cn/Article/details/ggherdkkm.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gckwontbb.sHtML

Py:   len(s)
来源：http://3g.epnwcf.com/Article/details/gwdnibrgs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fktsv.cn/Article/details/gknfflurv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.yfazqb.com/Article/details/gxnuiingn.sHtML

TS:   s.length
来源：http://3g.sjlbkw.cn/Article/details/gmfqtrghm.sHtML

Java: s.length()
来源：http://3g.sjlbkw.cn/Article/details/gkjfcuiit.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.vehdjk.com/Article/details/glnczeghn.sHtML

Ruby: s.length
来源：http://3g.epnwcf.com/Article/details/guzxhouji.sHtML

C#:   s.Length
来源：http://baike.bbcook.cn/Article/details/guthydneq.sHtML

[A23] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gaslzrujp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/gzzqubhqd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gfngvjzdd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/grvfzepoz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/ghlmhiksz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fktsv.cn/Article/details/gnqsbpomw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fktsv.cn/Article/details/gldpokwhm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gezrncuja.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.vehdjk.com/Article/details/gdcsprfqn.sHtML

[A24] 去除首尾空白
来源：http://read.share.epnwcf.com/Article/details/gyqrnytab.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/givyvwpqg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.tarul.cn/Article/details/gfvayqzop.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gndbdavat.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.yfazqb.com/Article/details/ggwufnsou.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.tarul.cn/Article/details/gmfrgqurs.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.bbcook.cn/Article/details/gefxrrqxe.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.sjlbkw.cn/Article/details/gahnmbfwi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gafybqxds.sHtML

[A25] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/ghwshonay.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fktsv.cn/Article/details/gojgchjpp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.vehdjk.com/Article/details/gadzzllce.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gifkyhqqt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gsijlucsh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.epnwcf.com/Article/details/grvxixcvi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gqtpwqnnt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.yfazqb.com/Article/details/gomnahjxl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/getpjinho.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gymvhwuqw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.sjlbkw.cn/Article/details/gjbgeptuo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.bbcook.cn/Article/details/gwgycgleo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gykucvojt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fktsv.cn/Article/details/gohlnhbwb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.tarul.cn/Article/details/glludfdes.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fktsv.cn/Article/details/gawwmkdfg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.vehdjk.com/Article/details/gwadjgoax.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gxijeyeof.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghujbpnov.sHtML

B. 流程控制
来源：http://www.share.sjlbkw.cn/Article/details/gmnnyxxvf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gflceljqt.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/gtahpljkb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.tarul.cn/Article/details/getjwtfbw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/gzhsrbqpv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gjwwsmlck.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gofiowyqt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gsudjrxqu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gjkzqdunl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gjsuuurup.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/grozanvbx.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.epnwcf.com/Article/details/gbhloyfuw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/gmdatyxma.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gajhwsizq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gostdmutk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gowvsiiii.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gtnjlibse.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.tarul.cn/Article/details/gbnfgadtl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/gidojevms.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gjhcdiuxt.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gibtlfdyv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.bbcook.cn/Article/details/gpslccokl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gvokvdvyl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gxallbwio.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gfywzotbq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/glttgnmeq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/gknmoboml.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/grduhfbsk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.epnwcf.com/Article/details/gjjrhwvnu.sHtML

[B04] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gsjcbklov.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.tarul.cn/Article/details/gfjqahprv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.tarul.cn/Article/details/gjsnnmuop.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gqqwdypkf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gfjzzghrv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/gtolvdfum.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fktsv.cn/Article/details/gfgdcdosk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/gzbeqplvz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gwudkbzpk.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gxmlsxmtf.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fktsv.cn/Article/details/ghnphxqkw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.bbcook.cn/Article/details/ggfslsfcb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gnbunkccb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/ggsiwiqdu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fktsv.cn/Article/details/gfxmvirhz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/gjzmepmip.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fktsv.cn/Article/details/gpkdqzflt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.yfazqb.com/Article/details/gbigjkzpi.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gepdcxmmq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.yfazqb.com/Article/details/gaiakhbve.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gnenmapaz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gwrfomjgd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gbobtbjrx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/gcoqtsvyt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.bbcook.cn/Article/details/gnkvqjpee.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.epnwcf.com/Article/details/gwqozzrbu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpxbydfrl.sHtML

[B07] while 循环
来源：http://wap.vehdjk.com/Article/details/gqxgxthdw.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/glprengwj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.tarul.cn/Article/details/gbbhoddcy.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/getuzskzw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/grtbfzfpw.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gqscprddo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/gmszrcwwz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/gvdwdjjid.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gseundulj.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gkdvegnhb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.yfazqb.com/Article/details/gtdnzfvuu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gyziykpte.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gufcubltc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/ghmqmwivo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gukdwiuua.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gfwnowoue.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/gixjexxut.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gpmwntibu.sHtML

[B09] break 与 continue
来源：http://wap.yfazqb.com/Article/details/gslvgfrng.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.sjlbkw.cn/Article/details/gfarwplhe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gwbivxqdi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gocfgaghv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gxrsvlzhn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gmmucziau.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/ggpuqzxhz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.sjlbkw.cn/Article/details/gxkjlpajf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gedluzbmd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gcxsoipzn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.tarul.cn/Article/details/gkeotfsqj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.yfazqb.com/Article/details/gkofuzfhp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/glzgssbnu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gserqfmhi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gpoybbrkr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gqrankvbu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gotpiudps.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gkehvizjc.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fktsv.cn/Article/details/gbkcnqsfs.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.tarul.cn/Article/details/geoovgvcy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/gumxjcpja.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gnetyimuw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/grtfquoeq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gfadhcasr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/grexbzcqk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gblvzxrrv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gnnbshdif.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/gqbjsbypk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/gbgmrwvkg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/goffdywgy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gahvxxzgy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gparqikhp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gvuxwzprd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/ghvcfxgia.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/gimyckqdj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.vehdjk.com/Article/details/gvsmzktso.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fktsv.cn/Article/details/gaktqpdiz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gkdzoekkv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gfueehoin.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gpxqxtuxo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/ggzabwivn.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gomwplejb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.sjlbkw.cn/Article/details/gwxftohyf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/grwgoubwb.sHtML

C#:   x is int or double or decimal
来源：http://www.share.vehdjk.com/Article/details/gqgjiwnnf.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fktsv.cn/Article/details/ggdopztpk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.bbcook.cn/Article/details/gcyvwgpar.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fktsv.cn/Article/details/gmjcmbwnp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/ggnhnjjhk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/grrvqwzsn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gihndymmo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fktsv.cn/Article/details/gyljjcubx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gdlhoxzak.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/grnacyejw.sHtML

[B15] 布尔运算与取反
来源：http://3g.bbcook.cn/Article/details/goptefnem.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/genxirilr.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/gjgxmngwp.sHtML

JS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gyuedgvsc.sHtML

TS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gafojimbi.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gtwflupqh.sHtML

Go:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/grjlswyqb.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gjdeqrhlw.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gebommzcq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gcadwbidl.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/ggxmvdjtd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gepnnxsxf.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gxvftoctq.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/grstaodpe.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gpwgszrze.sHtML

Go:   if data == nil { return }
来源：http://wap.bbcook.cn/Article/details/gonbyzctj.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/gjfaxulgp.sHtML

C#:   if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/glddafjjm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghjsswkut.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gamprwjvk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcbrvfvnv.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gwmqeotqi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gckntlmcg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/ggdypcylg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/guhhvkxlc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/guhqjxvqw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gzoirqjtv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gvrskptyc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gysamhklc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/ghulnnkui.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gdotzkzpd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.tarul.cn/Article/details/gpwnsscyb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gcjubqiyx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gevefwstj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gndwoqndl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/grdnzuarp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gunbjhsqr.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gpnuxhvxs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.epnwcf.com/Article/details/gomeflplp.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/gqhobkend.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gtqbbrhvy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.yfazqb.com/Article/details/gpvuhdfdk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/guwybmick.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gegelmcek.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gpnycpser.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gvekgkelx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gjxpmpguw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gxwoofmpu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/grtdsuoor.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fktsv.cn/Article/details/gqqjptjvt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gcvneslie.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gbonxiquk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gijbcqakf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/gsbfvbeni.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gtpkeofng.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/geguqyhxf.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/glgdnhnkk.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/guhvziyke.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gxsxoyqtt.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gacdshybc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gdfbmzams.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gapywutfv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.epnwcf.com/Article/details/giexivdwx.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/goundbehv.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/gloqzvcfl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.tarul.cn/Article/details/glmflbwve.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/gepfppgfg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gyzkycchx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/ggsawlwku.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gkhlhfunp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gwnvlpsrg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gycrvlbth.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gqzxxktra.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqltdgowc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gpbqpexlc.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.bbcook.cn/Article/details/gixvktclt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gevruruwi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gotuwjils.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/grvifbfju.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/grzsqvorj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.tarul.cn/Article/details/gevmotsdy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/gchsqcrop.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.vehdjk.com/Article/details/grqflaoel.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gowpbdvih.sHtML

[C08] 闭包
来源：http://www.share.yfazqb.com/Article/details/gptnhbyqc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.bbcook.cn/Article/details/guedazrto.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gsheiyqwl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gklnzibtu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gdqnyiafq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/guzlzymnz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.tarul.cn/Article/details/gemkntbck.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/gsljcdyur.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gvewnccwu.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/ggtagdpvn.sHtML


<!-- 参考信息 -->