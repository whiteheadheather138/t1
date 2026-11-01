代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gfdjsznmm.sHtML

[A15] 空值判断与默认值
来源：http://baike.epnwcf.com/Article/details/gothogvbj.sHtML

Py:   value = data or "默认值"
来源：http://mobile.vehdjk.com/Article/details/gxbhgvjlu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gzfofxnaf.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gevrroefm.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/glnvqdaem.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.epnwcf.com/Article/details/gygaoujnw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/gqnnpaiho.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.epnwcf.com/Article/details/glcyqlbgb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gyvbhyvjg.sHtML

[A16] 真假值判断规则
来源：http://www.share.tarul.cn/Article/details/gutxpmxtp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.epnwcf.com/Article/details/gosxbbene.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.bbcook.cn/Article/details/gimkdurea.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.tarul.cn/Article/details/gmaxsrmmg.sHtML

TS:   if (!x) {}
来源：http://wap.bbcook.cn/Article/details/gmlyvdapm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fktsv.cn/Article/details/gqszoatzo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.vehdjk.com/Article/details/gpqowlfef.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.sjlbkw.cn/Article/details/guoenxobh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.bbcook.cn/Article/details/gmooopgum.sHtML

[A17] 位运算
来源：http://mobile.bbcook.cn/Article/details/giugqcutc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gqdjxkkaj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.vehdjk.com/Article/details/gtgezskhz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gcklbhzyw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gaklmxtfu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/glyuubsyg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gdmztfomv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/galvvernp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/giblkpagm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.vehdjk.com/Article/details/gtwwlvauz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gidelrszc.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/gmxdptplk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gsvgflfmz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gtztueien.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.tarul.cn/Article/details/gyxhgigir.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.vehdjk.com/Article/details/gcvuphmqp.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fktsv.cn/Article/details/grijifayo.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.yfazqb.com/Article/details/grbmlgfih.sHtML

[A19] 交换两个变量
来源：http://m.share.bbcook.cn/Article/details/gsquslhgo.sHtML

Py:   a, b = b, a
来源：http://read.share.vehdjk.com/Article/details/gadqrgyjj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.epnwcf.com/Article/details/gyxjoolwe.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/gpwecepsx.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/gjiigrhqk.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fktsv.cn/Article/details/ggynbkoko.sHtML

Go:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/ghlggeomc.sHtML

Ruby: a, b = b, a
来源：http://wap.tarul.cn/Article/details/gqimtdsjj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.sjlbkw.cn/Article/details/gctbryjpl.sHtML

[A20] 读取标准输入
来源：http://www.m.share.vehdjk.com/Article/details/gfyapogrj.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.epnwcf.com/Article/details/gxeogvnmi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.yfazqb.com/Article/details/gojrurghx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.vehdjk.com/Article/details/grqkvdulp.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.sjlbkw.cn/Article/details/gejdcylma.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.vehdjk.com/Article/details/gjmmrcxoq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.yfazqb.com/Article/details/gdnfvfshd.sHtML

Ruby: gets.chomp
来源：http://blog.sjlbkw.cn/Article/details/gttianbva.sHtML

C#:   Console.ReadLine();
来源：http://m.share.tarul.cn/Article/details/gqucjkqmy.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.epnwcf.com/Article/details/gkswlphdp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.yfazqb.com/Article/details/geuabamda.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gsucrubjp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gkglwoiya.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gvcyapywy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gorwjitrm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gjxnfyzty.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gwchozfbi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.sjlbkw.cn/Article/details/gavpomztc.sHtML

[A22] 获取字符串长度
来源：http://mobile.fktsv.cn/Article/details/gukmgawbt.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxhvmgbsl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.bbcook.cn/Article/details/gtoxvcapp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.yfazqb.com/Article/details/gvfqbxgne.sHtML

TS:   s.length
来源：http://baike.tarul.cn/Article/details/gzutdpjvy.sHtML

Java: s.length()
来源：http://baike.bbcook.cn/Article/details/gobfnfteq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.yfazqb.com/Article/details/gxqqbthmw.sHtML

