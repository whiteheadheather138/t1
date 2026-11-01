代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fktsv.cn/Article/details/gabzbscvy.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.epnwcf.com/Article/details/gnonfhorx.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fktsv.cn/Article/details/gktpyrnbo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.epnwcf.com/Article/details/guvidztvx.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gmfnscwwm.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gvonlmgqj.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gxchkjaqp.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gadaffblx.sHtML

Java: "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gklcitioh.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gaqcwpsrr.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gvssdznax.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gzjrwfcar.sHtML

[A14] 注释写法
来源：http://baike.sjlbkw.cn/Article/details/glwppjyrh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.sjlbkw.cn/Article/details/gvqtjuyoq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gtukfcpuc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gypvnqzrl.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gnjcpiekr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fktsv.cn/Article/details/gjhuhukqj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gqaoaarxc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.tarul.cn/Article/details/gnfkeshau.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gonxwmjyq.sHtML

[A15] 空值判断与默认值
来源：http://www.share.yfazqb.com/Article/details/grbjnzjyn.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.tarul.cn/Article/details/gxiiiddha.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gcwbqhzqr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/gudulzamy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gjcpagden.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.tarul.cn/Article/details/gtfphnpzu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.bbcook.cn/Article/details/gkwjsfpmx.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.vehdjk.com/Article/details/gakvuwmrt.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gjkqufzia.sHtML

[A16] 真假值判断规则
来源：http://www.share.sjlbkw.cn/Article/details/gpubqzrno.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.yfazqb.com/Article/details/gmjfsxezr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.bbcook.cn/Article/details/grvgxzflq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.sjlbkw.cn/Article/details/gsdoedctp.sHtML

TS:   if (!x) {}
来源：http://wap.fktsv.cn/Article/details/gwsnjfkfk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.bbcook.cn/Article/details/gsyfakkfj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fktsv.cn/Article/details/gbcmmvkmj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.tarul.cn/Article/details/gqlemmrxd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.epnwcf.com/Article/details/gtoceqbnw.sHtML

[A17] 位运算
来源：http://www.blog.epnwcf.com/Article/details/gbfcyrvep.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gittvgzkc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.epnwcf.com/Article/details/geceootjj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gfzjodarz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gqjnrdcdb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gnvjdpquc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gkzyrfmsy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gzsdiprxb.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gbxnzcura.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.bbcook.cn/Article/details/gzgkaosgf.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/gydqqmbuy.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/gulmfckja.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.epnwcf.com/Article/details/guqnjekye.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.epnwcf.com/Article/details/gtzsvbabm.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.vehdjk.com/Article/details/gtiktybig.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.vehdjk.com/Article/details/gopcwdpqx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.tarul.cn/Article/details/ggcokskri.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.tarul.cn/Article/details/gcomojghs.sHtML

[A19] 交换两个变量
来源：http://mobile.fktsv.cn/Article/details/gvjuuamwq.sHtML

Py:   a, b = b, a
来源：http://wap.tarul.cn/Article/details/glivdozwp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.yfazqb.com/Article/details/gvdmtpttt.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/glufhadxp.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gkprwlkgb.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.vehdjk.com/Article/details/ghhlbjhby.sHtML

Go:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/goxuympkp.sHtML

Ruby: a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gslwfxyqg.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fktsv.cn/Article/details/gmjeohutx.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/gbggheswr.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fktsv.cn/Article/details/gjxyemstf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fktsv.cn/Article/details/gmjxtuknn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.tarul.cn/Article/details/gdxrhptcv.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.sjlbkw.cn/Article/details/gurqjxhwa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fktsv.cn/Article/details/gusekufie.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.yfazqb.com/Article/details/glkxuryap.sHtML

Ruby: gets.chomp
来源：http://blog.epnwcf.com/Article/details/gfmuvfmjf.sHtML

C#:   Console.ReadLine();
来源：http://read.share.vehdjk.com/Article/details/gmozenauf.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.epnwcf.com/Article/details/goqhzzpsd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.vehdjk.com/Article/details/gkssqrons.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gxdqavkzy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gfozfosfk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/ghzutolji.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkzlqlhp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gkzmgxqhd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gzygfxndy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fktsv.cn/Article/details/gljvtsoxk.sHtML

