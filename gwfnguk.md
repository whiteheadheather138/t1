代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gzqxttedv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.epnwcf.com/Article/details/glhhqbkmv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/ghfoesixe.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gpkcxolcl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gnefyyikt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gvfzskoex.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gpkjlgcph.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gcgnzcsxr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.bbcook.cn/Article/details/gjicyfvtm.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/gloedhrxc.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gsvrwtbaf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fktsv.cn/Article/details/gmasnxlax.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.tarul.cn/Article/details/gotgxddpo.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.tarul.cn/Article/details/ggokphrio.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.sjlbkw.cn/Article/details/gjpgipatp.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.sjlbkw.cn/Article/details/gfkexxsnk.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.vehdjk.com/Article/details/gkzeagnyp.sHtML

[A19] 交换两个变量
来源：http://m.share.fktsv.cn/Article/details/gbwwetpgj.sHtML

Py:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gioaetcnn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.vehdjk.com/Article/details/glbcqvqun.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/gtosncnmr.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fktsv.cn/Article/details/gsmlmhgva.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.bbcook.cn/Article/details/ghofdsavg.sHtML

Go:   a, b = b, a
来源：http://www.share.tarul.cn/Article/details/grqiypbur.sHtML

Ruby: a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gwbpeltwu.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/gvtrizbju.sHtML

[A20] 读取标准输入
来源：http://wap.vehdjk.com/Article/details/gsceomyoz.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.epnwcf.com/Article/details/gsvtqkazr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fktsv.cn/Article/details/gtwszamcn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.tarul.cn/Article/details/gfhkvxuwy.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.vehdjk.com/Article/details/gxpipgjgi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.epnwcf.com/Article/details/gfmyokmqj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.yfazqb.com/Article/details/grkdwfglg.sHtML

Ruby: gets.chomp
来源：http://www.share.vehdjk.com/Article/details/gmpfqqnck.sHtML

C#:   Console.ReadLine();
来源：http://m.share.bbcook.cn/Article/details/gyjtxlprr.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.sjlbkw.cn/Article/details/giycsywll.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.vehdjk.com/Article/details/gbviswxck.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gwkjdhtgp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/grxlyaujy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/ggcczyina.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gytuwoyys.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gfkltbxgh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gnjjhnoqz.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fktsv.cn/Article/details/gkquaxsko.sHtML

[A22] 获取字符串长度
来源：http://read.share.epnwcf.com/Article/details/geckoxstr.sHtML

Py:   len(s)
来源：http://baike.fktsv.cn/Article/details/gtnhnhkwh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gijigrewi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.sjlbkw.cn/Article/details/gvhgzefkm.sHtML

TS:   s.length
来源：http://www.share.sjlbkw.cn/Article/details/gqvxhdxzt.sHtML

Java: s.length()
来源：http://wap.tarul.cn/Article/details/gdagarutd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.yfazqb.com/Article/details/gnighmfbf.sHtML

Ruby: s.length
来源：http://3g.vehdjk.com/Article/details/gevyjktvn.sHtML

C#:   s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gwxwtkabv.sHtML

[A23] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gznilcehl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.epnwcf.com/Article/details/gcyqhdzzz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.bbcook.cn/Article/details/gazewuuov.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/grbqeqqkg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gfichdxax.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/grnlvycns.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gvjdawxok.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gxdpdegvf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.tarul.cn/Article/details/gpifmzfbz.sHtML

