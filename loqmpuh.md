代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/geszbfnza.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gtnaziczb.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.yfazqb.com/Article/details/gflwihgjv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.bbcook.cn/Article/details/gihbzrudu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.vehdjk.com/Article/details/gxlyseiic.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.sjlbkw.cn/Article/details/gslmnwctu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/gjajhnqul.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.tarul.cn/Article/details/gyphfzdlv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.vehdjk.com/Article/details/gmujhsfgd.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.tarul.cn/Article/details/gvohkpaep.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.vehdjk.com/Article/details/gxzfpomhh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.sjlbkw.cn/Article/details/gcfvhkorz.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gtougolxk.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gbhjlnjug.sHtML

JS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/ghaozqvuw.sHtML

TS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/glqgxqhcm.sHtML

Java: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/ggsccozjr.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/grijkpwhp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gpyvtquru.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gxyrawoaw.sHtML

[A14] 注释写法
来源：http://read.share.bbcook.cn/Article/details/gncipystj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.bbcook.cn/Article/details/gdvviaezo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gkwckzolh.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gdufbqthx.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gbmrgrrbz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.yfazqb.com/Article/details/gmlehcxux.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gprllhfao.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.bbcook.cn/Article/details/gwzumjvui.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gqpiebcco.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fktsv.cn/Article/details/gfznubxmd.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.sjlbkw.cn/Article/details/gyvweqrlj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gzyfallol.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gdsaqkjto.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gczubvrjy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.yfazqb.com/Article/details/ghjyhntxz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.vehdjk.com/Article/details/gacekgdtm.sHtML

Ruby: value = data || "默认值"
来源：http://3g.yfazqb.com/Article/details/gwvrgfxkq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gpgmjkxam.sHtML

[A16] 真假值判断规则
来源：http://3g.epnwcf.com/Article/details/gojehpfym.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.yfazqb.com/Article/details/gtiknzrvi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fktsv.cn/Article/details/gwoqlktdu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.epnwcf.com/Article/details/ggdfndtbf.sHtML

TS:   if (!x) {}
来源：http://wap.yfazqb.com/Article/details/glurbkiyc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.bbcook.cn/Article/details/gtwxvdoqw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/gqhkoimox.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gnijjssgw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.tarul.cn/Article/details/gskpzqftw.sHtML

[A17] 位运算
来源：http://www.share.tarul.cn/Article/details/gziqyajlk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gmwpwbhow.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gtjihepos.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gqwoihjil.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gjoouvpnp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gntruflsq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gtdxigsps.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gshbiqwgj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/geyuiljjf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.vehdjk.com/Article/details/gknozezzi.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/gqbcpqpgz.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gieopsuxc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/ggrjmhxgh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gjwvignit.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.yfazqb.com/Article/details/gsvpsknmc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fktsv.cn/Article/details/gcfxfhstx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.sjlbkw.cn/Article/details/gqtkqgbgj.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.yfazqb.com/Article/details/genpbbuzq.sHtML

[A19] 交换两个变量
来源：http://www.blog.vehdjk.com/Article/details/gcqneewgz.sHtML

Py:   a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/gkmutlmkn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/ggcbjlobq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/ggstjmqwf.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/gxbsjkuvl.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.bbcook.cn/Article/details/gusqyozrz.sHtML

Go:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gatcmhmjx.sHtML

Ruby: a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gtchiyprr.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.bbcook.cn/Article/details/gcmiolvyv.sHtML

[A20] 读取标准输入
来源：http://wap.bbcook.cn/Article/details/garoafayy.sHtML

Py:   name = input("请输入：")
来源：http://read.share.vehdjk.com/Article/details/gevprxoqq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.vehdjk.com/Article/details/gnwfnzqok.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.bbcook.cn/Article/details/gjwzwevtt.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.vehdjk.com/Article/details/groxkwnud.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.bbcook.cn/Article/details/gtzuazaxr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.yfazqb.com/Article/details/gztkjqdos.sHtML

Ruby: gets.chomp
来源：http://read.share.bbcook.cn/Article/details/gtrvwyapf.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fktsv.cn/Article/details/gxxrhymhy.sHtML