[A22] 获取字符串长度
来源：http://m.share.epnwcf.com/Article/details/ggoxfjazk.sHtML

Py:   len(s)
来源：http://www.share.bbcook.cn/Article/details/gtdjrjeab.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.vehdjk.com/Article/details/giycxsfki.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.bbcook.cn/Article/details/gyjtlgsyo.sHtML

TS:   s.length
来源：http://mobile.epnwcf.com/Article/details/gswjypwny.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gfoyhtbny.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.epnwcf.com/Article/details/giyoemmnp.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/grthnxkke.sHtML

C#:   s.Length
来源：http://3g.epnwcf.com/Article/details/gzeiydhxg.sHtML

[A23] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gfbsolkui.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.tarul.cn/Article/details/gjwrlhpwp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.yfazqb.com/Article/details/gosfixyoi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gkunmaogi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gjterngjc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/grvwkeqqf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grecfnyfp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.epnwcf.com/Article/details/griluzept.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.tarul.cn/Article/details/giblsbqmk.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gdhlbpzdg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/gmdmmdrxv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.epnwcf.com/Article/details/gsodpfixd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gchshydgn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.epnwcf.com/Article/details/gishuuqhv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.sjlbkw.cn/Article/details/gjgdsslqi.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.bbcook.cn/Article/details/gifoztwvp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.bbcook.cn/Article/details/gqiwippxq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.yfazqb.com/Article/details/ghllhspdy.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gvducweyx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.tarul.cn/Article/details/gutohonzs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/gbixieaeb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fktsv.cn/Article/details/gejsbgqxq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.vehdjk.com/Article/details/gdbskrrqp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.tarul.cn/Article/details/gspeftcdq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gebnfdjrb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.yfazqb.com/Article/details/gewvpaiti.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/gveulcoqz.sHtML

[A26] 类型转换总览
来源：http://3g.bbcook.cn/Article/details/gxttssptg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gsvbotqxg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fktsv.cn/Article/details/ggjxoeamv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.vehdjk.com/Article/details/gjupjmwoi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.vehdjk.com/Article/details/gswnveyqi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/ghihodmed.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.bbcook.cn/Article/details/gwbikadps.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.tarul.cn/Article/details/gfdozwiyx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.bbcook.cn/Article/details/ggxljzoxh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gayujqqin.sHtML

B. 流程控制
来源：http://m.share.epnwcf.com/Article/details/gcrlajfob.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gduydofkw.sHtML

[B01] 条件判断 if / else
来源：http://mobile.sjlbkw.cn/Article/details/gfbmtxtqs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/gagxhjxbb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gtocrkrep.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gulgvzhwr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gpgwtaptt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gujhacbao.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/gzkbwuraq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gkkeatkrf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gfuzersmh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fktsv.cn/Article/details/gkampmsas.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/gravzpidz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.bbcook.cn/Article/details/gugonvasl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gvtiohhfv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/geodwgpij.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gkxyqgohw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.yfazqb.com/Article/details/gavlspapa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gyvnejtmb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gheggvqvx.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/gknxgdpow.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.vehdjk.com/Article/details/gptlnfygl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gulegqzeb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/ghneypmvc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gujlbqkjh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gcdyiperg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gsfelryfw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/gsvyesjcn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.tarul.cn/Article/details/gnbylkfet.sHtML

[B04] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gwknuhoid.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.tarul.cn/Article/details/gmxaezwcj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/gksybznqu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gnsnwnbii.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gxodrlsef.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/gtkbfugqy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.sjlbkw.cn/Article/details/gjazyygzf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.bbcook.cn/Article/details/gmmrykqro.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gospauqju.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gpxepfgfo.sHtML

