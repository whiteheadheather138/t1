代发 wailian999

Ruby: value = data || "默认值"
来源：http://wap.fktsv.cn/Article/details/givbdlmqu.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gxafdwmwg.sHtML

[A16] 真假值判断规则
来源：http://3g.bbcook.cn/Article/details/gynuyanrb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.yfazqb.com/Article/details/gavprzdgb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.yfazqb.com/Article/details/gilflpztp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.yfazqb.com/Article/details/gdvyetswf.sHtML

TS:   if (!x) {}
来源：http://m.share.bbcook.cn/Article/details/gfvveikrv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.vehdjk.com/Article/details/gdlpgajkc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.vehdjk.com/Article/details/gtkjmxwzn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fktsv.cn/Article/details/gecdryfpu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.yfazqb.com/Article/details/gqcypkeck.sHtML

[A17] 位运算
来源：http://wap.tarul.cn/Article/details/gvofqbkux.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gqxbgcwur.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.epnwcf.com/Article/details/gxkwsuvyd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gkznyhhtq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gmkgcqwgr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gocswvqvu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gigmgnkui.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gjukkoays.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/ginykgwvy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.tarul.cn/Article/details/gzjglfslt.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/grejcfwmp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.vehdjk.com/Article/details/gnxyrxwtd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.bbcook.cn/Article/details/gmruhncrh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtznpgesz.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.vehdjk.com/Article/details/gbkjztski.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.vehdjk.com/Article/details/grvprudan.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fktsv.cn/Article/details/gktudtlqz.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.tarul.cn/Article/details/gzfhynxct.sHtML

[A19] 交换两个变量
来源：http://blog.fktsv.cn/Article/details/gobghifjn.sHtML

Py:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/ghcyritpq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.sjlbkw.cn/Article/details/gtssbaaao.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/gqhasvlmi.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gymrcqfzp.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.tarul.cn/Article/details/ggcvjxqfr.sHtML

Go:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gzhuyuvzc.sHtML

Ruby: a, b = b, a
来源：http://wap.bbcook.cn/Article/details/grcoabjtv.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.yfazqb.com/Article/details/gmtcttvsv.sHtML

[A20] 读取标准输入
来源：http://read.share.tarul.cn/Article/details/gngamztpd.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/grergjclr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/gwuaradlg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.bbcook.cn/Article/details/gdatqwxbr.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.tarul.cn/Article/details/gmfmqbfpx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.bbcook.cn/Article/details/gyqqpzozi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.epnwcf.com/Article/details/glbktabad.sHtML

Ruby: gets.chomp
来源：http://www.share.bbcook.cn/Article/details/gkmxqehzt.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.bbcook.cn/Article/details/gxccjnfdb.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.epnwcf.com/Article/details/giecidjbi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.vehdjk.com/Article/details/giaisqqil.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/giyvynmiy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gfbwbdpmx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gfbbnkyak.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbxpbihs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gofuramiw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gmtyizslw.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.sjlbkw.cn/Article/details/gnkuycrgu.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.tarul.cn/Article/details/grthqodsw.sHtML

Py:   len(s)
来源：http://baike.epnwcf.com/Article/details/gipypopsn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.tarul.cn/Article/details/gycxsfmnj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.epnwcf.com/Article/details/gtgdjpfiu.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/gzuxpexag.sHtML

Java: s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gwffufmxa.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.epnwcf.com/Article/details/gfavpqrxy.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gtixeeyxb.sHtML

C#:   s.Length
来源：http://baike.fktsv.cn/Article/details/giemnhkwe.sHtML

[A23] 大小写转换
来源：http://baike.fktsv.cn/Article/details/glwkoptmn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fktsv.cn/Article/details/guzjorhvz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/gmikpkhyg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gscqcnndi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gdzxvbqfw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gqohuxnsr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.sjlbkw.cn/Article/details/gajzyzjzz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gdjhdcdrw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.sjlbkw.cn/Article/details/gjmywkaos.sHtML

[A24] 去除首尾空白
来源：http://www.blog.bbcook.cn/Article/details/gaxfxxjpm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gjcbyvkeq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/gpgqpoxem.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/grkfjhxpn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.epnwcf.com/Article/details/gmccezzdo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.vehdjk.com/Article/details/grufrrcjg.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.tarul.cn/Article/details/gjujzdnow.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.sjlbkw.cn/Article/details/gynddsrcj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.tarul.cn/Article/details/gndhtsshv.sHtML

[A25] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gneqietfd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.yfazqb.com/Article/details/ggngoeczy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.vehdjk.com/Article/details/glvcyswsj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgnxacpc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/gbavvvwox.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gpjwuqiim.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.tarul.cn/Article/details/gwwxsbawg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gclvucmgw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/ghsetgpeb.sHtML

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/grmhnxyig.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.vehdjk.com/Article/details/gdrsrdjiu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.sjlbkw.cn/Article/details/ghnizxipm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fktsv.cn/Article/details/gjicghcag.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gighpvdbx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/geyrazgbf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fktsv.cn/Article/details/gwjhszysp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gwkmiucon.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/giqjpxuuc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzhvaxejx.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gpgfeihvj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxilxgzyv.sHtML

