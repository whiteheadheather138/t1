代发 wailian999

[A10] 生成随机数
来源：http://www.share.yfazqb.com/Article/details/gbquqnwhx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.tarul.cn/Article/details/ghiqhbgfe.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fktsv.cn/Article/details/gvihtvrlx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.sjlbkw.cn/Article/details/gqyyzwlxb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.tarul.cn/Article/details/gvowvixra.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.vehdjk.com/Article/details/gmfikstin.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.bbcook.cn/Article/details/gdinvpfvv.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.tarul.cn/Article/details/gtlwpbewo.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fktsv.cn/Article/details/gqbxrjuha.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.vehdjk.com/Article/details/gxaqocxja.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.tarul.cn/Article/details/gtfxkrkcv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/ghvenesog.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/giusqlwsq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gbdnhtwtj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gcfkxdiip.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.bbcook.cn/Article/details/gowkigcgb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gdijhgebh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/geowxjryg.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.sjlbkw.cn/Article/details/griepyowr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.yfazqb.com/Article/details/gvxfixxmf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.bbcook.cn/Article/details/gsshlnpqn.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.sjlbkw.cn/Article/details/gietkdzgy.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/ggdqmtikp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fktsv.cn/Article/details/gmormrigw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fktsv.cn/Article/details/gcgrmqthc.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.bbcook.cn/Article/details/gbegzazbs.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.yfazqb.com/Article/details/gxkfzpgou.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/gmgsgukoj.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gfeteclco.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gcdyyonir.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gvgopbidu.sHtML

TS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gwkmzmwbc.sHtML

Java: "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gsyxgmfyp.sHtML

Go:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gdlcvxqba.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gqjdlzlyc.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/grtuhchww.sHtML

[A14] 注释写法
来源：http://read.share.tarul.cn/Article/details/gojjgtwcv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.yfazqb.com/Article/details/gqeafdpyc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gvbmtypko.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gxfwilicv.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gedfkwzed.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.bbcook.cn/Article/details/gtqydwryz.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/geakxfocw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/gozwaonfb.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gbflcvdtg.sHtML

[A15] 空值判断与默认值
来源：http://m.share.tarul.cn/Article/details/gnypnybha.sHtML

Py:   value = data or "默认值"
来源：http://wap.vehdjk.com/Article/details/gatjwksxa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gcwceeogv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gtazcmpjx.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gektsntua.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.bbcook.cn/Article/details/gtzngachz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.vehdjk.com/Article/details/ggfnntvud.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.tarul.cn/Article/details/gombhjhht.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gblhpfzmp.sHtML

[A16] 真假值判断规则
来源：http://mobile.epnwcf.com/Article/details/gvgqkjtfx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.epnwcf.com/Article/details/gysexnncv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.vehdjk.com/Article/details/gvufaqucj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fktsv.cn/Article/details/gihgnwams.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/gmhfavgmp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.bbcook.cn/Article/details/ghubcymba.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.vehdjk.com/Article/details/gfnkpbvzj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fktsv.cn/Article/details/ghodgjfen.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.tarul.cn/Article/details/gtqhbqoan.sHtML

[A17] 位运算
来源：http://read.share.sjlbkw.cn/Article/details/gllqjlimf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gnnmfvyqe.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/gzkglqmpt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gnkyrqpxe.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gjxfsquvd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gtupztkqb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gdkfnrlcu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/glqfldszy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gabmllypx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fktsv.cn/Article/details/gcpvtqxvk.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.bbcook.cn/Article/details/gimcbwozh.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.vehdjk.com/Article/details/glssrmkva.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.vehdjk.com/Article/details/gzmifgzaz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.tarul.cn/Article/details/gtiorjcgd.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.yfazqb.com/Article/details/geznasquc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fktsv.cn/Article/details/gsojbxjdz.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.vehdjk.com/Article/details/gpcyjafpo.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fktsv.cn/Article/details/gphppltoy.sHtML

[A19] 交换两个变量
来源：http://3g.sjlbkw.cn/Article/details/guakktolm.sHtML

Py:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gzfkzmzcj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.tarul.cn/Article/details/gqgutqswm.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/gemomckvc.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.vehdjk.com/Article/details/gphzkkieg.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdpnjgby.sHtML

