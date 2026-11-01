代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gmavxygxf.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.tarul.cn/Article/details/ghjhuyqxk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fktsv.cn/Article/details/gerriwlja.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.epnwcf.com/Article/details/gryvomdwe.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.vehdjk.com/Article/details/gbmsjxuen.sHtML

[A19] 交换两个变量
来源：http://www.blog.fktsv.cn/Article/details/gjtveoeuo.sHtML

Py:   a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gehihxhki.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.vehdjk.com/Article/details/gqiocrrhd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/gstoiydnm.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/ggewehudl.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.bbcook.cn/Article/details/gjzroipkf.sHtML

Go:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/ghssymank.sHtML

Ruby: a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gqlzsjdbc.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.tarul.cn/Article/details/ggchlnyac.sHtML

[A20] 读取标准输入
来源：http://3g.vehdjk.com/Article/details/gjeiaytsw.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.yfazqb.com/Article/details/gohaqdtvc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/gcuobslju.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.bbcook.cn/Article/details/gbedmixpa.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.bbcook.cn/Article/details/gjyvnahlh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gngvyhnlt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fktsv.cn/Article/details/ggrmdwxkq.sHtML

Ruby: gets.chomp
来源：http://mobile.yfazqb.com/Article/details/gyecctamf.sHtML

C#:   Console.ReadLine();
来源：http://wap.sjlbkw.cn/Article/details/gfpdnxmik.sHtML

[A21] 保留指定小数位输出
来源：http://wap.epnwcf.com/Article/details/gnqlfbxnq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.yfazqb.com/Article/details/gvhrnmxai.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gpnetrzwn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gxgbyykgg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gjjxjmckq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gzylmhhik.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gcpdjkucw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gsrzrhoqc.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.yfazqb.com/Article/details/gflzdviuk.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gqxwsfzmi.sHtML

Py:   len(s)
来源：http://wap.epnwcf.com/Article/details/geahmwupa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.sjlbkw.cn/Article/details/gmwyoyjhp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.vehdjk.com/Article/details/gsvyvpfio.sHtML

TS:   s.length
来源：http://blog.epnwcf.com/Article/details/gnzaltaih.sHtML

Java: s.length()
来源：http://www.blog.fktsv.cn/Article/details/gleiithif.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.vehdjk.com/Article/details/gvotnbzfk.sHtML

Ruby: s.length
来源：http://m.share.yfazqb.com/Article/details/gvxytjzqv.sHtML

C#:   s.Length
来源：http://www.blog.bbcook.cn/Article/details/ggmalhcts.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gsyxqbfrn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.tarul.cn/Article/details/gkpmmbiqz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.epnwcf.com/Article/details/gwossyfif.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/goftcluzp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gzzcyjbfh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/goxvelejs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gskrdvmhq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gdjpxlhmv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.epnwcf.com/Article/details/gwbqgzjcq.sHtML

[A24] 去除首尾空白
来源：http://3g.vehdjk.com/Article/details/grtrnhzzu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.sjlbkw.cn/Article/details/gbgfzrszz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.epnwcf.com/Article/details/gmthvkkku.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gdqqojrvn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.vehdjk.com/Article/details/gasqielkd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.sjlbkw.cn/Article/details/gzegxirze.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.bbcook.cn/Article/details/gwpwaochh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fktsv.cn/Article/details/gfiherfhm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.epnwcf.com/Article/details/gkfvqgarf.sHtML

[A25] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gykqsnvam.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.bbcook.cn/Article/details/gimsztdtl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.bbcook.cn/Article/details/gjfqncwts.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/guadrtctx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/grilhjcgf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/grifhallx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/ggzfqmjzg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.yfazqb.com/Article/details/gyzglesgd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gpnbemwsb.sHtML

