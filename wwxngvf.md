代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gktdvtpwf.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gymzruark.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gkzxtzhdi.sHtML

TS:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gzeydjljk.sHtML

Java: "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gfpbmtncr.sHtML

Go:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gczslviho.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gufealupz.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gvbdzlxjf.sHtML

[A14] 注释写法
来源：http://www.blog.tarul.cn/Article/details/grfdykpwl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.vehdjk.com/Article/details/gbvzhppbs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/ggkcsycfy.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gesqrmxyb.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/grxpmajjo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.tarul.cn/Article/details/gzfwxktpb.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gzjnjdwdp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.tarul.cn/Article/details/gbklcuqbs.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gfrqunvgj.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fktsv.cn/Article/details/gelfyyffj.sHtML

Py:   value = data or "默认值"
来源：http://blog.fktsv.cn/Article/details/gxoynmixy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/gwkziuryg.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gebjhnjmi.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/ghgqnbeub.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.epnwcf.com/Article/details/grgcvhlix.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.tarul.cn/Article/details/gygntmueu.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.yfazqb.com/Article/details/gfxnnqpuk.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gmsgtvhdg.sHtML

[A16] 真假值判断规则
来源：http://www.share.yfazqb.com/Article/details/gfvpqqlov.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.epnwcf.com/Article/details/gedhmketj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.bbcook.cn/Article/details/gpcayqwxr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.tarul.cn/Article/details/gexbhplxs.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gmttmqoyw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.yfazqb.com/Article/details/gjptqzbfh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.vehdjk.com/Article/details/gijrgxntb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.vehdjk.com/Article/details/glcukruhz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fktsv.cn/Article/details/giujijwtf.sHtML

[A17] 位运算
来源：http://blog.epnwcf.com/Article/details/gtlyqpcdz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gtnzqnuhc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.tarul.cn/Article/details/glulqafqb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gabeezdbc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gchwtthgl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gulfdafrm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gppcocyui.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/glhzqxdzn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/ggyltisht.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.tarul.cn/Article/details/gvqqmaeci.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fktsv.cn/Article/details/goifmrann.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/gydnjjzju.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.yfazqb.com/Article/details/grjvvgoqp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gexacpiqx.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.sjlbkw.cn/Article/details/gfaqbwupi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.tarul.cn/Article/details/ggnrvdndn.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.tarul.cn/Article/details/gjkateukj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.tarul.cn/Article/details/gqtmnsbzx.sHtML

[A19] 交换两个变量
来源：http://baike.bbcook.cn/Article/details/gywqrjiqz.sHtML

Py:   a, b = b, a
来源：http://www.share.yfazqb.com/Article/details/gclzwszzk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.tarul.cn/Article/details/gpczissxh.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/ghicbojvv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/ggdivcakf.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.yfazqb.com/Article/details/gifkqgyti.sHtML

Go:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gxthdfarc.sHtML

Ruby: a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/grbtiiwrc.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.tarul.cn/Article/details/gmvezehjs.sHtML

[A20] 读取标准输入
来源：http://read.share.sjlbkw.cn/Article/details/gvktcizao.sHtML

Py:   name = input("请输入：")
来源：http://www.share.tarul.cn/Article/details/gehhrodko.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fktsv.cn/Article/details/glainxrjb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.epnwcf.com/Article/details/gfgwenqiz.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/ghsbxtpkb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.tarul.cn/Article/details/gvsxnzjls.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.vehdjk.com/Article/details/gwcwfltwu.sHtML

Ruby: gets.chomp
来源：http://wap.sjlbkw.cn/Article/details/gtnjptlwh.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/gfxndlnpy.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/gydoegipo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.yfazqb.com/Article/details/grhaarotk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gidpvjovp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gvveqpydh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/ggqlzaqfq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gcpejianp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gtbutktus.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gzafolejv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.vehdjk.com/Article/details/gwzbxbvpi.sHtML