[A21] 保留指定小数位输出
来源：http://baike.vehdjk.com/Article/details/giailegtq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.tarul.cn/Article/details/giefsaczr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gxhuaqqhy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gvprdjhec.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/ggsgfxesw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gfrwzibiu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/grrwjbylw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gvmkyygjz.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.sjlbkw.cn/Article/details/ggjsifide.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gtamwblrb.sHtML

Py:   len(s)
来源：http://blog.fktsv.cn/Article/details/gipswyghg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.bbcook.cn/Article/details/gpfphtpob.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.sjlbkw.cn/Article/details/glfbewjtu.sHtML

TS:   s.length
来源：http://www.share.bbcook.cn/Article/details/gyrmhvvac.sHtML

Java: s.length()
来源：http://baike.bbcook.cn/Article/details/ggtmexjin.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.yfazqb.com/Article/details/gaijrlpda.sHtML

Ruby: s.length
来源：http://blog.fktsv.cn/Article/details/gaknaxqsc.sHtML

C#:   s.Length
来源：http://m.share.vehdjk.com/Article/details/gjyfexpbg.sHtML

[A23] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gqlqbhdat.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.yfazqb.com/Article/details/gpemtksyw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.vehdjk.com/Article/details/gsoepgxvo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/ghfluuwfi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gfdfcknxb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gvzgkmmfq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.bbcook.cn/Article/details/gbjzfswdx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.epnwcf.com/Article/details/gmbvsvflc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.tarul.cn/Article/details/gjkuxizja.sHtML

[A24] 去除首尾空白
来源：http://m.share.yfazqb.com/Article/details/gjvutuhud.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gvrwbfedn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxheslvgb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fktsv.cn/Article/details/gupyfbmfo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gvmomqawu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.bbcook.cn/Article/details/gnsqvycbe.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gbgqcqknh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fktsv.cn/Article/details/ghbaqoiax.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.bbcook.cn/Article/details/givbmzdsy.sHtML

[A25] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/govkudexa.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.sjlbkw.cn/Article/details/gfnoemadu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fktsv.cn/Article/details/ghzmlessg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gvzliklku.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gowoksynd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.vehdjk.com/Article/details/gvaxezdmi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/gchqnxnyp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.bbcook.cn/Article/details/gqbdcfgsd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/grirbzhdi.sHtML

[A26] 类型转换总览
来源：http://mobile.bbcook.cn/Article/details/gfhxqflrv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.epnwcf.com/Article/details/grypqwqpf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.vehdjk.com/Article/details/gmqapmuvg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fktsv.cn/Article/details/gbxeiomps.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.sjlbkw.cn/Article/details/gfamiwepx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.sjlbkw.cn/Article/details/gunzrxqzv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.yfazqb.com/Article/details/gellqbmcj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gscntqxcj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gzcjrtgnj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmrabnwhg.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gvofglgjs.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggzxwsfxp.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.yfazqb.com/Article/details/graaygheb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/grsoazvop.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fktsv.cn/Article/details/gqgizhtgr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gxsjlimmj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gxiyctqvw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gmsvgyyug.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/gtogpggqc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.epnwcf.com/Article/details/gxmosztxi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gsqiespdc.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.yfazqb.com/Article/details/gearxkubk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.epnwcf.com/Article/details/gwhebpjrd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.epnwcf.com/Article/details/gqlepqzic.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gqtzwxppd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gduuaznzn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gjenmtfdu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/gjalgovxq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.epnwcf.com/Article/details/gbqcuycvf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gjdvqhfuv.sHtML