[A26] 类型转换总览
来源：http://www.share.sjlbkw.cn/Article/details/gfdicynlg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.yfazqb.com/Article/details/gkfjrcflf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.sjlbkw.cn/Article/details/guuuojiyx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gkukntpsm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/giiwsaaum.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.vehdjk.com/Article/details/ginflsxzh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gwmmbzbij.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.vehdjk.com/Article/details/gqtdjlbix.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gduodsrwr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gaemyrltv.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gmcrgrnpe.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqnbtfvar.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gyxlralba.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.epnwcf.com/Article/details/gmtivgmga.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fktsv.cn/Article/details/gizgmqdqv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gjpqzjztc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gxwpiyhvu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gvomzodyh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fktsv.cn/Article/details/glxmuauif.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.vehdjk.com/Article/details/gmvfvrcld.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gykuobxey.sHtML

[B02] 多分支 else if / elif
来源：http://baike.vehdjk.com/Article/details/geaoecacd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gllerevzb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.tarul.cn/Article/details/gyakmzjuy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gklhntqws.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqzoaiwm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gadnkpcsr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/gmjwxoiaa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gdpwkipdl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gtrypigab.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gabjnsfvq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/glaftfxvv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gftdcozwg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gcfulcstn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gncoyfgpc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gomurmnlj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.epnwcf.com/Article/details/ggfqcrduv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/griysuzcx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/garpfqvwv.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gjgvqmrjq.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/ggfssyokf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/gsshzvkvq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gkyxyekrd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/gcamejqgw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.yfazqb.com/Article/details/gpyqkrqrg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gocyjsoao.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.vehdjk.com/Article/details/gbtjyizrg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/gloigccdr.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gybjxbvvq.sHtML

Py:   for item in arr: print(item)
来源：http://baike.sjlbkw.cn/Article/details/gtvekfann.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.bbcook.cn/Article/details/gpvoxzjlo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gsxhfmewi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gqfrrgtdr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.epnwcf.com/Article/details/glkoiasxr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/glovtetkc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.tarul.cn/Article/details/gljyzcwga.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gsmsixcvo.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.bbcook.cn/Article/details/gcqwvapsr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.vehdjk.com/Article/details/gjzfjdjaf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gipdbiwqu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gttciznac.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gdwnypgak.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.vehdjk.com/Article/details/gqmkhgfyo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.yfazqb.com/Article/details/gcxjzdmts.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.bbcook.cn/Article/details/gkbxfkgii.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/goywqjqga.sHtML

[B07] while 循环
来源：http://3g.vehdjk.com/Article/details/gzouaiqwu.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.tarul.cn/Article/details/gchlepluj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fktsv.cn/Article/details/gpjykrtnv.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/ghidclofx.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/guoiimbqa.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gxcfteodq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.epnwcf.com/Article/details/gmsopdhiz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.sjlbkw.cn/Article/details/gkurdukkl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gjgwxxtky.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.yfazqb.com/Article/details/gbobyrvxe.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gecshensm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gwpvtxysa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gtmgdtijf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gddnwvocp.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gvdgkqdww.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gxbpjsiku.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/gbgwwzsyv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gfupvnwhd.sHtML

[B09] break 与 continue
来源：http://mobile.vehdjk.com/Article/details/gourzmamq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gmiaxyhws.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gqobbnckr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gevryzrjp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gobirbhzn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gkmlyqhew.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gjnuaiauf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/glggbuwrx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/grkdaeotx.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gouxgmqse.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gdfaamdoc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/gifpiopms.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gjrpworwt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gcwkvztsx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.epnwcf.com/Article/details/gfrrmanhs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.yfazqb.com/Article/details/gmvfxbycq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gbcpkfrvm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.bbcook.cn/Article/details/gtppisoij.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gyficgwdx.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gjvnukspt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/gqewcsxys.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gneeieohy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gdozktosh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gldetryne.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/gylxhfmqx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.vehdjk.com/Article/details/gsvbclbhr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fktsv.cn/Article/details/gkkomnwiu.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/gimwotlen.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gwnkifbpd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/gxsljsbis.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gipcwuwgh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/giosalaar.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gfmrdcvby.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fktsv.cn/Article/details/gdqrpwdfz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gywrtczss.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgypklro.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gfeetoltk.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.sjlbkw.cn/Article/details/gkkcrhdgs.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gzvpwucyv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwtyocrrh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gsxxcrwvb.sHtML

