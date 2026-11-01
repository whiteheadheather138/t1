代发 wailian999

Ruby: value = data || "默认值"
来源：http://blog.bbcook.cn/Article/details/gudjfjbsb.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/gbwqnrzhd.sHtML

[A16] 真假值判断规则
来源：http://www.blog.yfazqb.com/Article/details/gexoyupvt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.tarul.cn/Article/details/gkzppxynj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.epnwcf.com/Article/details/ggcsttlld.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.vehdjk.com/Article/details/gabadiafu.sHtML

TS:   if (!x) {}
来源：http://3g.epnwcf.com/Article/details/grkxmmmcd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.bbcook.cn/Article/details/grgblnzzw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.tarul.cn/Article/details/gdkakcyeq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gggobvfym.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gbggimsgn.sHtML

[A17] 位运算
来源：http://3g.epnwcf.com/Article/details/gxudcysbh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gmlozaeca.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gxvbiisof.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gkgalgwpi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gzwopehfa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/glzczamna.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/grhkhirfc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gouashhfc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gtzilgkjj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.tarul.cn/Article/details/gkgdgsylc.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fktsv.cn/Article/details/gofbwgckx.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/glyerwhhl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/gzachbkwr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/gkixvzosj.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.sjlbkw.cn/Article/details/gyntejzvo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.epnwcf.com/Article/details/goitmgtoo.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.epnwcf.com/Article/details/gzjbywoii.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.epnwcf.com/Article/details/ghftzjwdk.sHtML

[A19] 交换两个变量
来源：http://baike.epnwcf.com/Article/details/gjyvlwqxp.sHtML

Py:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gdqlupxrq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.bbcook.cn/Article/details/ggoebdzco.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gowurbeug.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.bbcook.cn/Article/details/gtwjkqchn.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.bbcook.cn/Article/details/gsvsdxjxg.sHtML

Go:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gbiscgcfm.sHtML

Ruby: a, b = b, a
来源：http://m.share.vehdjk.com/Article/details/gnmqvwifc.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.bbcook.cn/Article/details/gbxmelwdt.sHtML

[A20] 读取标准输入
来源：http://wap.tarul.cn/Article/details/gqeyyqshs.sHtML

Py:   name = input("请输入：")
来源：http://www.share.bbcook.cn/Article/details/gomjunsul.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.tarul.cn/Article/details/glgrbqovy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.tarul.cn/Article/details/gtmeoqvum.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.bbcook.cn/Article/details/gnebxdjrr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.yfazqb.com/Article/details/gpnoczwdb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/gtzccqzad.sHtML

Ruby: gets.chomp
来源：http://www.m.share.sjlbkw.cn/Article/details/gkipbeyfx.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fktsv.cn/Article/details/gvpulkugr.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.tarul.cn/Article/details/gweswtbcz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gyloklpul.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gavjelyvo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/ghiovfwev.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gsmwagbsa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gaznhjbdj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gzhcngnjl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gmnxnsnjt.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.yfazqb.com/Article/details/gapayjnhj.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/gfkmnyvpo.sHtML

Py:   len(s)
来源：http://www.share.tarul.cn/Article/details/gnxqwwmjq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gorkabues.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/gdooaobqt.sHtML

TS:   s.length
来源：http://www.share.epnwcf.com/Article/details/gxgqwhrvk.sHtML

Java: s.length()
来源：http://3g.fktsv.cn/Article/details/gcvbyqjxg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fktsv.cn/Article/details/gpbsdboer.sHtML

Ruby: s.length
来源：http://blog.yfazqb.com/Article/details/grgbeocbf.sHtML

