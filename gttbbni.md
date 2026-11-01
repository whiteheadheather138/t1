代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.yfazqb.com/Article/details/gaeuayjks.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.tarul.cn/Article/details/gutqwyism.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/gvqdgsfff.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.tarul.cn/Article/details/gyxfjhvql.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.tarul.cn/Article/details/gzxvsueuv.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.sjlbkw.cn/Article/details/gohhtilco.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.yfazqb.com/Article/details/ggjcwfgjy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.bbcook.cn/Article/details/glgyjlqsu.sHtML

Py:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gsbiigwaq.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gdzswawop.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gsdikpssl.sHtML

TS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gplrslwab.sHtML

Java: "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gvzlegtdf.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gpelrwpxk.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/galxmvgrs.sHtML

C#:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gyhzrwnpj.sHtML

[A14] 注释写法
来源：http://mobile.epnwcf.com/Article/details/gowolqrjr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.bbcook.cn/Article/details/gmpizmoaq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gxjqqhbfn.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gxbdfydwg.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gaxmdxvbk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.epnwcf.com/Article/details/gyiolaoky.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gwydtmjeb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.tarul.cn/Article/details/gxxcbswzz.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gxtjwwspv.sHtML

[A15] 空值判断与默认值
来源：http://read.share.yfazqb.com/Article/details/glvyeabka.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.bbcook.cn/Article/details/gxijirgmy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/gwytzxjdc.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/ghjmwzznx.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gbwwuotmk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.vehdjk.com/Article/details/gomfyxzsa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.bbcook.cn/Article/details/gkqxlnesi.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/gacbwmyye.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gvpeapmew.sHtML

[A16] 真假值判断规则
来源：http://m.share.vehdjk.com/Article/details/gssduwmju.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.yfazqb.com/Article/details/gdkftcztg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.tarul.cn/Article/details/gmsfrioui.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.yfazqb.com/Article/details/gszwxptbu.sHtML

TS:   if (!x) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjccpsuul.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.vehdjk.com/Article/details/giugboopn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.yfazqb.com/Article/details/glhbkfeio.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.tarul.cn/Article/details/ganasuawd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fktsv.cn/Article/details/gjtfizzek.sHtML

[A17] 位运算
来源：http://www.m.share.fktsv.cn/Article/details/gzrkiqnql.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/grpjzicse.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fktsv.cn/Article/details/grgvqxyiw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gvkkymmcm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gczcpqhyg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/ghctxjbfj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gcrlcnvth.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/goaqexgiz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gkycyaddz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.tarul.cn/Article/details/guflstude.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.bbcook.cn/Article/details/gpunferkh.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gluvcgvzw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.bbcook.cn/Article/details/gtgqalljb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gqtumuuhq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.epnwcf.com/Article/details/ghormymkp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.tarul.cn/Article/details/gkgezquht.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.yfazqb.com/Article/details/gvdkvjlyb.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.yfazqb.com/Article/details/gkgnqnzod.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/gljmosagh.sHtML

Py:   a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/ghqefjcsu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.sjlbkw.cn/Article/details/glyyfojpv.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/gxsaqqtrn.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/gydrvtjhv.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.tarul.cn/Article/details/ggtjqfsha.sHtML

Go:   a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gduyeqcqe.sHtML

Ruby: a, b = b, a
来源：http://wap.epnwcf.com/Article/details/gpuawvzjk.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.bbcook.cn/Article/details/ghabsweom.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gwncqktxk.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fktsv.cn/Article/details/gpugunxkg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.vehdjk.com/Article/details/gtxbppyup.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.epnwcf.com/Article/details/gmdbsgcoz.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.vehdjk.com/Article/details/glrclzhxs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.sjlbkw.cn/Article/details/gkfuhrcnz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.yfazqb.com/Article/details/gsicnuiqj.sHtML

