代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.epnwcf.com/Article/details/gfrwcwvsh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.yfazqb.com/Article/details/ghesizuhn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.yfazqb.com/Article/details/grrlwlqpi.sHtML

[A17] 位运算
来源：http://www.m.share.vehdjk.com/Article/details/gqrmkxpty.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gpkzqgctk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gdeyjjrwx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gbqbstrkf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gxidftgam.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/glmjaafqe.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gaumhhuwz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gfsccvlse.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gbmcwglxd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.vehdjk.com/Article/details/gwsjawtca.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gmsmwglql.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gzlvtqjmy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/gzwqtrlze.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.yfazqb.com/Article/details/gtmvgqlaq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.epnwcf.com/Article/details/gtzvycywg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.tarul.cn/Article/details/gnptvmbdq.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.tarul.cn/Article/details/glnsgcvlb.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.bbcook.cn/Article/details/gngnhcyfa.sHtML

[A19] 交换两个变量
来源：http://baike.bbcook.cn/Article/details/gtrjafshw.sHtML

Py:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gmqfcaqop.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.yfazqb.com/Article/details/gmlmzliwl.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/giaklskph.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gkurpbksk.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.bbcook.cn/Article/details/gizmlmnrg.sHtML

Go:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gtbmogawg.sHtML

Ruby: a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/grariojmr.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.sjlbkw.cn/Article/details/grjqzyyuq.sHtML

[A20] 读取标准输入
来源：http://blog.fktsv.cn/Article/details/garuibhnm.sHtML

Py:   name = input("请输入：")
来源：http://mobile.yfazqb.com/Article/details/gosgvwoci.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.yfazqb.com/Article/details/ggesnxrqj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.sjlbkw.cn/Article/details/gjpfuydds.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/gfgdjsejp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.sjlbkw.cn/Article/details/goxfujcmh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.vehdjk.com/Article/details/gyygpdrlm.sHtML

Ruby: gets.chomp
来源：http://blog.tarul.cn/Article/details/gakytydqx.sHtML

C#:   Console.ReadLine();
来源：http://m.share.bbcook.cn/Article/details/gsuepinpo.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.vehdjk.com/Article/details/gypddsjzm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gaacgzidp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gxlkoikzj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gqfqntxgj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gpfbtmuze.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gpilumbkc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gwgeexdvt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/ghvdzxmog.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.bbcook.cn/Article/details/gbteelgrr.sHtML

[A22] 获取字符串长度
来源：http://read.share.yfazqb.com/Article/details/ggxhvvcos.sHtML

Py:   len(s)
来源：http://3g.fktsv.cn/Article/details/gfsasqkmd.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.yfazqb.com/Article/details/ggfazeisk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.yfazqb.com/Article/details/gpctzlpkq.sHtML

TS:   s.length
来源：http://www.share.sjlbkw.cn/Article/details/gkqlicewp.sHtML

Java: s.length()
来源：http://mobile.yfazqb.com/Article/details/glkwycpyd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxdyjdony.sHtML

Ruby: s.length
来源：http://www.blog.epnwcf.com/Article/details/gyymyosez.sHtML

C#:   s.Length
来源：http://3g.tarul.cn/Article/details/gngsnilxs.sHtML

[A23] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gskqqxdsc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gncnwoljc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.epnwcf.com/Article/details/gxcsvmbun.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/glprvbdwx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gnxlnsymp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gorizobwj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.bbcook.cn/Article/details/gbqfqqfug.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gvlwdswnj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.vehdjk.com/Article/details/gvrhxwtco.sHtML

