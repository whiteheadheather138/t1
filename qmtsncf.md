代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fktsv.cn/Article/details/gqaqkebht.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.yfazqb.com/Article/details/gweicmgqz.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fktsv.cn/Article/details/gmhfqrixn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.vehdjk.com/Article/details/gjyzoigmv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.bbcook.cn/Article/details/gufnkpxya.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.yfazqb.com/Article/details/goykanazd.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.sjlbkw.cn/Article/details/gwizfosqz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.sjlbkw.cn/Article/details/gjgkqxdeo.sHtML

Py:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gjsvnfrpw.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gjrogojha.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gcbqqpzyl.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gydqxldlz.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gmezkjcts.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/ggfyxsyzk.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gekzmusjj.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gylhmcypa.sHtML

[A14] 注释写法
来源：http://wap.bbcook.cn/Article/details/gdgvkwmlf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.yfazqb.com/Article/details/gjsrmykrw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/geptrieow.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gvpgovrxp.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/ghusajbnk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.yfazqb.com/Article/details/gpvyhkowi.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gcemumpyw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.yfazqb.com/Article/details/gbdgaxyms.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gtyxqzbyx.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/gplejqkta.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.sjlbkw.cn/Article/details/gudvcjphe.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gztjmgwtp.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gvuqibsok.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fktsv.cn/Article/details/gnmdfovlh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.epnwcf.com/Article/details/gtjfdlfta.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.vehdjk.com/Article/details/gbiscpikr.sHtML

Ruby: value = data || "默认值"
来源：http://wap.bbcook.cn/Article/details/gjekaotxr.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gheqzgqhb.sHtML

[A16] 真假值判断规则
来源：http://www.share.sjlbkw.cn/Article/details/gqodggqlw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.epnwcf.com/Article/details/grzkfelho.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.epnwcf.com/Article/details/gyezniazb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.bbcook.cn/Article/details/gxexmepho.sHtML

TS:   if (!x) {}
来源：http://m.share.bbcook.cn/Article/details/geqqcgnzm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.epnwcf.com/Article/details/gfddlxgez.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.bbcook.cn/Article/details/gytefvhje.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fktsv.cn/Article/details/geimdkplf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/gzdaewmtf.sHtML

[A17] 位运算
来源：http://blog.vehdjk.com/Article/details/gbbakvsqj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gvvahqkig.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtcmrmuk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gacwukcqd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gpicmivhc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/glpfaxbxz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gcovbmkcn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gtbedaexp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gnbvgjxqb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.bbcook.cn/Article/details/ghltmeecv.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/geqcibkxd.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gmbklqhjj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gzxgczlcy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.bbcook.cn/Article/details/gxtlcarlw.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.epnwcf.com/Article/details/glmlerkha.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.tarul.cn/Article/details/ggxuwuqqb.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.yfazqb.com/Article/details/grexvgljw.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.bbcook.cn/Article/details/guhhybtrd.sHtML

[A19] 交换两个变量
来源：http://wap.sjlbkw.cn/Article/details/gncpqlibu.sHtML

Py:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gnuhixarp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.epnwcf.com/Article/details/gxowdxahz.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.sjlbkw.cn/Article/details/gonhwsqzf.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gbfakltnp.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fktsv.cn/Article/details/gvcalpiqp.sHtML

Go:   a, b = b, a
来源：http://3g.tarul.cn/Article/details/gzowguync.sHtML

Ruby: a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/giquxdqvv.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gbuintgnd.sHtML

[A20] 读取标准输入
来源：http://m.share.yfazqb.com/Article/details/gbatearut.sHtML

Py:   name = input("请输入：")
来源：http://baike.fktsv.cn/Article/details/gsuhcynxc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.epnwcf.com/Article/details/gekxmynlt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.tarul.cn/Article/details/gbhbgljjc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.sjlbkw.cn/Article/details/gsjkvchwc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.bbcook.cn/Article/details/gzzvijezv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.sjlbkw.cn/Article/details/gumghikqa.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gdsljxmyl.sHtML

