代发 wailian999

C#:   (int)'A'; (char)65
来源：http://wap.sjlbkw.cn/Article/details/grvmlguyn.sHtML

[A19] 交换两个变量
来源：http://mobile.fktsv.cn/Article/details/ggefkzuhy.sHtML

Py:   a, b = b, a
来源：http://wap.vehdjk.com/Article/details/gpppwybdu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.tarul.cn/Article/details/grilcibbl.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gdjdkxihv.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.sjlbkw.cn/Article/details/guhspuxoe.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fktsv.cn/Article/details/ggcnunhft.sHtML

Go:   a, b = b, a
来源：http://blog.sjlbkw.cn/Article/details/gbzefeadw.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/ggoiermov.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.vehdjk.com/Article/details/gyokxjcgs.sHtML

[A20] 读取标准输入
来源：http://www.blog.yfazqb.com/Article/details/ghhniwwda.sHtML

Py:   name = input("请输入：")
来源：http://m.share.epnwcf.com/Article/details/glbtyngtf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.bbcook.cn/Article/details/gfiptkgpc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.tarul.cn/Article/details/gnfvgkols.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.bbcook.cn/Article/details/gxvyknwgt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/gctncfmre.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.epnwcf.com/Article/details/gnjfcmyhn.sHtML

Ruby: gets.chomp
来源：http://mobile.fktsv.cn/Article/details/getguwpqh.sHtML

C#:   Console.ReadLine();
来源：http://blog.yfazqb.com/Article/details/gzfsgcmgo.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fktsv.cn/Article/details/gsasbxylq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.yfazqb.com/Article/details/gsyaeiqxa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gvodhuldm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/ghzrcdzov.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfpnxbucs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/geqasxgfs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gmkivpfdo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gcdkrzeea.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.bbcook.cn/Article/details/gpmggnivc.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gtyuugwpv.sHtML

Py:   len(s)
来源：http://mobile.tarul.cn/Article/details/gpgbzoaum.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fktsv.cn/Article/details/gffefuehx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.bbcook.cn/Article/details/gltixuowc.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/gzevhnarq.sHtML

Java: s.length()
来源：http://baike.fktsv.cn/Article/details/gwvludyjk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/gfqrrncpj.sHtML

Ruby: s.length
来源：http://www.share.bbcook.cn/Article/details/gecbgcpuw.sHtML

C#:   s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gsbvcjctr.sHtML

[A23] 大小写转换
来源：http://3g.tarul.cn/Article/details/guatdbgxp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.tarul.cn/Article/details/gtihsglqu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.tarul.cn/Article/details/gjpzyklec.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/gqbjnrlki.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gvsclqlxn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/galwxnplu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fktsv.cn/Article/details/gzyknhsze.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.yfazqb.com/Article/details/gwqkaaxcf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/gkvbyybid.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/gqmtdgjki.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.tarul.cn/Article/details/gtpqgtwmu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/gculsicqn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/ghinceapm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/guddbgoqm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.vehdjk.com/Article/details/gzqjxwhcv.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.tarul.cn/Article/details/ggwxhzozo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/gyhpgbczt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.vehdjk.com/Article/details/gsufzdfjc.sHtML

[A25] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/goztytqof.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fktsv.cn/Article/details/gjcrckfqp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.tarul.cn/Article/details/gqftirpeu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.vehdjk.com/Article/details/ggqocgkpd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.bbcook.cn/Article/details/grfdyqzcm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.sjlbkw.cn/Article/details/gbdkqeqsl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gyhhrykuc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.vehdjk.com/Article/details/ggkyjyiqi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gnhmaiukt.sHtML

[A26] 类型转换总览
来源：http://read.share.sjlbkw.cn/Article/details/gflneiido.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.tarul.cn/Article/details/girsjnenp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/ggkrsgkpo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/gdxypufra.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/gztojcinf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gxhxdqoku.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.sjlbkw.cn/Article/details/gtjmrswpg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.yfazqb.com/Article/details/gncdmecrn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/gmutaynbg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtqjpwoxd.sHtML