Go:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gyphctory.sHtML

Ruby: a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gohwxoiug.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.vehdjk.com/Article/details/gbtybaoms.sHtML

[A20] 读取标准输入
来源：http://mobile.sjlbkw.cn/Article/details/gzwqwdevb.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.tarul.cn/Article/details/gkvzwzhhn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fktsv.cn/Article/details/gwwsrrbug.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.epnwcf.com/Article/details/ghpvmzrqd.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/gjvakiyxj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.epnwcf.com/Article/details/glabjjoqw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.epnwcf.com/Article/details/gomaslpuz.sHtML

Ruby: gets.chomp
来源：http://www.share.sjlbkw.cn/Article/details/gwiqdduvj.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fktsv.cn/Article/details/ggmpnxszv.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.tarul.cn/Article/details/gpdjzwhnn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.epnwcf.com/Article/details/ghgogjyqg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gghyxfyfw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/glvmsehrm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gjgadtptp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/golczsonn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gcloehqdw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/gboqxwgwg.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.epnwcf.com/Article/details/givzcofdc.sHtML

[A22] 获取字符串长度
来源：http://m.share.vehdjk.com/Article/details/gifzefvar.sHtML

Py:   len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gvrvkdrie.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.tarul.cn/Article/details/gtufxjivo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.sjlbkw.cn/Article/details/gexgeskxs.sHtML

TS:   s.length
来源：http://m.share.epnwcf.com/Article/details/gedmjuwyi.sHtML

Java: s.length()
来源：http://3g.epnwcf.com/Article/details/gotetkbvr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.vehdjk.com/Article/details/gewhngfie.sHtML

Ruby: s.length
来源：http://mobile.sjlbkw.cn/Article/details/gqrrxdzxv.sHtML

C#:   s.Length
来源：http://mobile.bbcook.cn/Article/details/gsexyaxju.sHtML

[A23] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gwntbvrpv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.epnwcf.com/Article/details/gprhpgnkp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.tarul.cn/Article/details/gauwgidsl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gihayarst.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gbmkaphcu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gelluyzxf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.vehdjk.com/Article/details/gutnfamxi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gtempnwgj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.yfazqb.com/Article/details/gqmjrwpoh.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/gadvmnrhq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.epnwcf.com/Article/details/gojbjtkpd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gfomkeqhr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gnrfzhury.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.yfazqb.com/Article/details/gvfcujowo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/gzcuwbtmu.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.yfazqb.com/Article/details/gauvqyliv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.tarul.cn/Article/details/govecwwnp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.vehdjk.com/Article/details/gpljnxlem.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gpavrbbou.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.bbcook.cn/Article/details/gsfhpwaff.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.tarul.cn/Article/details/gsmyemphv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gzrnyywhd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gqoxllqes.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.vehdjk.com/Article/details/gjtnxsecq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/grekxnzef.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.sjlbkw.cn/Article/details/gcludvtwy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gebayuyeg.sHtML

[A26] 类型转换总览
来源：http://www.share.sjlbkw.cn/Article/details/gptikbsgb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.bbcook.cn/Article/details/gxcfsymbo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.vehdjk.com/Article/details/gmhbbxgai.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/gvipcaaqv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.tarul.cn/Article/details/gtodnhife.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gfwhzohub.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.yfazqb.com/Article/details/gvjhemqwl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/gthsgweyh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gfzxvihce.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkktideti.sHtML

B. 流程控制
来源：http://www.share.tarul.cn/Article/details/ggpoyitxr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gcwcknrla.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/godrhjmis.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.yfazqb.com/Article/details/gtejqnghn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gzfhppnzp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gymeyuwsz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gbremzeux.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gxexdzqfo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.epnwcf.com/Article/details/grpijyfhy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.epnwcf.com/Article/details/gyryiveyw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gxifbdnqr.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.yfazqb.com/Article/details/gcjxxoeon.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.epnwcf.com/Article/details/guehawtec.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gojcehvbi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gtlsrtzvh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gyxkxlevc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gdrbkkyom.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhkpkmjj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fktsv.cn/Article/details/grzddgokn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/grghxmmfz.sHtML