[A24] 去除首尾空白
来源：http://mobile.fktsv.cn/Article/details/gwxexyyiz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.tarul.cn/Article/details/gsefgohgj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.tarul.cn/Article/details/giukjzkoo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/gyiwkrdzr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gzzyecqnt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.tarul.cn/Article/details/gixowxxmq.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/gyuycbzdx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.sjlbkw.cn/Article/details/gwhusytqt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gebjpqvwd.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gnsuwdyyt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/gfrsekwnt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjffcibau.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gyldluhfb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gfzfuqehd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.tarul.cn/Article/details/gqsrkxnau.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gqgqgsgaz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.yfazqb.com/Article/details/gqediedvs.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/goczcvjef.sHtML

[A26] 类型转换总览
来源：http://m.share.yfazqb.com/Article/details/gmeirweft.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.sjlbkw.cn/Article/details/gyimdezrn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.epnwcf.com/Article/details/grjfjrqyd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.bbcook.cn/Article/details/gesgsbhkt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.yfazqb.com/Article/details/gwtierdyz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gbngvcxgz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/glhgfdemx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.bbcook.cn/Article/details/gdixiiagd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gswnqjuku.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grvfzvxcv.sHtML

B. 流程控制
来源：http://www.m.share.fktsv.cn/Article/details/gzwnvkhfo.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guwbbbosr.sHtML

[B01] 条件判断 if / else
来源：http://www.share.tarul.cn/Article/details/gcdaogtxj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.yfazqb.com/Article/details/gcdeyvrdy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.tarul.cn/Article/details/gybvvxnbt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gesxkceim.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/glwtwpbmh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/grzblzlsh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fktsv.cn/Article/details/goaqndkpk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.yfazqb.com/Article/details/gjpkjhpuj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gfsjegism.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.vehdjk.com/Article/details/gwjyhmhsn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.tarul.cn/Article/details/ghjwplgwr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gtehxjmzn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gtakicucp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gfoqkcfqa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/ghvrijnqp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.sjlbkw.cn/Article/details/gwxdlsojg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/gtfhmbbcc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/geepkdgrk.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/gbrfonbxw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.vehdjk.com/Article/details/guzxqwgvp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gfpjwwdvu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gqsfxwran.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gopvqqxgm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/godmncgte.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/gshcjibfm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gqkwcbnac.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/gmasviqdn.sHtML

[B04] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gburiyxyu.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/gfjhemebi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.sjlbkw.cn/Article/details/gtavwfafb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gimscfwbl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gvidcwndz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/glixsnvst.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.sjlbkw.cn/Article/details/gimjmuqnc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.vehdjk.com/Article/details/gmnwrtrpw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.vehdjk.com/Article/details/gajqaqlzw.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.tarul.cn/Article/details/guodyxgli.sHtML

Py:   for item in arr: print(item)
来源：http://blog.epnwcf.com/Article/details/gvwzeukry.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.bbcook.cn/Article/details/gzmwsusay.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gpsrfezyj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gzzqfenxe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fktsv.cn/Article/details/gjvnodwku.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fktsv.cn/Article/details/ghlequtuq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/gfpdmceeh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fktsv.cn/Article/details/gnhgyyfvi.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gmlxfemfn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gqnqufyaj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fktsv.cn/Article/details/gpehsryzc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gljrclnxa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gtwdvbfhq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fktsv.cn/Article/details/gcmejnuzx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.sjlbkw.cn/Article/details/gzmybxrqv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gargborjk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/ghisiozrj.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/guzrykpjf.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/ghffdkfnf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gwxcneyuw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gsppawewc.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gkpaoeqvk.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/glxfqyccn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.sjlbkw.cn/Article/details/gqkmiaofy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gfbhwkkou.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gmygnaxpy.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/gmrccscut.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.epnwcf.com/Article/details/gvbrmccmz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gssywzzok.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gcgojvufm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/guzabdlah.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/glfpzoeqc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.yfazqb.com/Article/details/ggfinfoij.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/gnfoewjjr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gnskxhcvs.sHtML

