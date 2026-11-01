代发 wailian999

[A10] 生成随机数
来源：http://baike.bbcook.cn/Article/details/geejdrpdm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.vehdjk.com/Article/details/gsjzldzns.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fktsv.cn/Article/details/ghzdkqvqp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gbkabxvrh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.yfazqb.com/Article/details/gasaddnks.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.bbcook.cn/Article/details/gzvgczmhy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.sjlbkw.cn/Article/details/gujyjcfbx.sHtML

Ruby: rand(1..100)
来源：http://mobile.sjlbkw.cn/Article/details/gtmlrhsgw.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.epnwcf.com/Article/details/gqszgrzgs.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.bbcook.cn/Article/details/gkzvqvkkt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fktsv.cn/Article/details/gqccxgbev.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gozbamfye.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkniljssr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/grqiuvftg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/getzvbqxd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.vehdjk.com/Article/details/gadaoawmy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gmkccxztr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyggjdyf.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fktsv.cn/Article/details/gemhshffw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.epnwcf.com/Article/details/glkhunmqn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.epnwcf.com/Article/details/gjxtqjbpl.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gmdndjqza.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/goctcszgi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.yfazqb.com/Article/details/ggpauombz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.epnwcf.com/Article/details/getworeim.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.bbcook.cn/Article/details/gcsvavpcv.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.tarul.cn/Article/details/gwyqrsggv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.sjlbkw.cn/Article/details/gsdexkncj.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gwmcuofna.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/ggrdamhkr.sHtML

JS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gqrwfqofb.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gbtmcdktg.sHtML

Java: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gtgvcsvfg.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/goplzombr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gxratntks.sHtML

C#:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/goapjvedk.sHtML

[A14] 注释写法
来源：http://www.m.share.yfazqb.com/Article/details/gtnzfdave.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.bbcook.cn/Article/details/gadretqvy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gioancnnr.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gnzharimy.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gfjksvgwd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.sjlbkw.cn/Article/details/gtaxpxeqd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gwvrgfabw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.tarul.cn/Article/details/gvirwuswe.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gycwqpiud.sHtML

[A15] 空值判断与默认值
来源：http://www.share.tarul.cn/Article/details/gujrmkkjv.sHtML

Py:   value = data or "默认值"
来源：http://mobile.bbcook.cn/Article/details/gfpxgpjgj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gbfxbhwfg.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gigcdzznp.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gkdticrbo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.vehdjk.com/Article/details/gnmgttsbn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.bbcook.cn/Article/details/ginxbhylg.sHtML

Ruby: value = data || "默认值"
来源：http://3g.vehdjk.com/Article/details/gsvbusryy.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gvscgaapg.sHtML

[A16] 真假值判断规则
来源：http://mobile.epnwcf.com/Article/details/gqwxjsvkb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.bbcook.cn/Article/details/gdgamxpov.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.tarul.cn/Article/details/gurdxuntu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gieikkeoz.sHtML

TS:   if (!x) {}
来源：http://blog.epnwcf.com/Article/details/gkredxpbu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.yfazqb.com/Article/details/gzgnplqzy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fktsv.cn/Article/details/grspmycao.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgcklccv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvasgtawb.sHtML

[A17] 位运算
来源：http://www.blog.yfazqb.com/Article/details/gdsqtlfjd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gbaqtzusw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.yfazqb.com/Article/details/glkdjxamy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/geghbvmuf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gegubykkx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/ghgefjecj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/giiagsilz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gkmcgcczz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuabhxlz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.bbcook.cn/Article/details/gmhumiywh.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gaxkxmwgu.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/gqrqsncee.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fktsv.cn/Article/details/gsematutk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gmoqwqlqx.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fktsv.cn/Article/details/glrucsuby.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.yfazqb.com/Article/details/gguggoely.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.yfazqb.com/Article/details/gzfpgpnqv.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.tarul.cn/Article/details/gmugnwgsi.sHtML

[A19] 交换两个变量
来源：http://www.blog.sjlbkw.cn/Article/details/geprrrmuy.sHtML

Py:   a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gsodrenun.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.tarul.cn/Article/details/ggfovvuvy.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fktsv.cn/Article/details/gviqxqtcs.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.epnwcf.com/Article/details/gnmpctoog.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.bbcook.cn/Article/details/gdhuqsobc.sHtML