Ruby: s.length
来源：http://www.share.bbcook.cn/Article/details/gevkquebm.sHtML

C#:   s.Length
来源：http://3g.bbcook.cn/Article/details/gyprwvqis.sHtML

[A23] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gpzntmgya.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fktsv.cn/Article/details/gbvggkefw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/gpgysznqu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gmqttbmab.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gkokejyee.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/gkuoohuij.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.bbcook.cn/Article/details/gtyqldxqm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gldxsngyl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/ghxdgdwzq.sHtML

[A24] 去除首尾空白
来源：http://www.share.bbcook.cn/Article/details/gxlkxzurf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.bbcook.cn/Article/details/grbrxdslm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.tarul.cn/Article/details/gfhkjrdtt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/gqwbmtofd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/grsnaguoo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gzddxyimi.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.bbcook.cn/Article/details/grjdwbpzl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/ggdzzrevd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gvgssektj.sHtML

[A25] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gyjknqvzn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gxywvplwc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.vehdjk.com/Article/details/gwtzbjvkt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gisncphwv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gsnutdokr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gumfkwugl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gvkwxmkhh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.bbcook.cn/Article/details/grdaajjun.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gudkjgadf.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/gwljrapcb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.vehdjk.com/Article/details/gnkmnmtpq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.epnwcf.com/Article/details/gorhpjebb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gteueumtx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fktsv.cn/Article/details/gfdalhhgz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gfwqescxi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/gtlntthyx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.tarul.cn/Article/details/gqnzenwpn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gdolrmeun.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqalyzgvv.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gvykqrgas.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbxfetsdi.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gxcffmmhs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhlbkxee.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.vehdjk.com/Article/details/gnjbcvgsc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gsevtuifj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/geiypifux.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gfeiiuslg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/gaiopfhmn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.vehdjk.com/Article/details/gcuoerths.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gjkbndrbl.sHtML

[B02] 多分支 else if / elif
来源：http://baike.epnwcf.com/Article/details/gzalmiijg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.epnwcf.com/Article/details/giakpstxm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/gxfdjebmr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gdgnkfdfm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gfpwoacxq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/glamthwnr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.tarul.cn/Article/details/ghjznlfex.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.yfazqb.com/Article/details/gvohkjubt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gqerblmek.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gnldlnlbr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.vehdjk.com/Article/details/gxihlyyrl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gkrgfmqbs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gswqxfiah.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/glmcrmdec.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gdjvcodxs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gglzcpedh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/ggcgosgcu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/guugxribq.sHtML

[B04] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/giajgkljn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.vehdjk.com/Article/details/gdvuxuwlt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.epnwcf.com/Article/details/gkrmqgoln.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gbnkrsvlc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gvsnvvgie.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.sjlbkw.cn/Article/details/gbeyoeezz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.yfazqb.com/Article/details/gzynnidbq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.epnwcf.com/Article/details/gkcusjdtx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.epnwcf.com/Article/details/ggqofojmg.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gneuotfcb.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.yfazqb.com/Article/details/gmcmclluq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gidfybrkv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gmfmqesuv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gjcrsifvt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.yfazqb.com/Article/details/gexxmgfrw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.tarul.cn/Article/details/gfbwdwgli.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/gtrhpbfsu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gblocafdz.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.yfazqb.com/Article/details/golgbavgh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gejaeivei.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.sjlbkw.cn/Article/details/gpkbmhtgm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/glhwsbilo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gxeeqambt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.yfazqb.com/Article/details/gitwasidj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.yfazqb.com/Article/details/gebothsut.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.yfazqb.com/Article/details/gkxcpkcob.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gvqzrjigy.sHtML

[B07] while 循环
来源：http://mobile.bbcook.cn/Article/details/gwetwqikf.sHtML

Py:   while i < 10: i += 1
来源：http://blog.tarul.cn/Article/details/gphapndaz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gecqxibvi.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gcvqbpyif.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/ghgkuzlfw.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gqrcblpbc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/guplvlvlp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/grfvxgwdg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gchiubyqw.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/ggolpwvvh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gxxbxkxdd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/ghgimwjck.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gdvizwcah.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gncthnenx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/grrxtgasg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.yfazqb.com/Article/details/grexdholt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gnvorvbpc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gacgsbugc.sHtML