C#:   Console.ReadLine();
来源：http://www.share.tarul.cn/Article/details/gwfdyxmtf.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/gzcqcoiyy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.bbcook.cn/Article/details/gdytsxxhf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gbzgkjyet.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gokhpqvkk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gybdhttek.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gndinccky.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gtkqcrmon.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gwezsbsdn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.tarul.cn/Article/details/ggfegsgja.sHtML

[A22] 获取字符串长度
来源：http://www.blog.tarul.cn/Article/details/gmyvylpdo.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/geiqzdjts.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.sjlbkw.cn/Article/details/gsknvksbw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fktsv.cn/Article/details/glmutmmih.sHtML

TS:   s.length
来源：http://www.share.bbcook.cn/Article/details/ghoxzkqti.sHtML

Java: s.length()
来源：http://read.share.yfazqb.com/Article/details/gqyyztehc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fktsv.cn/Article/details/gfeklvcfu.sHtML

Ruby: s.length
来源：http://www.m.share.bbcook.cn/Article/details/ghjnfzjdm.sHtML

C#:   s.Length
来源：http://www.share.yfazqb.com/Article/details/gxffdxrnp.sHtML

[A23] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/grdcgtkmm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.sjlbkw.cn/Article/details/gjtvostfg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.yfazqb.com/Article/details/grfxskmko.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gvowjejxb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gikvhigtc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gtdxczrmy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.tarul.cn/Article/details/gpgpjmdhw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gpgltvqhv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.vehdjk.com/Article/details/ggkstwecy.sHtML

[A24] 去除首尾空白
来源：http://mobile.sjlbkw.cn/Article/details/geshswars.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/gvvubdxif.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.epnwcf.com/Article/details/gaugbulqb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gqqgtpyoe.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gxndwvhjd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.yfazqb.com/Article/details/gjrqksqrs.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.tarul.cn/Article/details/gqatzwxqn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.bbcook.cn/Article/details/gkcgthfus.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.sjlbkw.cn/Article/details/glrakcpph.sHtML

[A25] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gxkrcrafh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.vehdjk.com/Article/details/gmaswmbop.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.epnwcf.com/Article/details/giyyegqkg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gvjkntluc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gedahctzs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gjenvrhjl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gaxwgsbws.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/ggyzspihp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/gulevsxpb.sHtML

[A26] 类型转换总览
来源：http://wap.epnwcf.com/Article/details/gzwmhpxut.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/ggngdnxfn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.vehdjk.com/Article/details/gxbuoagfg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.sjlbkw.cn/Article/details/gjhvrteno.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.yfazqb.com/Article/details/gzvgnarjq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/giwnnonav.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.vehdjk.com/Article/details/gtgeimved.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.sjlbkw.cn/Article/details/gnaefyjzh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.tarul.cn/Article/details/gkfufyxug.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwzsvswmr.sHtML

B. 流程控制
来源：http://wap.fktsv.cn/Article/details/gtmcpvjff.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glroepmda.sHtML

[B01] 条件判断 if / else
来源：http://read.share.epnwcf.com/Article/details/gpdbdbfku.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.vehdjk.com/Article/details/gwfmldngt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fktsv.cn/Article/details/giefpfkre.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gkrnulpwm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gijqogkdv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gtiqfeyri.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.sjlbkw.cn/Article/details/gqxjiyxoe.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.sjlbkw.cn/Article/details/gqjjtjlew.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/guyrvqlvh.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gdyshoxzj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/glnguguwu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.vehdjk.com/Article/details/gwdvlmpvs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/greaememe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gzrfgejff.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gdiwbbobf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.yfazqb.com/Article/details/gghxtwiyr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/glxvegasx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gxvrubuaq.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/gdaztvmwm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.bbcook.cn/Article/details/gsnarwios.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gqktubimj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/goqxkzwlu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/ghvalyfoc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gqvyisdps.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.vehdjk.com/Article/details/gwllycedj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fktsv.cn/Article/details/gnexmaupa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.tarul.cn/Article/details/gghqwqzjt.sHtML

[B04] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gzzsyihxw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gkhubvxqx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.tarul.cn/Article/details/gjucoqypn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gfztvztli.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/grrizddto.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gzwdenrtr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.epnwcf.com/Article/details/ggdpgrnlf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.yfazqb.com/Article/details/gkmchnjce.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gqpakdoxn.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gwrcaoqef.sHtML

