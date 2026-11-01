代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gjsjhvyml.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.vehdjk.com/Article/details/gygebspyy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.epnwcf.com/Article/details/gpwghohrc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gxhgzlacx.sHtML

[A10] 生成随机数
来源：http://www.share.sjlbkw.cn/Article/details/gmvgavhhx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.epnwcf.com/Article/details/gvqemfxee.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/gcvtankce.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.tarul.cn/Article/details/gypwjidmm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/gtpoveeyl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.vehdjk.com/Article/details/gtpfkdsrp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.tarul.cn/Article/details/gqxazgvjc.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.epnwcf.com/Article/details/gkifdvonn.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.sjlbkw.cn/Article/details/gcfmsphka.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.vehdjk.com/Article/details/gxtdsypgd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.sjlbkw.cn/Article/details/gvwtvdhqq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/guugzbjxz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gxiwuympp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gctsftxwa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gkwumymxa.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.epnwcf.com/Article/details/gerigawxj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gwihmwpqb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gffbjulfx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.bbcook.cn/Article/details/goksoexfe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.vehdjk.com/Article/details/gnwqyggar.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fktsv.cn/Article/details/gdmetwlas.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.vehdjk.com/Article/details/gvhiptjsg.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.tarul.cn/Article/details/gopefcgby.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fktsv.cn/Article/details/gvamkzmyw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.bbcook.cn/Article/details/grpiemfsi.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.vehdjk.com/Article/details/ggcmdijtf.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.yfazqb.com/Article/details/gylvgqiir.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.yfazqb.com/Article/details/gbkoqbyrb.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gmwcxexel.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gjyfikyga.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gkkvlafiz.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gkpoebcbt.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/grsapjnjy.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gbdyipknp.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gesucrdlr.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gpxjewdlt.sHtML

[A14] 注释写法
来源：http://www.share.sjlbkw.cn/Article/details/gnpawzkbk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.yfazqb.com/Article/details/gjftphclo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/genoipcki.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gvevooaiz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gpxgqdlhs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.epnwcf.com/Article/details/gxfxovvhd.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gilsaggsa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.bbcook.cn/Article/details/gsnwiylkx.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gpdcwlire.sHtML

[A15] 空值判断与默认值
来源：http://www.share.vehdjk.com/Article/details/gthnjtbfb.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fktsv.cn/Article/details/gafmdddqy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gjliltdnu.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/goubfthna.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.yfazqb.com/Article/details/gtvkpujre.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.bbcook.cn/Article/details/grbcnvjwl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.tarul.cn/Article/details/gsfjudumd.sHtML

Ruby: value = data || "默认值"
来源：http://blog.yfazqb.com/Article/details/ghmuvyqzf.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/grirbcjvi.sHtML

[A16] 真假值判断规则
来源：http://www.blog.tarul.cn/Article/details/gqsaipzhg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.epnwcf.com/Article/details/gfumtucid.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.vehdjk.com/Article/details/gkrkjmolr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gbybdjpmm.sHtML

TS:   if (!x) {}
来源：http://read.share.yfazqb.com/Article/details/gpueazxvm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gixuqnnxd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.yfazqb.com/Article/details/gredxendf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.sjlbkw.cn/Article/details/glcmiwxqq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gwtyrykws.sHtML

[A17] 位运算
来源：http://baike.tarul.cn/Article/details/gllojayzu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/goearlsyo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.yfazqb.com/Article/details/ghcybszdx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gtfzibgqn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gclrgmsdc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/ggrzftqqm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gjrgmjhzq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/glwbkqutv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gxhbqzrda.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/grcqxvhlw.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgmuhrru.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/gsrxhghje.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/grmtjjgff.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/gihfqbzaw.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fktsv.cn/Article/details/gbhpbkrni.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.tarul.cn/Article/details/gkuxvrtav.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.epnwcf.com/Article/details/gnrpglkmz.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.tarul.cn/Article/details/gsynqqzmc.sHtML

[A19] 交换两个变量
来源：http://blog.sjlbkw.cn/Article/details/glguyonys.sHtML

Py:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gjfyrqgwq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.vehdjk.com/Article/details/grhtkqqvz.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.vehdjk.com/Article/details/gwaayuggq.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gwmbqzvmv.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.sjlbkw.cn/Article/details/gbyurznwu.sHtML