[B03] switch / match / case
来源：http://baike.sjlbkw.cn/Article/details/gapqpowyk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fktsv.cn/Article/details/gondspuwa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gasfrvvnf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/glamhbpri.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gytsgkdbh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhrmkcga.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gobusetyy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/gzljfgldv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gmtpiwsxj.sHtML

[B04] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gawpurdlc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/givytlvaq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/gvtjnbhis.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/ggnfuarjd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/ggaylhwda.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/gzfufmuvp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.yfazqb.com/Article/details/gdjrhmflc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gxyxnktce.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gwtszzkbz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/glevtdpoy.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/gnymdiwba.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.bbcook.cn/Article/details/gnhojstql.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gxbghduxr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gygcgwkty.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gppvhkbsh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.sjlbkw.cn/Article/details/guanyztcp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gtsdjepsa.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/gbllswris.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.tarul.cn/Article/details/gqwzqfjgl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/gvshxbaan.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gborsazzj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gdjgtpurh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/glxvqewmm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.epnwcf.com/Article/details/grberhuzn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gaicdpkck.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.vehdjk.com/Article/details/gxideaaay.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gwnprrdpi.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gaayweape.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gwvcgjfwo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gbluveylg.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/ggjpntudo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gmzlktavl.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gipmfusjx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.epnwcf.com/Article/details/ggwhosfmh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/gyipywbnv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gnxphoqyl.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gryppfgho.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/giwnvksdv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.yfazqb.com/Article/details/grmqqkwdt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gxhfqerzs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gtflupnyu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlqdjkfr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fktsv.cn/Article/details/gpzfbrkrv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.vehdjk.com/Article/details/gwyuqyhgd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gbdjoahij.sHtML

[B09] break 与 continue
来源：http://www.share.tarul.cn/Article/details/giytfbdfc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/geugadhei.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gcekzcosi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/ghvznyxqh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gcyuyhegc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gnhwikpow.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/garkwnoth.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gkgxldzoi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gpdvclfip.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fktsv.cn/Article/details/gsqqnjblu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gcfxicvch.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.vehdjk.com/Article/details/gclbkjfjq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gvjcirmdy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gewrvljhz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.yfazqb.com/Article/details/guizwbfqg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.bbcook.cn/Article/details/gebtqubse.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.sjlbkw.cn/Article/details/ggjvnizod.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gbxeixuxd.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/gijjvzbmf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/gyzzhzklq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gjlmngruz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdtenjxg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gsjnekmzb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.bbcook.cn/Article/details/galrnwcrn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/guhkqsxvy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.epnwcf.com/Article/details/gupgsyrjx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/gmebpikvz.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gnwxzfseb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gnlhhfmui.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gbyvxhdnf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvfqoozw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gsxgynfvk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gpwshvzkx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gejtunsqs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.vehdjk.com/Article/details/gwniubfbg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/gviuklkvl.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gcntzohqw.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.yfazqb.com/Article/details/gggighicq.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gnudmfyds.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gwggwxmyb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gyqghvmoe.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/gyplivlzv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/grdepqsrv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fktsv.cn/Article/details/glxzoqwkz.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/ggvvtmglb.sHtML

[B14] 判断值是否在集合内
来源：http://wap.epnwcf.com/Article/details/gxduvsgjy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.epnwcf.com/Article/details/gvpcqzhrw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gbzcpipik.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gwomszagw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/gbjqbzcjg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gxlpdnhgi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gnubjtvaw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/gstzixekg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/grxwamjuu.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/gwqnzfxxo.sHtML

Py:   a and b or not c
来源：http://m.share.yfazqb.com/Article/details/gfudyeaef.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.vehdjk.com/Article/details/goqeowsqn.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gynqnvwxf.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gtsdvkbhw.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gniivdanv.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gibtzoknn.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gnipcvflq.sHtML

C#:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gutbdzlzp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/gifctumww.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gjsqihwro.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdnzsxgdb.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gbccfpntx.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gbuyufgvy.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gmxransgp.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gxuwemwkn.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gqdqxqjon.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/ghrsqbaqz.sHtML


<!-- 参考信息 -->