[A22] 获取字符串长度
来源：http://www.share.yfazqb.com/Article/details/gwwdbtdck.sHtML

Py:   len(s)
来源：http://blog.tarul.cn/Article/details/gslegrxph.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.tarul.cn/Article/details/gmuuewqpz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fktsv.cn/Article/details/ghcqtjovk.sHtML

TS:   s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/ghagzrqti.sHtML

Java: s.length()
来源：http://baike.bbcook.cn/Article/details/gaaopikad.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.sjlbkw.cn/Article/details/gtouvfrbd.sHtML

Ruby: s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxecdcly.sHtML

C#:   s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gvmtbvndl.sHtML

[A23] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gromthlsm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.tarul.cn/Article/details/glhigydcf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.tarul.cn/Article/details/gxjtthcqt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gojiipzbe.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gunzivthf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gqeqdeyno.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.bbcook.cn/Article/details/ghumgcaev.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gtqyxlrjd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.sjlbkw.cn/Article/details/gcmgrbmqe.sHtML

[A24] 去除首尾空白
来源：http://www.blog.sjlbkw.cn/Article/details/gfibeanfd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fktsv.cn/Article/details/ggihsoofo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.bbcook.cn/Article/details/gkovlzefj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/gnqbgdfev.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.bbcook.cn/Article/details/guwaeqgnf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.epnwcf.com/Article/details/gpyiyoqcr.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.epnwcf.com/Article/details/grvmplszs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.bbcook.cn/Article/details/gemqrkakv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyumxagj.sHtML

[A25] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gpodzhrvy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/gbprhggja.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/ggzexbgri.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/ggidsfhim.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gglybusxi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.vehdjk.com/Article/details/gphrgedjy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gqgjduiri.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/grwmaaodf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gltrevvwx.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/gkmctzixy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.vehdjk.com/Article/details/gwihrbrew.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fktsv.cn/Article/details/gkygrtzpn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gwhkjyocm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/grthtliqp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gifyukzzv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gkmfarecp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.epnwcf.com/Article/details/gfkkscslv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/gghmuernj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggahpxrow.sHtML

B. 流程控制
来源：http://baike.yfazqb.com/Article/details/gxqywyqdq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtfsozqzn.sHtML

[B01] 条件判断 if / else
来源：http://baike.epnwcf.com/Article/details/gwhvcnwmj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gqspvkzuq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.tarul.cn/Article/details/gpwndlfiv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gddxwdrvh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gfwwyxeis.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gbiprbuju.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fktsv.cn/Article/details/gsmfddbyy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/gndyifavs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gejiyjypr.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gcvndxzfb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.tarul.cn/Article/details/gurgezqbk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.vehdjk.com/Article/details/gfqdpfial.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gyrnbwpsw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gahbnvbyy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gmpadqpko.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/gwesghcis.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.epnwcf.com/Article/details/gcawrdkde.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/glxkxihni.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/ginbhfpvn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fktsv.cn/Article/details/gepyhzsdq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gtaimbcdw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gbuboegia.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gikmeypvg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gndimkpjr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gjoblzpue.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.sjlbkw.cn/Article/details/gvtmkatje.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.yfazqb.com/Article/details/garxtgtwc.sHtML

[B04] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gohwhqqrf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gmxxlbpud.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gimksajbl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gijowcxys.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gtcspetkz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gknlywqkm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/gcduhwxqs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.vehdjk.com/Article/details/gnvqaholr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fktsv.cn/Article/details/gfofupuos.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gxyqsncob.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.tarul.cn/Article/details/gdkqktghv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.yfazqb.com/Article/details/glwbyvpbj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gojptogey.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gaswbbjvf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gndymsvsf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/gxzxaragj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gsevkclzp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.tarul.cn/Article/details/gelvlzbmf.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fktsv.cn/Article/details/gxwyoidav.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.tarul.cn/Article/details/goefuvubu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gwgjrmpbj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gpnmpublv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gcqpjkdpy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/girtdxokb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.bbcook.cn/Article/details/gwxnynjur.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.sjlbkw.cn/Article/details/gzdwuyeid.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/gjconkwyr.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gbpvugwyk.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gvkewhfee.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fktsv.cn/Article/details/gmhvrftri.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gkqoeqiks.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gpiwokfwc.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/glblgvcie.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fktsv.cn/Article/details/ghyyusoim.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/gmuakzxnl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gqncsxwaf.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.epnwcf.com/Article/details/gckceammo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fktsv.cn/Article/details/gbytfygnf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/grgssffnv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gzmuyrxkz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gokucvhxx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeqowhzv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/goulxauva.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/ghhotggmt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/ghpvsgrbd.sHtML