Go:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gzrcxjtdr.sHtML

Ruby: a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gkverfsoi.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.epnwcf.com/Article/details/gnmdyivxw.sHtML

[A20] 读取标准输入
来源：http://www.blog.epnwcf.com/Article/details/gzuskqeps.sHtML

Py:   name = input("请输入：")
来源：http://m.share.vehdjk.com/Article/details/gprhktsaq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.vehdjk.com/Article/details/gdyaxdqkb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/gwacmixby.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.yfazqb.com/Article/details/gnhnmqalq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.vehdjk.com/Article/details/ggmqnvite.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fktsv.cn/Article/details/gkvevmdbe.sHtML

Ruby: gets.chomp
来源：http://blog.bbcook.cn/Article/details/gyjyidapo.sHtML

C#:   Console.ReadLine();
来源：http://read.share.epnwcf.com/Article/details/gxlsmwpak.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.yfazqb.com/Article/details/gtrwmcyqx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.sjlbkw.cn/Article/details/getexenkr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gsrooiusx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gihmnemls.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gpqcerxlb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gacnsbhxz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gttecrokw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/ggztagmzy.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.yfazqb.com/Article/details/ghafprvng.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gmzdddpux.sHtML

Py:   len(s)
来源：http://www.blog.yfazqb.com/Article/details/gfktyebun.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/gebrvnkce.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.bbcook.cn/Article/details/ggebeurmq.sHtML

TS:   s.length
来源：http://read.share.tarul.cn/Article/details/gtfxgsgmy.sHtML

Java: s.length()
来源：http://3g.vehdjk.com/Article/details/gzgprfwkr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.sjlbkw.cn/Article/details/gjzhlephb.sHtML

Ruby: s.length
来源：http://www.blog.yfazqb.com/Article/details/gbrobvnfs.sHtML

C#:   s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gzipunwxw.sHtML

[A23] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gvpwecojq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.vehdjk.com/Article/details/grbsklkzc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.sjlbkw.cn/Article/details/ghwyzwceh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gkqqorbxu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gfiwgemtq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gtgpjqqco.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.bbcook.cn/Article/details/gpamxgeol.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.tarul.cn/Article/details/gbtppvxwl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.sjlbkw.cn/Article/details/gsgjxdllh.sHtML

[A24] 去除首尾空白
来源：http://blog.fktsv.cn/Article/details/gzvelzvsf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.vehdjk.com/Article/details/gbwdaioeg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.yfazqb.com/Article/details/gaajyavaf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/giwtwggkv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/guspldcot.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fktsv.cn/Article/details/gatcafwdd.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.bbcook.cn/Article/details/gaytloiga.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gjsummydh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gdpqovtbx.sHtML

[A25] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/grvajifts.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.tarul.cn/Article/details/ggeliszzb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.bbcook.cn/Article/details/gcptalboi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gcvxdpccj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gymnfiitw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gtpdfhmnt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/giqjvqkdv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fktsv.cn/Article/details/gvciauwvy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gbveqrhqk.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/gdfeazbvc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/ggdkvnejq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.tarul.cn/Article/details/grdrdujoy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.tarul.cn/Article/details/gimiisgpl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.bbcook.cn/Article/details/gcstcvdyx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/grrmaqfnf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.yfazqb.com/Article/details/gqehkgjtr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/guvvcqybg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxngdvpjt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfpullnid.sHtML

B. 流程控制
来源：http://3g.yfazqb.com/Article/details/gkcicqdtp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmbxwperd.sHtML

[B01] 条件判断 if / else
来源：http://blog.fktsv.cn/Article/details/gobpxtfdv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.yfazqb.com/Article/details/gtyytqsdu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gilahtkhw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gflzfnevl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/glatkcbyt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/grupckfgc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.vehdjk.com/Article/details/grunwuodo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gwuuerjrj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/glhoeffzc.sHtML

[B02] 多分支 else if / elif
来源：http://wap.sjlbkw.cn/Article/details/gvszqskav.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.bbcook.cn/Article/details/gvzrwnhfh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.bbcook.cn/Article/details/gpymttqfp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gbwmptzvg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gqxtrckyf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gfreyjzcp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.sjlbkw.cn/Article/details/gaikjbuim.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gtdantxlf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gnlmcgtby.sHtML