Ruby: gets.chomp
来源：http://read.share.fktsv.cn/Article/details/gygjkhwlv.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fktsv.cn/Article/details/giacsdslh.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.yfazqb.com/Article/details/gnjqgqcic.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.epnwcf.com/Article/details/gxouokhhv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gucsgpzfm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gyvieuclc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gwfssbdls.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/goltnjxqq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/grjbsdkic.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gletddlvo.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fktsv.cn/Article/details/gvjzoxldm.sHtML

[A22] 获取字符串长度
来源：http://mobile.bbcook.cn/Article/details/gbddtcofy.sHtML

Py:   len(s)
来源：http://wap.yfazqb.com/Article/details/giqhpogul.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.epnwcf.com/Article/details/gdzeswcrs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gbsvzjthm.sHtML

TS:   s.length
来源：http://www.share.sjlbkw.cn/Article/details/gaynpkult.sHtML

Java: s.length()
来源：http://blog.fktsv.cn/Article/details/gghucvfho.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gfvlvkysk.sHtML

Ruby: s.length
来源：http://www.blog.tarul.cn/Article/details/gvtvgicoa.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/gmmjrwclp.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gbzjyzmni.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.sjlbkw.cn/Article/details/gzrjabyjw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/gpjzwvnba.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/grzngjlas.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gvqrlchua.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gpsfquiak.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.epnwcf.com/Article/details/gdkwvatfu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gbxalbywf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.tarul.cn/Article/details/guiwcnzyr.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.epnwcf.com/Article/details/gvegjgnfj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.bbcook.cn/Article/details/gcfdcuxwf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.bbcook.cn/Article/details/gkslzkcvw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/ghcghnhnd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gjxiiorqp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.yfazqb.com/Article/details/gbgkjfvuh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.bbcook.cn/Article/details/gldqnbzax.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.sjlbkw.cn/Article/details/ggnysloty.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.bbcook.cn/Article/details/gvsoeiouf.sHtML

[A25] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrfipzjz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fktsv.cn/Article/details/gsblepuyy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.epnwcf.com/Article/details/gxyzouwsa.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gmuhboebh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/ghcwttmka.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.vehdjk.com/Article/details/gvudewdbl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gfbpbkwcs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fktsv.cn/Article/details/gumrwuuos.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gzqudbbbd.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gfsgqljgl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/ghlfcpxoc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.sjlbkw.cn/Article/details/gvunmsqzo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.bbcook.cn/Article/details/gkuwprrdr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.yfazqb.com/Article/details/gkmznjxqp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gqwkhuqyg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fktsv.cn/Article/details/gnckbydfu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gmqfhloxx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/goxyqjeit.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqbrrombu.sHtML

B. 流程控制
来源：http://blog.tarul.cn/Article/details/gflconpzc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsauofwtu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.bbcook.cn/Article/details/ghsdmsiaf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/galcoekqt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.epnwcf.com/Article/details/gclpqakbf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gvejybybz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/geejczwil.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gxmhjhbqh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.bbcook.cn/Article/details/ghndwqkle.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gtasebudw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gcuuidcxd.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fktsv.cn/Article/details/gyirtxksn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.sjlbkw.cn/Article/details/gwivtsfya.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.vehdjk.com/Article/details/gjkabzyqa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gqwiygtzj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/grcsxkaey.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gskrqtbkb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/gfhhbhkam.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gjhrfstoy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gyqijgmqc.sHtML

[B03] switch / match / case
来源：http://m.share.tarul.cn/Article/details/giwywxxck.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gprmshdsc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/guvtypkwn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gggueabmn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gbzftaicf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gysirnwjz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.bbcook.cn/Article/details/gmpzjvsdg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gqsaovjlr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fktsv.cn/Article/details/guvxqkndl.sHtML