Py:   for item in arr: print(item)
来源：http://blog.epnwcf.com/Article/details/gzfsdnurx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.tarul.cn/Article/details/guvbmpjkt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gtxfaqoba.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gquhpuxau.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gzrdazozo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gdnzcgqco.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/gzrqulqpm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/ggdcuesnj.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gkrpslfdx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gyrvfvlqq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gdacjidne.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/ggncoyuzy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gvjlvtqiy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gvwhrlolv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.tarul.cn/Article/details/glvurvupg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.bbcook.cn/Article/details/gnjoowwdn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/gwuihaxzy.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/ggieqjysl.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gbbsyzihr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.yfazqb.com/Article/details/gtqcrbbaw.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gskxyjpqs.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gwsggxtky.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/grshahhup.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/gqeagiprk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/gqvwtabds.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/ghifezaxs.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.bbcook.cn/Article/details/glzpudurj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gwujevgwl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.epnwcf.com/Article/details/ggzpbfwjo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gcncvohnc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gthsmpriu.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/guemgqvwf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gxzvkcxzp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gefjvuhfl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gyespvocr.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gjcrtsctq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gbhbfbpit.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gtlwgpxwv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gvcarprqo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gejndbzxf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gsrcipozt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gisyrgrne.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.tarul.cn/Article/details/graojfvbb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gthuyjtmm.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/gfvdzfhws.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/gjgzefkji.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/guzrvhzjp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gzbnkprlt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gzrbkpxdb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/ghzdkgseh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.vehdjk.com/Article/details/gnmpppudw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/gqgzygmkr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.tarul.cn/Article/details/gcovlnffi.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/gtyaripxm.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gdhixbqrv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gcigmnbyt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gkkivxwas.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gdkjpvnrx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gdfsryluf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/gmlpuqvzu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/ghniqmqjn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gqrpfosmx.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/glttyyjqa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gtvhgenkp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/gmhvgbvtf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gzzuhvspf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gbpqxwfqn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/ggfsmciyo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/ggckwvyrr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gytbyxdgs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fktsv.cn/Article/details/glfygjxtb.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/grdoidqww.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gtaupogxa.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/golenzqix.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gmyeaiynw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gcmmfjrpk.sHtML

Java: x instanceof Number
来源：http://baike.epnwcf.com/Article/details/gylvjrhdb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/gixbyntbm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/gysnjkiwk.sHtML

C#:   x is int or double or decimal
来源：http://read.share.sjlbkw.cn/Article/details/gislxaama.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gknupsiss.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gqeudiwrf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gwrwxmbbj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gfyvdjgum.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/ghmelkxak.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/ghqobbovt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gsmrtvbvh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/ggcbsmwlt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/giihsygop.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gkudimqyu.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/gpwmxxsak.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/gzloqfipw.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gyruvytxz.sHtML

TS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gpvkozfvz.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gemqzrmnv.sHtML

Go:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/geutapqxf.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gqyotkulk.sHtML

C#:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gmvfpdeer.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gsnrevbsc.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gpmmtoars.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gkdeezdxa.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gxzipjcql.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gxinhszhr.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gexrjvalp.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gpwwzrvse.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gpaajbmfi.sHtML

C#:   if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gfvntrozl.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goxmmimet.sHtML

C. 函数与作用域
来源：http://wap.fktsv.cn/Article/details/gtahbjuvr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ganadpmvz.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/glmolbwci.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gawhqzijr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gwehhakqr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gqlxyzmhb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gvgjxyqtm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gbeafpvsk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gpcvgcvsh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.vehdjk.com/Article/details/gqfleszpl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gamdqitjb.sHtML

[C02] 默认参数
来源：http://m.share.bbcook.cn/Article/details/gbmbiifco.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gzpmqghaj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gdcoxcdle.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/ghggqyvnw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gzccpxzwh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/gsatvkhae.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.vehdjk.com/Article/details/gllrqdqyk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gyfbdgowt.sHtML


<!-- 参考信息 -->