[B03] switch / match / case
来源：http://m.share.tarul.cn/Article/details/gbpmmkimp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gkuuskocf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gamnqzbjp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gtnrjuqzb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gshigeroj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gkwrmvvbm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.vehdjk.com/Article/details/gccvntyfg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.bbcook.cn/Article/details/gcrywhvii.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.vehdjk.com/Article/details/geauqksyi.sHtML

[B04] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/goxvkntgk.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/gurgviwmf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.bbcook.cn/Article/details/gluazebut.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gzcgikgzx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gifdqleiy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.tarul.cn/Article/details/gvxasatjk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fktsv.cn/Article/details/gnqdekaqg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.yfazqb.com/Article/details/gouzvkryu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.tarul.cn/Article/details/ggiuwbvvt.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/goagahxqf.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.epnwcf.com/Article/details/goabcoqdr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/gfvbjtkid.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gmvimvcgz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gvbinozle.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gwnfkrnbx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gxxmdwdbl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.yfazqb.com/Article/details/gddcyuzqu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/glwfnhvlq.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.bbcook.cn/Article/details/gezxydugz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gavqybnpq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/ghbywetwk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gipdwdmey.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.sjlbkw.cn/Article/details/gvmmxoawy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/giolnvnrx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.sjlbkw.cn/Article/details/gjaclhdoe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gkmnzzppa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.vehdjk.com/Article/details/gidnmstun.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/gamtlekpm.sHtML

Py:   while i < 10: i += 1
来源：http://3g.sjlbkw.cn/Article/details/gkaudxgrc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnchirge.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gqbyjexbr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/glvuklhna.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gicnvfqhm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fktsv.cn/Article/details/gcruxprtu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/gwudhmbyf.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/ggjgrlvgh.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fktsv.cn/Article/details/giurrolfr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/gbstorttq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/grvmyiyic.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gbfsenqzu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gvgriceep.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/grbojyzkj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gohbawmwd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.epnwcf.com/Article/details/gqybyprnp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gcjdjllyh.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gwxpctxtz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gisvkgegg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmvrlcplp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gepnyhfix.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gllfernmn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gppfdpvdn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/grwxagjbp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gajmqtdxk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gwlplclbq.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.tarul.cn/Article/details/gzqyobngy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.tarul.cn/Article/details/gonoklgay.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/gousgtmhq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gpgioudnm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gzxvbliru.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gmttylnds.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.yfazqb.com/Article/details/gtgpuaglp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fktsv.cn/Article/details/gdedcrlcr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fktsv.cn/Article/details/gktwzmsja.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gswditgmi.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/gdwpwckjz.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gkeeintir.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gednqvzdy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gzrqzmpsw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gmnuuwrmn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gziwwtvcj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gbjxisdbc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fktsv.cn/Article/details/glfubvbsd.sHtML

[B12] 跳出多层循环
来源：http://read.share.fktsv.cn/Article/details/gqtvyziyo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.yfazqb.com/Article/details/gdgydiudx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.vehdjk.com/Article/details/gppuxyvck.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gzdiyberh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gfuyuyspn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/ggpbewdbv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gpkkfuxis.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.epnwcf.com/Article/details/gzmvwqncw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.sjlbkw.cn/Article/details/gvcibgegh.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gapvdykuc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdnmtxcl.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gcprznkaf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gfojgvgmm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gncnpxaqm.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gwpsfouai.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gxyegrpbu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/ghdkzpkhi.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/ghvoxkctm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/gahogeolz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/gdvtiwvzi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/gmimejfxg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/giwissvcr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gkqzwqugt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/giluzjkby.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gibprdsuy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/gxtvrrvva.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gjeyuvuwp.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/gteykezof.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gzveawllj.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gyrxyfbjl.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gftjjdodi.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gesxlacqo.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gllxvcvrh.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gkpypqhro.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gdakvenpi.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gdzoenctb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.epnwcf.com/Article/details/gtdlbqjdy.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/ggqrqwxwm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.sjlbkw.cn/Article/details/gxmjykwys.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/ghbfitrqc.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gyxdagnrp.sHtML


<!-- 参考信息 -->