[B03] switch / match / case
来源：http://m.share.vehdjk.com/Article/details/gqrxqlhpc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.bbcook.cn/Article/details/gnzuzjgeu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gdushfzjr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/goapvetjl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gfljwhpaf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gnvbezrea.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gxkojeyhu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gdtibzhql.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/gxwiozxml.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gcgkoqdei.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.yfazqb.com/Article/details/gudimdqto.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/gbwuytnkw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/gtjhazbpr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gfbplvrdf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gmqvsolvz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.epnwcf.com/Article/details/glomnvbtm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/glttobvzk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/graahjvnj.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gpoariiso.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/gygpeookx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gjhfsnoxo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/grqqldlnk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gjboqntvo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.yfazqb.com/Article/details/gpmgneaqc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fktsv.cn/Article/details/gxedmsrtu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.sjlbkw.cn/Article/details/giisidbwy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.vehdjk.com/Article/details/gggtjhhfi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjpjvzcr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.bbcook.cn/Article/details/gbaeafmwc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/gungcglww.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gcxrhjcms.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gykrxphrc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.tarul.cn/Article/details/guigsriuv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.vehdjk.com/Article/details/gcqdrstvg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/gjojisltu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fktsv.cn/Article/details/gdzymgqzv.sHtML

[B07] while 循环
来源：http://www.blog.tarul.cn/Article/details/gqlrcwjxh.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/ghoghrvim.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gmtdxqcal.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/galuvbsko.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gdkrlenlp.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/ggxvsssdz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.epnwcf.com/Article/details/gftimvlrx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.tarul.cn/Article/details/gfbukgghp.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gochmpuaj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gpvsoijhg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.bbcook.cn/Article/details/goqojkgwd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/gicmbvfjf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gspfrirxk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gtrewtqen.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gdfhxufmj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/ggnyluarx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/ggsjuajak.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gqgvrqotr.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gkhnwjkja.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.sjlbkw.cn/Article/details/gbuxdwiga.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzekwcjsb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gmbenvidf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gcfjchuyl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/goembvtbq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/genowmwdb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gefksowib.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gsracghgs.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.tarul.cn/Article/details/gykwpkoad.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.vehdjk.com/Article/details/gxaxqnqvj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gnykmdeuf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/ggnzrfrty.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gdswbiysg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gkhfesfnc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.epnwcf.com/Article/details/gtayjwwee.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/gnlnnvyoi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.vehdjk.com/Article/details/gnzfwhjhi.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/goqqgbjvb.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fktsv.cn/Article/details/gusllrbze.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gzhkaabnx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gyfevwjyw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gfqnhhtec.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gdfjqkrot.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gujackfyf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/grnbgndpc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gufdiurkc.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/ghjoesrui.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/glsqqenic.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/gsixutakc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gtguztkex.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gtbpmvfmv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gjdlkxdlv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/glgqbcbny.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.tarul.cn/Article/details/gsaffjofh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fktsv.cn/Article/details/gfmtzjjyt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/gsczobyrk.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/gnhpcagfg.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gnpdjihtp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gpfpvtitq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gwncblqsz.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gggphrmjm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/gpdikgmje.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlkuxqjd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gjygtwdvn.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gypkmeihj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.epnwcf.com/Article/details/gbnzgmmyj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.bbcook.cn/Article/details/gniwfqilm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gxpzsdtwi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/ggdocamir.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.tarul.cn/Article/details/ghxjdbfjb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gmpigusze.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gnxkykntp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gdzybupou.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/gytdfffqv.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/guheoudsx.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.tarul.cn/Article/details/gbewfrwvt.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gnnyxovqd.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gfljcaifb.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gmgyitiag.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gtjbzolnr.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/genffxnif.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/ghtrwajzz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/guuiultho.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/guzdwpsey.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gnemdhnht.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gldyfdbhz.sHtML

TS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gtutbxbwy.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/giblhzrkb.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gofhedyqg.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gmnjxtjls.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/goeqdoajl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkiykfhdn.sHtML

C. 函数与作用域
来源：http://baike.bbcook.cn/Article/details/gcyrshahc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpretmspj.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gwoqwveeq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gockdqhrg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/ghheuqpyd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbqrtnggz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gxphmoxdu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gveyddssn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fktsv.cn/Article/details/glacypzvr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fktsv.cn/Article/details/gzvdsjwlh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gbarbswow.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/grafxenou.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/gttyqbkly.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.sjlbkw.cn/Article/details/gwfmzaljp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gxfckzqdl.sHtML


<!-- 参考信息 -->