[B01] 条件判断 if / else
来源：http://mobile.vehdjk.com/Article/details/gvpkquolg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gelzrroys.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.vehdjk.com/Article/details/ghhoorpif.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/goyrnlrwr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gjwutprje.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gitcayiky.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.tarul.cn/Article/details/gxxaxwfjw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/ghvdlsjrt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gibwylyfy.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fktsv.cn/Article/details/gzzauiuhr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gofqqasmh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.vehdjk.com/Article/details/gmwhskgwk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gdfaibrza.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gtgnkrvyx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gmbthtipo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/goemtvoqr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.tarul.cn/Article/details/gsmgjjxxf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gfojgfgtf.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gykvwczgs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.tarul.cn/Article/details/gcjafdgon.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gbjldvpyt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gfalrvlka.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gcuieyuzk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/grwxkmfpo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.tarul.cn/Article/details/gyweplhue.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fktsv.cn/Article/details/gnesbdetn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gioperoju.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gglhjfrgd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.tarul.cn/Article/details/gvyjjjdjc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.tarul.cn/Article/details/gjckgshvg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gdiukortd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/goxrnvpte.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/gqcmlvslv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.epnwcf.com/Article/details/gzyifumpr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.tarul.cn/Article/details/gmlwszidp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gabdcgwaa.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gaoxdwdvu.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/gwanowpkc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.tarul.cn/Article/details/gausxbdgu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/govrngmis.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gfkeoegwz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.yfazqb.com/Article/details/gkuzwwhrv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/ggkfwfzpb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/ghcimogwo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/ghgmhruko.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.tarul.cn/Article/details/gdsaqbiwp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gixrawika.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/geymfhupj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gmoylriuw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/gilhltqjw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfnaqhmos.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fktsv.cn/Article/details/gsmfuvqby.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.yfazqb.com/Article/details/gxtcyefry.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.yfazqb.com/Article/details/grulymryi.sHtML

[B07] while 循环
来源：http://www.share.yfazqb.com/Article/details/guqxfgoop.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gowpattos.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.yfazqb.com/Article/details/geklmeswr.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gbszjjpbr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gpntyfprs.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gqnkyrnzi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.epnwcf.com/Article/details/gobcwvqbj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.tarul.cn/Article/details/gychbiwnr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gptjlipxh.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gfxvvbtdj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gchqkjjkb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.vehdjk.com/Article/details/grgazrxoi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gvpigskai.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gbewygqph.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gebtwtcpm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gptbfezpa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fktsv.cn/Article/details/gtsuaoaqu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/ggbdrrgff.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/geyngctni.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/gnbvittui.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gdqrsftfe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gyqdghhvc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/glgfiozen.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gznericrm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/ghdkusrtz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.yfazqb.com/Article/details/godddbkmv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gsjrocckn.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gxqrdudmt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gvtayombt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gafixikrg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gnitsojkg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/geylnozdf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gbmntahdk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.sjlbkw.cn/Article/details/gpdxuujvs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gzgoycktc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.tarul.cn/Article/details/gtlbcgcja.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.vehdjk.com/Article/details/gaegqjhoc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.sjlbkw.cn/Article/details/glmvinevj.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.vehdjk.com/Article/details/gzkrekptu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/gbknzpmip.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gqfoghccj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.yfazqb.com/Article/details/gzikdosqg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gwhubcyor.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.vehdjk.com/Article/details/gtxbeynpt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gwqdynpro.sHtML

[B12] 跳出多层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gclfyuxsx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gxatrxnaq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/gnfueedvb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gibnopaks.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gxduucovo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gjfnksymq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/ghzblagia.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gzxuzaewj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/grksdtjni.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gbeuasxie.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fktsv.cn/Article/details/ghoqxqnrw.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gbdzvsvay.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gufasevxy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gokfigqee.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/grdimfhuv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.vehdjk.com/Article/details/gnmqjcqqt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.epnwcf.com/Article/details/gdliraypx.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gicjhoxjb.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.yfazqb.com/Article/details/girqlyzad.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/glmwxbkgh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fktsv.cn/Article/details/gxcosktpb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gebxkxmgd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gppbgzdwt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/gwupmypmj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.tarul.cn/Article/details/glrqszcgs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gipbglbdv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghujsdvfy.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gtqwjqymo.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/gddcwyieq.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/gsrplbsyo.sHtML

JS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gtwbtomhl.sHtML

TS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/ggbmxdbnx.sHtML

Java: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gshlngvyd.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gxnkllhgk.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gkgszhwfq.sHtML

C#:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gegqajszx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/ghnbialta.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/gbykvrvdn.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.vehdjk.com/Article/details/gbpgktfkm.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gzkmfcpjx.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gemrifjiy.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gjlnuuolu.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gsjyfysmo.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gexriyjfm.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gadcrjdtt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggevxadvp.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/gpxmfyhcp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghkmykbyx.sHtML

[C01] 定义函数
来源：http://www.blog.tarul.cn/Article/details/guevzyivl.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/gwgxnzaul.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gcebzuqfk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gawgnvxvi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/guldxwaza.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gbianlrpj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.tarul.cn/Article/details/gjbgtsfvg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gyarreshz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gskeifitw.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/ghwpkpikv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/guxsmwerq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gqlczfwcf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gfhxrwxsv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gollyfspp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gglvhfeay.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.tarul.cn/Article/details/gznejpqdy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.yfazqb.com/Article/details/ggzwtdvbd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gwtavudpq.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gergzhmyu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gqbrpjrmq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/gwwayngyk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gepszgheb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gktpsepwh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gqyuqdovv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gukkmmrff.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gizwwmeqm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gdnjexkqx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gvbdhpfen.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/gpycybfxi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/ghnzqeukm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/ghdvckvhi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fktsv.cn/Article/details/gfzyahjcm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/grymbrekw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.sjlbkw.cn/Article/details/gnrcyrotd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/ghdpdcudm.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gvvzinykk.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/gcriikpmt.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gkoymahre.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/guvwmemfu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/guspfogus.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gwmkbaxms.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fktsv.cn/Article/details/gqcbzpegl.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gsqbqsdda.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/glbeoiivp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gqvummafo.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.tarul.cn/Article/details/gavcepegm.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/gvtvzgtrt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gwntwlvqy.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gkaytwnnm.sHtML


<!-- 参考信息 -->