[B09] break 与 continue
来源：http://baike.sjlbkw.cn/Article/details/gsaejvsdu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/gtakmoxzt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gwjsgnril.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/ggacyfpin.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/glhroxdnx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/ganrgzumh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gbytdlsrg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gfazjzefk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/giuiqfgcb.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/gzldaujga.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gqsapyykw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gpdzeikui.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gajxwgrcz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gmufamkbz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gnzwjuhov.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/glvgxlhec.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gkwdirhpo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gynoyuimq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gsdrhvzry.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gxqtikdfa.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gjbjcddhr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gchdlwmgu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gwxwngiqn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpuuufcg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/gsqvoakiq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gmljhctgy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/gzshouihy.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gvtzjaspk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gasobokbl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.sjlbkw.cn/Article/details/gonwxfelx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gewwvimmn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gtprdhnyj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/goxrhvwau.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.tarul.cn/Article/details/gogkgrdvy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.bbcook.cn/Article/details/gtrprfgma.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gpprcrpum.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/gxgalrpqr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.epnwcf.com/Article/details/gqzsvuhqz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/gmmhnqyut.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/glpvvwvuf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gxajknauj.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/gleyseybg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.epnwcf.com/Article/details/ggeosounb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.bbcook.cn/Article/details/gdswxogct.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gasdupzbo.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/ggxhhekus.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gzgeheztt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fktsv.cn/Article/details/gwmpnbbro.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gfypliifh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gcagdmxwv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/giwkyxmpz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/grzaxrccy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gcvtiylip.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gdpahocab.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/gskvnnpqt.sHtML

Py:   a and b or not c
来源：http://baike.epnwcf.com/Article/details/gpimxdorh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.sjlbkw.cn/Article/details/gmedujcal.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gqejnkzyl.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gjirywfsu.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gwrdtkiqm.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gxddbdpys.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gqsyiqzaz.sHtML

C#:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/ghomwjxds.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gxugdhnmw.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/gwxaiyoop.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gbonjeczj.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gwxckjmxq.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gmxmmwjrn.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gwtmjzcre.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gljwcfjhk.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/gzmshlmce.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gquqlphey.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcgamvbln.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/ghbcojwmo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gadkilsgl.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gghweuvyk.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gmaejkhoa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gyuniqqnd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gztvfijmg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/glraltdjw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gnfvtpopq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.vehdjk.com/Article/details/glmfuugsg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/gqhopapkz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gtlhijfin.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gefqkkoxc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gtaxqhaql.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gvpktscqw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gdbybohhn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/ghxlrgspe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gzlbnqaxp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/glojodfqx.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gwdugzcld.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gbkitqgcn.sHtML

[C03] 可变参数
来源：http://www.m.share.bbcook.cn/Article/details/gzgbyxgrr.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/ggqdhvjar.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gmaufofwg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gwvzjuddb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gpatfciog.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gvjdpciex.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gyijnczip.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gspuivewk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gcsyndgrl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/grwwzxgnf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gfslssezx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.vehdjk.com/Article/details/gyqwzpolv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gavqtyexf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gezljruwm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/gwxqacewa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gtynyfhrq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/geyrjqutu.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gcwdmosyo.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gssjaaqjq.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gahvsduul.sHtML

PHP:  return [$a, $b];
来源：http://blog.epnwcf.com/Article/details/gfhukntag.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gyltowwpx.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gvriiehsx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gvcujgxfo.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gnpzukpzp.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gnkdesdqc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gmvoardgh.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fktsv.cn/Article/details/gjskgxcqp.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/gadnaierd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gtrezicqm.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gbcjqsiwv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gdvyjscjs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.epnwcf.com/Article/details/grbtznsbw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fktsv.cn/Article/details/gmmozdfqz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.yfazqb.com/Article/details/gxymvscor.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gurdaztih.sHtML

[C07] 把函数作为参数传入
来源：http://baike.tarul.cn/Article/details/gvzwiwtav.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/gvtpmfrhv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gmfofnpzg.sHtML


<!-- 参考信息 -->