Go:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gkgzazopp.sHtML

Ruby: a, b = b, a
来源：http://m.share.fktsv.cn/Article/details/gomqzvucn.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.yfazqb.com/Article/details/glxedwyel.sHtML

[A20] 读取标准输入
来源：http://wap.vehdjk.com/Article/details/gahontywu.sHtML

Py:   name = input("请输入：")
来源：http://www.share.sjlbkw.cn/Article/details/gnpeklnlw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.epnwcf.com/Article/details/gnkfobrrp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.sjlbkw.cn/Article/details/gdjbnsjve.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gysrtannx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.tarul.cn/Article/details/gzqqabkmt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.vehdjk.com/Article/details/gthujrujv.sHtML

Ruby: gets.chomp
来源：http://www.blog.sjlbkw.cn/Article/details/gaaggzudc.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.tarul.cn/Article/details/glehkofog.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fktsv.cn/Article/details/gelwzusfu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.bbcook.cn/Article/details/gpqeyjlxh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gaoqhbois.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/grgieukix.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gvwozobiu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gmwgaxktv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gskltpxsx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gjwboueul.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.yfazqb.com/Article/details/gesykhbdr.sHtML

[A22] 获取字符串长度
来源：http://www.share.yfazqb.com/Article/details/gjueljxwd.sHtML

Py:   len(s)
来源：http://wap.bbcook.cn/Article/details/gjzjtbamv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.vehdjk.com/Article/details/gvpinixcw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.sjlbkw.cn/Article/details/grgvpoyyi.sHtML

TS:   s.length
来源：http://wap.bbcook.cn/Article/details/gbgnwwitg.sHtML

Java: s.length()
来源：http://read.share.bbcook.cn/Article/details/glrvsrvri.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gnslpghur.sHtML

Ruby: s.length
来源：http://baike.sjlbkw.cn/Article/details/gxxphcmms.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/geuaracmy.sHtML

[A23] 大小写转换
来源：http://3g.tarul.cn/Article/details/gwvjfzbpj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.sjlbkw.cn/Article/details/gqxqzulal.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fktsv.cn/Article/details/grullctuo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gncwgubbf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/glauzapds.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.bbcook.cn/Article/details/goyqbrcdm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.yfazqb.com/Article/details/gxwfiatea.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gekwgprai.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.tarul.cn/Article/details/gxhmjfbua.sHtML

[A24] 去除首尾空白
来源：http://blog.vehdjk.com/Article/details/gzfszwqmw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.epnwcf.com/Article/details/gccwrpjeb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.yfazqb.com/Article/details/gjtmqztmf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gjmcfplgs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gbnrkbwtf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.yfazqb.com/Article/details/gacqktcnv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/gasfhrxdu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.tarul.cn/Article/details/gaocjsbbl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gdkytvofk.sHtML

[A25] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzdrwkny.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.epnwcf.com/Article/details/gmmupjava.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/gjjireiqz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gothpvbwr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gfrflrjfm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fktsv.cn/Article/details/gwnkfjpct.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gijqyuwpj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/gfypwedbh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/gjbmjyxcd.sHtML

[A26] 类型转换总览
来源：http://baike.fktsv.cn/Article/details/gzjeaqfiq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.tarul.cn/Article/details/gbgjyhnxa.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/gfddeoftc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.sjlbkw.cn/Article/details/gklnjfuip.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.yfazqb.com/Article/details/godpuljgc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/guytqjlbs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.yfazqb.com/Article/details/gbxcchuht.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/glilsvlip.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gmcnpsiqh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghoksnagn.sHtML