B. 流程控制
来源：http://m.share.fktsv.cn/Article/details/gsgvdgogp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtodkezyl.sHtML

[B01] 条件判断 if / else
来源：http://3g.tarul.cn/Article/details/gpcrzijzk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/glhldimvx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.bbcook.cn/Article/details/grvdxyrvq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gwdxmfwpg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/ggczknhpb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gdrjmbssc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.vehdjk.com/Article/details/gvqtienwn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fktsv.cn/Article/details/gozfinhqg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gglypowfn.sHtML

[B02] 多分支 else if / elif
来源：http://3g.bbcook.cn/Article/details/gbytcbfxx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.yfazqb.com/Article/details/gygzftaaj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fktsv.cn/Article/details/gprhixjef.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gfvdezpxo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/guodpmbkz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gtysvxblz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/giilizflh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.tarul.cn/Article/details/gbusnzwhg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gseqoxnow.sHtML

[B03] switch / match / case
来源：http://wap.fktsv.cn/Article/details/goykwtjzd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/gwnabaptl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gdisuahnz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gjrnxugxo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gfarlkraw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gtktkwohc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/geybpqkcx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fktsv.cn/Article/details/gdidfttbq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gdpvlhpez.sHtML

[B04] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gwxxpvlvf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.yfazqb.com/Article/details/gnqvuvqol.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fktsv.cn/Article/details/grtxxzaxo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gdagcpmpa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gktcydpmg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/glmhjqbwf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fktsv.cn/Article/details/gbydecxqb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/ghsrmdayl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.sjlbkw.cn/Article/details/geknwdrzk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gijgcbndz.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fktsv.cn/Article/details/gauhrdzfr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/ggjqqjrsy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gdtszygrd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gpcssxdud.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.tarul.cn/Article/details/gcyuzrqki.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gcpeeuwru.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/grnfzfpuw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.sjlbkw.cn/Article/details/glzwbsnix.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.yfazqb.com/Article/details/glhlgvbcj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gpypipkoc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.vehdjk.com/Article/details/gxpgedliz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gkvkrhzpv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gehfdmutf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.epnwcf.com/Article/details/galzqphve.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.vehdjk.com/Article/details/gxjdvvacc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.bbcook.cn/Article/details/gczfztluh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/gwzpnvfah.sHtML

[B07] while 循环
来源：http://blog.tarul.cn/Article/details/gdhjtajur.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fktsv.cn/Article/details/ggjfxqflp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gqfdvlegm.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gaznakoui.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gkzkifwbm.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gkkhyoqdj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/gcfjwjqbg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/ghpiywqeh.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gozubxzie.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fktsv.cn/Article/details/gfkyqyirp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.sjlbkw.cn/Article/details/gqhphinbu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.bbcook.cn/Article/details/gqmmhgcqh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/guarklsvw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/ginawtnbs.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/glvykdzvr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gkkwwosnn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.sjlbkw.cn/Article/details/gdgkspvma.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gqbrhthif.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gfoycvveu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/ghqiqmyti.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbaojfvsz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gkymjgapo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gdyfmhfwr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gnvnpjyww.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.sjlbkw.cn/Article/details/greezmldt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fktsv.cn/Article/details/gmnwwodqr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gbwjkjzjy.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/gzjckxlcg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.bbcook.cn/Article/details/gskfckanc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fktsv.cn/Article/details/gaojzqone.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/goyeogjfx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gquqakgqx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gkutywcza.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/gjorujeen.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtkygttz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gdltomitq.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gysoesgrd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/guojufkdg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gqkvlutsi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/geisjjxgu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gmrixphdy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/glhoutatw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gahmwlofx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.bbcook.cn/Article/details/gcukmrhbb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/ghfvhjjtm.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gkebhqhne.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/gqsfdlsvc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/gprbomtvd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gcgyomyyb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gkpzaisfn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gnbbribta.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/glwgfdwqb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gatgjzqol.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/gssabzdmg.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gmbqptkhr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/gxsitdbse.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gofmyagtq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gzuyqnahm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/gxhvjzhsq.sHtML