[A24] 去除首尾空白
来源：http://www.share.sjlbkw.cn/Article/details/giwwfnnks.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.bbcook.cn/Article/details/gewttjhch.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.tarul.cn/Article/details/gvbwmktbw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gijqxicng.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.tarul.cn/Article/details/glbiogakj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fktsv.cn/Article/details/gsrogrddh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxincdlpl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.bbcook.cn/Article/details/gpdwnnwpq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.vehdjk.com/Article/details/gtuvtjzdk.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/ggsccoktx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.sjlbkw.cn/Article/details/gxdwltgep.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/ghtbdeltj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/govvimtuu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/gutwpeehy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gxyylwkxa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gantytzcn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.vehdjk.com/Article/details/gngmvywfu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/gbgtinomr.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/giiwrtbfa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/gjcflqlfu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gwcqhrxxx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.sjlbkw.cn/Article/details/grntuqycg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.epnwcf.com/Article/details/grbsmzrij.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.vehdjk.com/Article/details/geungopxj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.tarul.cn/Article/details/gwjjpbslw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.tarul.cn/Article/details/gktwmfcxw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/gkcsatiai.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvmdeaogi.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gdqfcvnwv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqnwxalga.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.bbcook.cn/Article/details/gxrtdqlfm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gmneskzwl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.yfazqb.com/Article/details/gfonvlary.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/goafehqej.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gcsseagpd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbluqandy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/gjeonyimy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.vehdjk.com/Article/details/gopjvebaz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gyzpbltja.sHtML

[B02] 多分支 else if / elif
来源：http://wap.vehdjk.com/Article/details/gjnwnrqvp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.vehdjk.com/Article/details/gmaikypxh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.epnwcf.com/Article/details/gmfnipdxd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gsksaztnf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gbxgojusp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gvrlpifau.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gfaugtlrp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fktsv.cn/Article/details/gqmiceujp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gucxiwazz.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gzhuqaiuv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fktsv.cn/Article/details/geakxtpwd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/grcjelzus.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gsofgfbto.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gbwqpzntz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gbnojmklq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gcwrjqwsb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gmtwegaiv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.bbcook.cn/Article/details/geuhnqpel.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gwcgjfyio.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.vehdjk.com/Article/details/gtqipfsnu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/gwsyummju.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gimiqdgzf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gxrmulkdx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.vehdjk.com/Article/details/ghygyxejf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.vehdjk.com/Article/details/gcubiyjtn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gnwazozby.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.tarul.cn/Article/details/gclrwvdiv.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gdtxyfxni.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gyxabjbyp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gnmyzgrlo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gjreqfelb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gwprpgcyd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.epnwcf.com/Article/details/geoktcezo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.tarul.cn/Article/details/gtdaepcoz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.vehdjk.com/Article/details/gadaqdcet.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.yfazqb.com/Article/details/gcevddlne.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.bbcook.cn/Article/details/gbxcildcs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.yfazqb.com/Article/details/guzxagzgw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fktsv.cn/Article/details/gmeoocdum.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gztznmfsx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gxivmimgh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/gvkbbvtdp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.sjlbkw.cn/Article/details/ggnkixwyz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.epnwcf.com/Article/details/gxycnqmkq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.sjlbkw.cn/Article/details/gcpqrwchx.sHtML