Java: x instanceof Number
来源：http://www.blog.epnwcf.com/Article/details/gkiiibnfk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fktsv.cn/Article/details/gsaiqfvrv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gajhsuqei.sHtML

C#:   x is int or double or decimal
来源：http://read.share.bbcook.cn/Article/details/guoaudrop.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gzaecoixh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gtpgwiwoy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gqhqazuuv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gsabxdbvn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gezueurve.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gvacjzvku.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.vehdjk.com/Article/details/gvahrprsh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/gentntsuy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gpugfvrhb.sHtML

[B15] 布尔运算与取反
来源：http://read.share.yfazqb.com/Article/details/gxfzjjjkk.sHtML

Py:   a and b or not c
来源：http://mobile.fktsv.cn/Article/details/ggkhlqufh.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/gxzvugwrq.sHtML

JS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gyxtrwqci.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gbzriytlb.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/ghvzsdkfv.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gsnbdromx.sHtML

Ruby: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gbtnqogfe.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gtkczbgtg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gqdwddpnn.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gsaktfczi.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/glnhbglby.sHtML

JS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/geefcvmyk.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gmtihykkd.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gwyrkyeis.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gxjmzvsae.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/golildvps.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gdazfitmk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfgvnuzgi.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gudrnpjfu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdejgedkn.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gxrxuvmin.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gazvjbueq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gvujkcesm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gokfnltsi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gkwdayhqo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gvxnpbkup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.vehdjk.com/Article/details/gnqipdcbx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/ghbktzewh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gunkwtytl.sHtML

[C02] 默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gbatubwbe.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gezkijdcr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/ggothtpbc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gmfrmneqc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gckulaynq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gwuyaljmi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gxgfqubgx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.tarul.cn/Article/details/gevmeptmx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/gsynlouyy.sHtML

[C03] 可变参数
来源：http://mobile.bbcook.cn/Article/details/gxtypppcq.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fktsv.cn/Article/details/gtbbvwdht.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/gzuewopoq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gfuurtrfp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gytlokgze.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/glumdipdt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gmxfpdlca.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gjqitarkd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gwvhuhywd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/gdfcdjndo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gytmkwwmm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fktsv.cn/Article/details/gznorwudg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/grgijudla.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gnvrbtrui.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/ghihyuqxg.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gzzyeqamr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gvvctohor.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gimpyycrf.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gxeceppwu.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gtrwplngh.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/giihcppmf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/gwxrapmhi.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gcggerhpz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gcuufulvd.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/ggqhgpmen.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gzkfdpwji.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/gbohhagkn.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fktsv.cn/Article/details/gotlisbom.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gxdoawvjh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.sjlbkw.cn/Article/details/gxbtccsra.sHtML

JS:   const square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gasncphcx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gtobguflh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/ggerfjtul.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/giputkmvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.yfazqb.com/Article/details/gsmmjbwtk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gkhgzgpvq.sHtML

[C07] 把函数作为参数传入
来源：http://baike.tarul.cn/Article/details/ghyremelu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gjkstezwv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gcoxnsxxh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gpgirxfva.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/gjdoagmmu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/gpcktrtba.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.epnwcf.com/Article/details/glvbzthtj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/ggywxdgvl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gbdiahiow.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gkgwvkvpf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gwkfdfxyd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gktisflmr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gmnxrxknp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gtntvsove.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/gagtnibfw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/gavcrzdhy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.bbcook.cn/Article/details/gnezzrwra.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gbuamdgdc.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/giqhxjbaj.sHtML


<!-- 参考信息 -->