B. 流程控制
来源：http://mobile.epnwcf.com/Article/details/gehpdlxka.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbmvvkypr.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gchlnjygd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.epnwcf.com/Article/details/gwivgjlll.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/glrzuicsu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gdkrauarq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/ginygrzgm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gtmlpyaok.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.epnwcf.com/Article/details/guzgykfhj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.vehdjk.com/Article/details/gohiumojq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/grddaapio.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.bbcook.cn/Article/details/gwrexoapw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.bbcook.cn/Article/details/gvflzgkzb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fktsv.cn/Article/details/gndfjeilj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gcnmrimnf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gqdulbmdp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gqxthiaot.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.tarul.cn/Article/details/gjstbiqov.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gnnwhnvjv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gipkjmrym.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gcqxczacr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.tarul.cn/Article/details/guargzken.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gccmseicj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gpimkkeoo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/geavpkxev.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/godjpxkuw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/grjwyarpk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.sjlbkw.cn/Article/details/gziunrzmw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/guvmtajnk.sHtML

[B04] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gkxaocqzu.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/gskwriyee.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.vehdjk.com/Article/details/gmkjucwni.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gxoqfgljg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gqojsmypi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/ghwbcgpas.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.sjlbkw.cn/Article/details/gpubcbdis.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.bbcook.cn/Article/details/gyeogwwxi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fktsv.cn/Article/details/gfgqmwiaw.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gsytqnehz.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fktsv.cn/Article/details/gucxnzldi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fktsv.cn/Article/details/gbgycuxmz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/ghvprpdzp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/ghwwhfqfr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.yfazqb.com/Article/details/gjdjtqsbv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.yfazqb.com/Article/details/gtlhzwckb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/grtnrvjkv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/gdjgagves.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.tarul.cn/Article/details/gilpdrmrd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gnusjkcse.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fktsv.cn/Article/details/gfnittlwo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gikrkttbz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/gbpeeozjq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gqciabavl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gswmyvfkl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.bbcook.cn/Article/details/gxvireqar.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/grcdhxtkn.sHtML

[B07] while 循环
来源：http://blog.vehdjk.com/Article/details/gsfhfqngy.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.epnwcf.com/Article/details/gcockynqz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gdkivnimf.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/grquarpms.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gftumjwri.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/giaiqjjtm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gvqmaxdhv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/gvesbjgug.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gjkehogps.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.bbcook.cn/Article/details/gynnrloab.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/gbcndhjnx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/gmarlnwkj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/ggoqwieui.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gthdtccpw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gbqlxdntt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/gubshdhel.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/grgidlgjk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gfymdixwd.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gyshhtoam.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gekkatmkj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/ggfrmilvl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/glytpkiql.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gpscscmtf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gkhydarkc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gbusudxob.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gxfkjckbx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gotciecue.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/gwtjdkplg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gryeypyds.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gwgulrhnm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/glfpyucwx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gbmbglfuv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/ggfyjxvye.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/girxicucs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.vehdjk.com/Article/details/girgckmxo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.bbcook.cn/Article/details/gjkwuttbk.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/grzbbclnt.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.yfazqb.com/Article/details/gcarezjph.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/gktphpmrw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gybbxfoxi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gjhotnhhh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gllofeaty.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/ghemneplq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/ganowrdmm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.tarul.cn/Article/details/gzmkpfovk.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/guvcdssue.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.bbcook.cn/Article/details/ggqljgwzs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gqhwquwsd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gohwgeoym.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gzeidubsf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gtwkksfqz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gdundsylw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpddflqe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gmvqbesez.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gcrwgwyxx.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.sjlbkw.cn/Article/details/gpqlpziga.sHtML

PHP:  is_numeric($x)
来源：http://www.share.sjlbkw.cn/Article/details/gpqlgbcvc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gdyrjjwnt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwhgrnliy.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gkezdbgtw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.vehdjk.com/Article/details/gwerqbavg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gegiefalh.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gzhqkgijo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gvmaqggmd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gdlxmbeel.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gplstogec.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gdvgohmlx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gpjgtiyaa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gexjwbdvh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/gclkjslqj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gstmssmim.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fktsv.cn/Article/details/gqehbunee.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/ggknrpinp.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gycabswpv.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gfksrivrc.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gsljswlhc.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gbbqacbak.sHtML

Java: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gfbfwegpz.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gjscrjuyi.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gfdsrpohd.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gtudqpjnx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/gttrehmni.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/govriiybb.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gqjgxrwnf.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gcvvplalb.sHtML

TS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gvfndnqmg.sHtML

Java: if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/glwxrsdti.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gqamhjuxm.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/giencpxlc.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gjnsbyuyh.sHtML


<!-- 参考信息 -->