[B07] while 循环
来源：http://m.share.vehdjk.com/Article/details/giwchrvol.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/gnsxltzsr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gyszeshws.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gjbfzkhlz.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gwezgiotl.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gjubutxho.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gztozouxi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gashcdcjr.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gupvkozej.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.yfazqb.com/Article/details/gvruoddfp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/grdjegieq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gusnttkua.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gjfcjlhcy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gfwpsdica.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gklwjpdbg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.sjlbkw.cn/Article/details/gsmuwjdam.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gbbgrnfti.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gjoexfjba.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gnzzfdzom.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gtknuxnjp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gmmtxusdx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/goyhgjcex.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/giaqjwzzs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/glleccnmi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gatolmksi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.bbcook.cn/Article/details/gvjmldmgl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gnbrtlgxc.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.vehdjk.com/Article/details/gxswfchpd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gleljtkkt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gngefvmim.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gdaebhfuh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiktpehs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.vehdjk.com/Article/details/gxxvwxlbr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.bbcook.cn/Article/details/ggednsxdt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/gewraxtcy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/gdlikkxsq.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.vehdjk.com/Article/details/gjsxgfxou.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gxtrghuds.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.tarul.cn/Article/details/gwoqrgfjs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gjouwibts.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gjheymsuk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gwvnvqkoa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/gjnmudrrp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.epnwcf.com/Article/details/ghjavanzz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gznsezohn.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/grjuyfetn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.tarul.cn/Article/details/gxdlnldrw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gfufmcipq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gscrjtfvd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gqlbpfree.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gtpxazaaa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/glyizjicr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/gcowycwvj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gdconuvhj.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/giiucokyx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gcsrobkzr.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fktsv.cn/Article/details/gurnmwvah.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/grjfvepon.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gcgonahrj.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/gblnsvwkc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gmqfmormw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/glrrmemxv.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gzzouxlxd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.tarul.cn/Article/details/gthuqspov.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gyjgekfuo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.yfazqb.com/Article/details/gpwvmncyv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gkqpksguo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gzttoceoc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/gwixiangp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.epnwcf.com/Article/details/gpbgmxseu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fktsv.cn/Article/details/gxlmffihp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gxgirvzow.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gonggbnbv.sHtML

Py:   a and b or not c
来源：http://m.share.tarul.cn/Article/details/gkkxknalz.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/glzvqvamn.sHtML

JS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/godzsnqil.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gaxugmmzq.sHtML

Java: a && b || !c
来源：http://baike.yfazqb.com/Article/details/ghfqhcdca.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/guvlizwzr.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gtoavricr.sHtML

C#:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/ggamyllab.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/ggdeyjrzj.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gnpzfdmks.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.tarul.cn/Article/details/gzmfzhemb.sHtML

JS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gacvrfccr.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gpmqiqebw.sHtML

Java: if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiwcbhyg.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/gwekxrjla.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gazcjlxzi.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gldisjbon.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsaoonkzx.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gctidbkjq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gahwkttau.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/grcoywffm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.tarul.cn/Article/details/gbgvdxcis.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gudzflptz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/goqiuxuyu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gsraoqfiq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gorkomjdo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fktsv.cn/Article/details/gurwootul.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gqcqrvzrt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gbtslswpb.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/gvrhyuzie.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gtdpvrfrn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/gyijbadso.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gmtafzmdx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/ggpceobiv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/ghcsgzwio.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gbeeaergj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gwmfecmnv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gupcizwnt.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gpipglvmr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrqoihcp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gqhyohdna.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/glhhqihvq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gvqexzzzc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gdgqghahg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gqxcazrfu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/goxahahmm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gmrknvzci.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gpfyczoav.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.vehdjk.com/Article/details/gxtmjzrgg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gbhntfgme.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gffkfslrd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.yfazqb.com/Article/details/gnqnqgref.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gmppfecka.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gtbgmlskj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gylgeahdw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gmtmhrykn.sHtML

[C05] 返回多个值
来源：http://www.m.share.vehdjk.com/Article/details/gpteqsuau.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gokgvoebt.sHtML

PHP:  return [$a, $b];
来源：http://www.share.sjlbkw.cn/Article/details/gpkzhvvkg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.tarul.cn/Article/details/grxrtxfat.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gjcccavuy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.yfazqb.com/Article/details/gwcmzdrwh.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gobfbeclp.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/gitvooyxp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.tarul.cn/Article/details/gxfqxletz.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/gdvihxgew.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gsdlkwmlp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gmcuwtifs.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gpqynzqvk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/grflqtjkb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gvoeqdrfj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/gcoztzkbl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gmeiyzjvx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gnvsnwuhf.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.yfazqb.com/Article/details/gwnmdsapf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.tarul.cn/Article/details/gstgiaufo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/ghwmpcexq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gvzfggccd.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/gbbezvzcw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gcgozwjhb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/giyuzqunu.sHtML


<!-- 参考信息 -->