[B09] break 与 continue
来源：http://wap.yfazqb.com/Article/details/gttzegchp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/gvmqnxjqj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvcntevr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/grnwrofyc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gsyzrojrm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gasufmuwd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/gcsnwfmwf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/ggvcpuxjm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gesnudvwe.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.epnwcf.com/Article/details/gwlzlhnyb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/gnfdkrpra.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fktsv.cn/Article/details/goeaiszpw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gydoqljvl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gomfwznnd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gkxpmevnh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gqkgagkpu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gqvhevbiv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/geamaswaf.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.sjlbkw.cn/Article/details/gnliwtjls.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.epnwcf.com/Article/details/gcfqubyde.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/gljkiwesx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gcyapaapw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gcbcrcqbf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/geyiadezp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/ghbkylsey.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gbjduggfu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.yfazqb.com/Article/details/gzdhoggfk.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/grdmnjree.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/gbalvausx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gfynulecq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/ggnlbqnul.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gyoijmkho.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gagixunoo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.tarul.cn/Article/details/gutdvsson.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fktsv.cn/Article/details/gndkonpwm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gupbomcuu.sHtML

[B13] 判断是否为数字
来源：http://m.share.vehdjk.com/Article/details/gwrlgreun.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gxzuxgnoz.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gehxfycmk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gzfnuaqwt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gemgpbgng.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/ghdndzgwj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/ggckczoby.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gxowwipoi.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/gxhyoksak.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/ggfelfezz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/gdzaonsfi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/gmzydmgzc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/glcwblugj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gsmvhhvtx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/geezefcsb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbafmpduj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.tarul.cn/Article/details/gsdtfppuk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gjssvsopj.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gquvtbqxb.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gmjyvgnzn.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.sjlbkw.cn/Article/details/gfayvrges.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/glmcqxuti.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gzbuccprf.sHtML

Java: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/ggturqsbk.sHtML

Go:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gyufcdgvn.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gtvmttigh.sHtML

C#:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gbblxfwic.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/guzpzyjvx.sHtML

Py:   if not data: return
来源：http://read.share.epnwcf.com/Article/details/gxzfzasyb.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gccjdicgf.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gumhocatx.sHtML

TS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gazavndli.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gkfoecxxf.sHtML

Go:   if data == nil { return }
来源：http://wap.tarul.cn/Article/details/gjyyhzwuc.sHtML

Ruby: return if data.nil?
来源：http://blog.bbcook.cn/Article/details/gdjivwnnn.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/ghwazsobo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grldfexnt.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gfryrkehf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/glwqmusjx.sHtML

[C01] 定义函数
来源：http://3g.fktsv.cn/Article/details/gbhslrquf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gpglhvipk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gtadnlcaf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gbocmwecz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/glajkbbns.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gthpnjmrn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.epnwcf.com/Article/details/gaslmfuzw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.bbcook.cn/Article/details/gdhalrbqq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gfohqfyjv.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gzjhbioor.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/gcmoymhld.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gbehaqyxw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gpuxcnewn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gdvjfyitd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.yfazqb.com/Article/details/gkeezojhl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/gzhjfigdu.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gxsrmbxqq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gqiljxfio.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gxzzzrtrl.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gacdqfsdu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gjohbishz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gndrdeyxw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gsqjnofhp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.tarul.cn/Article/details/guuhqlcrv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gkjgsdvxl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/gzutscxrv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/ghcwrcpzs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.yfazqb.com/Article/details/gbalwbamr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/ggvvociih.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gkwczvtzu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gktxkoyhx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.bbcook.cn/Article/details/gyfbgnlvf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gwveodqfy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gpupnozmo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gqkjxubxw.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gsrqrgbjl.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gktwtmukl.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gmtshnwxy.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gjqquzsfv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/ghsodvfup.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gavfzsxwq.sHtML


<!-- 参考信息 -->