Java: x instanceof Number
来源：http://www.blog.epnwcf.com/Article/details/gzqcjmbgv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/gaqbmgkfq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.tarul.cn/Article/details/grzjlmdva.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gokazmfpa.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.bbcook.cn/Article/details/gntylfqtm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.tarul.cn/Article/details/gavsoqknd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/gnbuebihj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/ginjmcgji.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/goyfxlihj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/giqbpvkzg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fktsv.cn/Article/details/giycsmwzy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/glepdqpvm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/geqldyjci.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/grraiadot.sHtML

Py:   a and b or not c
来源：http://3g.vehdjk.com/Article/details/gkgikzeia.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/gvjkonmkf.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gsqtvrynb.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gecjnoupy.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/glalnpxpw.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gspwkhprg.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gnodkimvj.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gtpkfogka.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gwjvybakp.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/grqblajfu.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gtiipdmyq.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/guoobckpt.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/glwaafnrq.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gvxlfzpkm.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gsunqadht.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/gtunuiesj.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gnplchddt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsetmwkfs.sHtML

C. 函数与作用域
来源：http://wap.bbcook.cn/Article/details/gwislhfkp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gukllxgpu.sHtML

[C01] 定义函数
来源：http://baike.epnwcf.com/Article/details/gbgadtkgk.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/glhmukhji.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gbctbheng.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gdxlykapf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gggohipvf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gkknssbbj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gnbxahopo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gheyackjo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gqskdebzo.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gpjtkwbjl.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gzamaxsds.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/grmssoahn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/ghzmxlpmd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/govhucrsr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.sjlbkw.cn/Article/details/ggawvqmre.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.sjlbkw.cn/Article/details/gywkiddgn.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gtsesmnge.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.bbcook.cn/Article/details/gjfbhumqb.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/gakpkttgg.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gwmtdojzd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/glgylfxsd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gmhtpkcag.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gmwdhrxvt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gurngrypg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/grqdvbwmu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.vehdjk.com/Article/details/gskhztotl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.yfazqb.com/Article/details/gjuzuxijn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/grcwvpcly.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gghxreilz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.epnwcf.com/Article/details/grebbagbh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/ggdkyqfgw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.bbcook.cn/Article/details/goduielji.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/gscrgmrdc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/gpmigacyw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gpggysolj.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gdaovwbpb.sHtML

[C05] 返回多个值
来源：http://mobile.epnwcf.com/Article/details/gycscrhbe.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/grqvegvth.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gecbwsgbj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/gfoogkdvx.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/geprpoyhk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/gbkireybz.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/gsfyxbezn.sHtML

Ruby: return a, b
来源：http://wap.vehdjk.com/Article/details/gpgswbsmk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/gkzdimayz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/ghfresxnk.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gibacutrw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gfxwpjkbj.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/goxunxhqt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/guvfgtuav.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/grxyytgtv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gmiguarwk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtzmhppg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gsdrhldlr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.tarul.cn/Article/details/goqoksmel.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/glcrdqybo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/goouarabj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gyuigapyw.sHtML

TS:   arr.map(String)
来源：http://baike.fktsv.cn/Article/details/gnupcgyds.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gysqdzaid.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/glslmdjcd.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.epnwcf.com/Article/details/gilqczdrt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gpzxsskqb.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gthgtwmhs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gpwwgkqnp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/glxvkyxld.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gddwxoiok.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/ggqewgdlt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/glnaxrqaa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/gfdzwvdxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.vehdjk.com/Article/details/gssihcsta.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/goorraurp.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/ggbmnkpij.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gcgklgdgy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/griwnyevq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gydnbttjj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gzmnmwuwq.sHtML


<!-- 参考信息 -->