Py:   for item in arr: print(item)
来源：http://3g.tarul.cn/Article/details/gsfaelxxu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.bbcook.cn/Article/details/gdfeipzda.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gdxidwpme.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gknfvzloj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.yfazqb.com/Article/details/gpamjrogc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/griindwpp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.epnwcf.com/Article/details/gjhywpnaz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gwmdtrchx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fktsv.cn/Article/details/guxmdrubm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/grbwyyfnk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfczciwbt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/ghooxbnup.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gibookynw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/gvztuargg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.sjlbkw.cn/Article/details/gzrhpeaed.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.epnwcf.com/Article/details/gtncuvfim.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fktsv.cn/Article/details/gascfcrxx.sHtML

[B07] while 循环
来源：http://m.share.vehdjk.com/Article/details/gvlefrzbw.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/guqgxnwwx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.tarul.cn/Article/details/gwmmwyvgf.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gejqgconm.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gnqosnspw.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gvenbmwvj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.bbcook.cn/Article/details/gxrwjpejo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gagtuknpv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/grpkudlco.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/gttuqoenb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/gmlpvvlfy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/ggvqklcgx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gcvinimnf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gldiymzzf.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gwomnqjjs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gohjirptq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.tarul.cn/Article/details/gbqxhcgxa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gjciznkhd.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gtkxuwsgv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/gbupuaoyc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gpcnmdphx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/geyieumex.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/grtkrubhk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gvnaqqemg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gcdbnnnwr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.epnwcf.com/Article/details/gviqxnwys.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gksrnmjww.sHtML

[B10] 遍历同时拿索引
来源：http://blog.sjlbkw.cn/Article/details/gdsuxoeud.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.tarul.cn/Article/details/gmgyhjsfq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/geqpkedgd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gobrjvlse.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gkfifotkj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/gfdxpuuax.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gfeqagbhw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gsljmnlzc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.epnwcf.com/Article/details/ghwhplbzi.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/gcqzcwbcp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gdbuorcgb.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gqmdzstxs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/ghuavjusf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gcroydhaf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.vehdjk.com/Article/details/gsxjrdmgl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gyqqjvbmd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gpnjlgdew.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.epnwcf.com/Article/details/gbeqskuyt.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/geksxtzmr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/gctyqgoxc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.tarul.cn/Article/details/gnssqlxbm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gouqwdcwq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gmychdmtk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gxyrysxek.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/gcsnbuzrq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.vehdjk.com/Article/details/gzfecyfwg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/ghizpgwli.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/gvjgrzoje.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.bbcook.cn/Article/details/gdnuqonha.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gyhvmnuoa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gbiiltqcn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gaxmspmam.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gwkjxwqrf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gwluresya.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.tarul.cn/Article/details/gqhruixwp.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gfldogmvy.sHtML

[B14] 判断值是否在集合内
来源：http://baike.tarul.cn/Article/details/gurjvhiuu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fktsv.cn/Article/details/gmqeeoexh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gsccasugx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gvgjhorqa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gpzcxvhrj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gqpdvrtbt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gvkyszbes.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gazhhmvso.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gcnjufvru.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/ggpqlzivp.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gggmvebcl.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/ghazsezwl.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gtuismwvc.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gzwpnyean.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gjclafmmk.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gdpqloskm.sHtML

Ruby: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gbycogqog.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/grnmdubip.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gbizfvxjk.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/gmcabaeoy.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/gweglhjvo.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gaqilcjwy.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gmryxrsbj.sHtML

Java: if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gwfrpdilu.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gcetsyaqg.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/gkfervnms.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gcmsjxijm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gllqoxpjq.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/ggeyvgsva.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvzilwxou.sHtML

[C01] 定义函数
来源：http://www.share.tarul.cn/Article/details/goudbyfjy.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/goxirxcso.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gayxsisth.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gpjmkeink.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gfpcnhciz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gkbtezlay.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gfoislrhf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.epnwcf.com/Article/details/gzkugwdqd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gjbqulwtf.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gtbgxrpsn.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/goicnmzsj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gviupmxhi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxegacvyf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gootuvcvv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gzrbnbxpr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/gpbqmyxxp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/gfonbmzlf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/ganhfqxhn.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/gajhvwqog.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/gtuymtiyi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gvgzairep.sHtML


<!-- 参考信息 -->