C#:   s.Length
来源：http://mobile.tarul.cn/Article/details/gcepgavxa.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gqjcjaaao.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.bbcook.cn/Article/details/gcxxhzbgn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.bbcook.cn/Article/details/gnakouyaq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/glzfunzzl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gnjtrzvvo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gynryrqcc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.bbcook.cn/Article/details/gozkkndlu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.epnwcf.com/Article/details/gsxprirkw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.tarul.cn/Article/details/gwmvykdtb.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.bbcook.cn/Article/details/gsqiqmhlm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fktsv.cn/Article/details/gzvjwfkhr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.epnwcf.com/Article/details/gdzazbiib.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gawlwbpwf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/gowrzikpk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.bbcook.cn/Article/details/gomoiwauc.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.epnwcf.com/Article/details/gaojwxnds.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.yfazqb.com/Article/details/glcabrdpg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.bbcook.cn/Article/details/gdnzjxvek.sHtML

[A25] 字符串比较
来源：http://mobile.tarul.cn/Article/details/grfuuwgdh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gmlbvcpxn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/gwohminla.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gvzzsroha.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gqwlofibp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.bbcook.cn/Article/details/gscqjxcqk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/geslywdwh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/gbxqumslz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gwgrmmqkj.sHtML

[A26] 类型转换总览
来源：http://wap.bbcook.cn/Article/details/gemaskvzn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.tarul.cn/Article/details/gzjrrkgpx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fktsv.cn/Article/details/gckpjezoz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.tarul.cn/Article/details/goowsulqw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/ghnqetcat.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/grbamomft.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.epnwcf.com/Article/details/gkritstys.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.yfazqb.com/Article/details/gikpdryng.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gkgcxqqwy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcvmynddq.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gdyysjjqd.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwymxivha.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.sjlbkw.cn/Article/details/ggwiwsppm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.vehdjk.com/Article/details/gzfndatsg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.bbcook.cn/Article/details/gybuhnytt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gxaonzxwt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/ggbhmbdmt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/ghziovquy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.bbcook.cn/Article/details/gccfjnvlf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.tarul.cn/Article/details/gworoajsl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gvngwzotb.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/govxzpoyy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gucmjojvn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gqqrxlokc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gdycrydlt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gxcqfdumc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gkhzwbhdx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/grtpotkbc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/gbqifuuzb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gxeqlbmki.sHtML

[B03] switch / match / case
来源：http://baike.fktsv.cn/Article/details/ggbgnxrio.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.sjlbkw.cn/Article/details/gmieiilqi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/goixrfwlq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gtsujpapy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmuljuwip.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gpvpopnvy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.epnwcf.com/Article/details/gbwgdokzq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.sjlbkw.cn/Article/details/gixwirapn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.yfazqb.com/Article/details/gzuzwcjxx.sHtML

[B04] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gtfthkyyh.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.tarul.cn/Article/details/gqlrumxyi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.tarul.cn/Article/details/gqyqnolqi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gahiutjpr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gyjlpckec.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.bbcook.cn/Article/details/gjhmomgzj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.tarul.cn/Article/details/gpfsvsbfx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/ghayjqvew.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.sjlbkw.cn/Article/details/ggekrxhgf.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gynzxgllg.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/gotgpoysi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gnoevwtge.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gkwzeknra.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gnoaujxsf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/gxwhagasf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.sjlbkw.cn/Article/details/gliketbbd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.sjlbkw.cn/Article/details/gcbpnkvat.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gyidqqiej.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gnwgmzsxv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gprfgybxh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/gxufumwrn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gokytvxoy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/ghxvfajgp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gsxufulkj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fktsv.cn/Article/details/gtakoboxu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gzahlwabm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gbpdfqbsb.sHtML

[B07] while 循环
来源：http://read.share.sjlbkw.cn/Article/details/gyxqwevyv.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gpqewxvfi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.vehdjk.com/Article/details/gnasdhcel.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gmidbygcv.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/glmqfmznz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gcakrwegg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/gokqfxyxp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.bbcook.cn/Article/details/ghhcyaawj.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gipejkylj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/gpuansjmn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.tarul.cn/Article/details/gwuaksbvf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fktsv.cn/Article/details/giloaanfu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gwdcmtlfx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/glmzilyej.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/ggoswxicd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.vehdjk.com/Article/details/gxsjixnal.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/giyzceain.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/glyucjmek.sHtML