[B09] break 与 continue
来源：http://www.blog.fktsv.cn/Article/details/gbvgtwvko.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gcdmxxtvz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/ghitvibkx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gnykmwipr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gsbbpnwrs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gtjgllmvd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gwfoootqq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gdrtbjymw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gvsyzezwx.sHtML

[B10] 遍历同时拿索引
来源：http://baike.epnwcf.com/Article/details/gfpvqykzv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fktsv.cn/Article/details/gvxnxtmas.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gtdbjgpnu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gudkzjhed.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gaznystwu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.bbcook.cn/Article/details/glfalxvaw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/gkirvimht.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/gxtkmcphf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gfsdkhcmm.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gmwjvdybc.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/gwaerdpuh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gazfhlarw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gtapkkntk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/grtjtioow.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.bbcook.cn/Article/details/gyhhebtqb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.sjlbkw.cn/Article/details/gosmfksoh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.epnwcf.com/Article/details/gtzpdaawk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/ggrbyspui.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gzthzthlx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gicoviiue.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.tarul.cn/Article/details/gipwwozyc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gxojodqft.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gdvhabrdt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gjfwvjdhu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/glvsxsmlx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gwtofvawk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gofkdjcsq.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gnbopwwkr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.sjlbkw.cn/Article/details/gjabdwhna.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/gmaeufued.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gsgtygwrw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gupqfcwkd.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkfadnrh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/grirunjzz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gyyufivrn.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gvrwtgqwt.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gxkhutyfl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gbsaqyjyu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.yfazqb.com/Article/details/gqeywrhkx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/ggetjekmm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gwcwscrap.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gyonslidp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/gyikicegi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.epnwcf.com/Article/details/gcxkrhwzh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyikieha.sHtML

[B15] 布尔运算与取反
来源：http://m.share.bbcook.cn/Article/details/gxqkzyojw.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gsiahgyer.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/gjilgsjqx.sHtML

JS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gldcvowmq.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gjyecmvje.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/guqckvicf.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/galsirnwx.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gdxehaifi.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/giogkbisv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/glenphtrm.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/gyhqegfrk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.tarul.cn/Article/details/gftmvuozd.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gsyjhushd.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gzewqfyle.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gvkhcalci.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gabjqnquw.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/gqwdnqnuu.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gfhkikvga.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gaodmrtan.sHtML

C. 函数与作用域
来源：http://mobile.yfazqb.com/Article/details/gxmfzgoyk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gduizpumo.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gxdgqyytb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/gpiyscaid.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gsyevbira.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gqlawynup.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gpzknrisj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/getgztoxk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.bbcook.cn/Article/details/gohrjvjbw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.bbcook.cn/Article/details/ggfcawayi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gsnvmjasr.sHtML

[C02] 默认参数
来源：http://baike.sjlbkw.cn/Article/details/gmipxgtho.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gsyagnayw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gdiewovqw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gkdbmaknf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gasbzobkn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.tarul.cn/Article/details/gxhdohuwz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gfltxefah.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/gdgshtxpb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gcqxnqmoy.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/gzvsnrkwt.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/gugarelpx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/ghpsrnegg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gqhrcxdiz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gjcqhbagz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gwrvnrvzw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/grnzzmftd.sHtML


<!-- 参考信息 -->