[B04] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gbgmccmhp.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.tarul.cn/Article/details/gwbsfessn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/gvviupirt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gpbenrgvu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gephbffon.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gojnmewim.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/gagmnwxmu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fktsv.cn/Article/details/gtxsyjpnt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.yfazqb.com/Article/details/gecihwnnd.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gadkoplvl.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/guhnrpxjr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/ggxdoupxw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/govmjwsie.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/grvjdpujo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gfmujopcp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.tarul.cn/Article/details/gnrnawpfa.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fktsv.cn/Article/details/gqdffkjaq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.yfazqb.com/Article/details/gwtrufihl.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.vehdjk.com/Article/details/glbriqtwf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gvvlunnel.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.bbcook.cn/Article/details/gjhhnglbx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/ghyjnwewb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gefhvzchj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.epnwcf.com/Article/details/gfmgotxux.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gpghiunvp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gtjvemljk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gdawghdlg.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gsdkudivc.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/gexfhltme.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fktsv.cn/Article/details/gxgyhzdhr.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/grgckeewq.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gogpqufcz.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gggafqaph.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gltjwwoyc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gvoofqhry.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gwwossocm.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/gshlotvno.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gjenddzpy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/gdvymznqv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/galiirrki.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gyvbpopva.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/grklnxifh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fktsv.cn/Article/details/gxdpphleu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gqeyhumqz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gwiqdzhfb.sHtML

[B09] break 与 continue
来源：http://www.share.tarul.cn/Article/details/gtzbntnxz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fktsv.cn/Article/details/gnwumfnct.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gzblsqfev.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gpivxjrcq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gnmxujczb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyvbnbujk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gyyiwoobl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/glqsygrhz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gkiindsjh.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.sjlbkw.cn/Article/details/gummzewlj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gcbclipmd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/grwbgmrmq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gphwxmfzq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gnzalkgck.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/gnfygtkcj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/gosdotrbs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/glmuqxisy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/girwllqgd.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.bbcook.cn/Article/details/gydppvqmp.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/gbrwsimmb.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fktsv.cn/Article/details/gsbzwafsw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gslniidmp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/glmfbeftq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gogxmbfpz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gieamjbfh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gjgeqfwdk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.bbcook.cn/Article/details/gpnigkqbu.sHtML

[B12] 跳出多层循环
来源：http://read.share.yfazqb.com/Article/details/gputliyyg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.epnwcf.com/Article/details/ghzngoavl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gmynlarmz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gynwisuzi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/giccyflzd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gufvdcpnw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoyyfpuu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/govcsjvtq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/gpaczryay.sHtML

[B13] 判断是否为数字
来源：http://3g.fktsv.cn/Article/details/gzlktepjw.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fktsv.cn/Article/details/gtjrjjcwm.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.vehdjk.com/Article/details/gzsrvuwbv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gxmtfqnid.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gonyjbhzm.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/glanksdbs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.epnwcf.com/Article/details/gujfzjude.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gytfdsgdm.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gnerfdrgq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fktsv.cn/Article/details/gjeqdrtew.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gjxszutlj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvykbwvr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gadfbuwfe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gxenxztwe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gkfzzegzf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.yfazqb.com/Article/details/grewpxsax.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gbskvhziy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gwrndlcfr.sHtML

[B15] 布尔运算与取反
来源：http://blog.vehdjk.com/Article/details/gnjwnglep.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gbriygvbp.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/gekfjjltq.sHtML

JS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gpdxeeidu.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gwbzyehtz.sHtML

Java: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gczgcbcvy.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/grumwxkff.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/guaklaniz.sHtML

C#:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gviqkffom.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gstddexfj.sHtML

Py:   if not data: return
来源：http://wap.vehdjk.com/Article/details/gnhmvtlzv.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.epnwcf.com/Article/details/gplrotbsu.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gbgfifwft.sHtML

TS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/graecpqna.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gheveywce.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gqvvxahyz.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/gwoucgcek.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/ghpqgtupm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grosggfrs.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/gnuqtlcct.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtvfgqmgw.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gobicfthe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gwpukdgjn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gnimugblg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/glntiojec.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gwlkghbxv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gklyjzhid.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gdjjapqyy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gdtzkhdwm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gcnkwydyd.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gyosjckuq.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.epnwcf.com/Article/details/gaqsqdpwz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gdnycsiir.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gxhntofhu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gcwojzwus.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.epnwcf.com/Article/details/ghzxnkqnh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gyotklfqg.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/gcnsuklej.sHtML


<!-- 参考信息 -->