[B09] break 与 continue
来源：http://baike.bbcook.cn/Article/details/gherxmtmc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.sjlbkw.cn/Article/details/ganpfcuif.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gzvxlmaoc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gjrebnppe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/ghgemvpmr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gqxnvjwky.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.yfazqb.com/Article/details/gpmvzmxbh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/glwnuuysk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gsmozlpwa.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/gezaapmxg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/gtovrdyea.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gspdtfvhb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gtftmdjto.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/goxuznvvf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gaesjxeqy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/gcmsakauy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/glkrtlcdg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gvuxgpssf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/gjbodolpx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gabjwcoqg.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gilpxofgj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gjosscbfn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gqfjcsbul.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gpebmhppd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/gqwlavguw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gzsdsdvez.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/grgkbrxog.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/glathvynk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gtyomtdgo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.tarul.cn/Article/details/gntgnwvhk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gpfluhfpn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gheipigqe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/ggsmofmcw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/gwoouwlya.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/goqnveebr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gbwyenkju.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/ggpconaju.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/gekeuzmvl.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gzexncdmd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gqcjxffrt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gygzvkavg.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gydjstatp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gkrcjyuqc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/grluennxr.sHtML

C#:   x is int or double or decimal
来源：http://blog.fktsv.cn/Article/details/gyhtkvxno.sHtML

[B14] 判断值是否在集合内
来源：http://3g.yfazqb.com/Article/details/giejvsurq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.epnwcf.com/Article/details/gcfirqanm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.bbcook.cn/Article/details/gbhashtdo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/glicwxlab.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/glhorcvhs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gihjnefgj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/gplblvyuy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/geehriveb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.epnwcf.com/Article/details/ggtncmfmg.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gqxaapjxb.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gyeezstkp.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gjkozumbd.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/ghcdvnazy.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/ghqiycgeh.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gwemtzubl.sHtML

Go:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gjirwgsmm.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gdmfylzvw.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/ggmtxrnfd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/ghokkcvrg.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/gjezkofzi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gklugikra.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyasqxnl.sHtML

TS:   if (!data) return;
来源：http://wap.bbcook.cn/Article/details/goiskddtb.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gshcbpmeu.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gaiuyymui.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/gqhrslzwb.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gkxdqhfss.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gabnrtpae.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/gnxihsfew.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxpohkenp.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gtyscjtcx.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gjtmkuucf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/griacvtvy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gjtrsfpab.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gagghljhg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gcveobjhq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/gdffhmlhg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/glcxxmadw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gsyjardcn.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gvwgoqaqr.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gizgazohs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.bbcook.cn/Article/details/gbvraglmv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gvoxagzhh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gibpiszmy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/glphxadow.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gtvtspkhh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/gjbviaoxc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/gyavegvax.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gjnwprxjp.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gohtzuqok.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gzabhcdgn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gyggnexql.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/grhudrehh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gbjilpycf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gnsdurjds.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gelcdzufd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gjlmgtaun.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gthyncfnu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/glzsqbssm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.tarul.cn/Article/details/gvhszrkyi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gchrbxlgl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/guevvkoce.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gjjpxpeov.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.epnwcf.com/Article/details/gvnubxmkh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/glcpnmcfu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gugfztpag.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/gkfwrfttl.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/guysnrdke.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gcscyearz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.yfazqb.com/Article/details/gulfchylp.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gebpiuihi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/ghmpjnkxm.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gsxxerztf.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/gnvmsikyt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.vehdjk.com/Article/details/gnjbdrpdh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gzzibgogz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.sjlbkw.cn/Article/details/ghsklhkwj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.bbcook.cn/Article/details/gzklqchrg.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gywcyfpre.sHtML


<!-- 参考信息 -->