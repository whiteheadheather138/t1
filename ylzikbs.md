代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gjgrzdgsa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.sjlbkw.cn/Article/details/gjwokoecc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/geqhdheuq.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.tarul.cn/Article/details/ggqhuutby.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/ghgpjkkye.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gkzksmgcz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gqfadkdvo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.tarul.cn/Article/details/gunuiyxpo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gbzsxicuz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.yfazqb.com/Article/details/gqabtdgso.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.tarul.cn/Article/details/gykwuoeci.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gfglsbojq.sHtML

[A10] 生成随机数
来源：http://blog.bbcook.cn/Article/details/gywdeyeew.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.yfazqb.com/Article/details/gtajgkzma.sHtML

PHP:  random_int(1, 100);
来源：http://blog.vehdjk.com/Article/details/gbpwvxspn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/glclonsqx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.vehdjk.com/Article/details/gdhxdtrkd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gfibqbwjl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fktsv.cn/Article/details/gwcssfukj.sHtML

Ruby: rand(1..100)
来源：http://3g.sjlbkw.cn/Article/details/ggkmfmcpb.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.tarul.cn/Article/details/gvyitjcdy.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.bbcook.cn/Article/details/gftrjxfto.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fktsv.cn/Article/details/gexlzfpgq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gxwxvbrwh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gorwlspht.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gwweyqklw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gjpspfxcv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/ggrxxxbwa.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gjbshdwzv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gajbwcdwc.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fktsv.cn/Article/details/gojwaxgfh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.epnwcf.com/Article/details/gycxqofgt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzhdrjmc.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.tarul.cn/Article/details/gxldecfzi.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.bbcook.cn/Article/details/gfbwtzguo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.tarul.cn/Article/details/gncpncpxj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.bbcook.cn/Article/details/grdzujaea.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.sjlbkw.cn/Article/details/gvroayyyb.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.tarul.cn/Article/details/gfboedicb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.epnwcf.com/Article/details/ghrrwyzmv.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gvvimgbse.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/grofruflz.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gjdvtbobn.sHtML

TS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gsmutdkht.sHtML

Java: "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gskjcquam.sHtML

Go:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gwwwuhaka.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gemxjlxck.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/giwzksgat.sHtML

[A14] 注释写法
来源：http://m.share.vehdjk.com/Article/details/gztkfnrhl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.bbcook.cn/Article/details/gxnqvjfyh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gvhietqir.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gwynhetrv.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/getisqcvs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.yfazqb.com/Article/details/gyyvcaitb.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/ggvrqrutu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.sjlbkw.cn/Article/details/gqjbcenhp.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gfnhcocng.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.bbcook.cn/Article/details/gtdemswuv.sHtML

Py:   value = data or "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gysznwkth.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gnypdbixn.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/golkuakde.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gprwverym.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fktsv.cn/Article/details/gwvgtgogh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.sjlbkw.cn/Article/details/gzmfrbwtr.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.epnwcf.com/Article/details/givsqxtzo.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gfplblard.sHtML

[A16] 真假值判断规则
来源：http://read.share.yfazqb.com/Article/details/guwrsovwf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.vehdjk.com/Article/details/gsbjcpyqa.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.bbcook.cn/Article/details/gpmvtnuab.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.tarul.cn/Article/details/gtkayopro.sHtML

TS:   if (!x) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbcxpison.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.bbcook.cn/Article/details/gwhflkkxv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.yfazqb.com/Article/details/gjgtwayqu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.vehdjk.com/Article/details/gxyduzgse.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.bbcook.cn/Article/details/gresamhtz.sHtML

[A17] 位运算
来源：http://blog.bbcook.cn/Article/details/gznewuzjl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gnoccqysu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fktsv.cn/Article/details/gyinzxube.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gopkeztvj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gdvgrkweo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/groheejvc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/glykpgste.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/glweuueax.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gtuxvdchq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.bbcook.cn/Article/details/gywljzlrj.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.epnwcf.com/Article/details/gkndptfyf.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gejcvucdk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.bbcook.cn/Article/details/gakwqbubh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gkklvkoqm.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.tarul.cn/Article/details/gqacjidyd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.bbcook.cn/Article/details/gvanekquv.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.bbcook.cn/Article/details/gtjotkdcv.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.sjlbkw.cn/Article/details/gfjqrreyk.sHtML

[A19] 交换两个变量
来源：http://wap.epnwcf.com/Article/details/gejxwzsxf.sHtML

Py:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gwuqmicmp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.tarul.cn/Article/details/gudbugxsp.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.tarul.cn/Article/details/gskkstwof.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gvbgbtcad.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fktsv.cn/Article/details/gocdcdebz.sHtML

Go:   a, b = b, a
来源：http://www.share.vehdjk.com/Article/details/ghsqjcdmb.sHtML

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gyfhmixud.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbdovdfg.sHtML

[A20] 读取标准输入
来源：http://www.share.sjlbkw.cn/Article/details/gdawcwnvy.sHtML

Py:   name = input("请输入：")
来源：http://3g.tarul.cn/Article/details/gwyqugwri.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.sjlbkw.cn/Article/details/guitnwssx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.tarul.cn/Article/details/gaxvpmqpb.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.vehdjk.com/Article/details/gehntrwts.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.yfazqb.com/Article/details/giytrmkcv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.yfazqb.com/Article/details/gddywbbvf.sHtML

Ruby: gets.chomp
来源：http://3g.vehdjk.com/Article/details/gclvbssvd.sHtML

C#:   Console.ReadLine();
来源：http://m.share.vehdjk.com/Article/details/gxdnfeiev.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.epnwcf.com/Article/details/gbzatqetv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.yfazqb.com/Article/details/gwtqxlgto.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gomzpboef.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gonutwban.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gjhnjdawk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwpcravx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gycwgmgzo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gmvnyxmgl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/glawksohd.sHtML

[A22] 获取字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/glzjnlrhw.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwtxfohjp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/gmooquyde.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.epnwcf.com/Article/details/gfrgpjjex.sHtML

TS:   s.length
来源：http://www.share.yfazqb.com/Article/details/gbobhxvrt.sHtML

Java: s.length()
来源：http://wap.vehdjk.com/Article/details/gvycwhxih.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gghgaguhm.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/glnlnoyos.sHtML

C#:   s.Length
来源：http://mobile.bbcook.cn/Article/details/gmovvuwlq.sHtML

[A23] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gbsfepbhn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gsgtnflwk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fktsv.cn/Article/details/gxnmruqge.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gwxlnbumu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/geyfrbglx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gntmonmsg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gfrehdgwg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.yfazqb.com/Article/details/gjdepilxl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fktsv.cn/Article/details/gmsqhoxbx.sHtML

[A24] 去除首尾空白
来源：http://www.blog.tarul.cn/Article/details/gtorvmzrl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.yfazqb.com/Article/details/gomnzifhh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gibmtvvrh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gghookcxk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.vehdjk.com/Article/details/gtbjubejr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.vehdjk.com/Article/details/giiwubuni.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.bbcook.cn/Article/details/gtrznfxga.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gevdzhlhr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.bbcook.cn/Article/details/gijtcupil.sHtML

[A25] 字符串比较
来源：http://m.share.tarul.cn/Article/details/guuqdbudp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/ghmgwyltz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.yfazqb.com/Article/details/gvouqingh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/gxvwsgjjt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gsjlftzqb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.bbcook.cn/Article/details/gvltufzmw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/gfcfhaqbv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.sjlbkw.cn/Article/details/gqlkinclc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/glucgpuds.sHtML

[A26] 类型转换总览
来源：http://baike.tarul.cn/Article/details/gjyskfliv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.sjlbkw.cn/Article/details/gtfceanpu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fktsv.cn/Article/details/getqehmhg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/goaskksag.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gmbdmixng.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gxhopbzkk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/gmfswbrfo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.yfazqb.com/Article/details/ghudrkqii.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gapbetauh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxhetumjn.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/glfsiglvu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzdiqhlgn.sHtML

[B01] 条件判断 if / else
来源：http://baike.sjlbkw.cn/Article/details/gznqmisxh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/glwzdfriw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/gyzrvyrto.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gcnapsitg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gopmvdyyp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gnbunnklf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/gwarwppvl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.vehdjk.com/Article/details/gcvnbnsyu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrgzkmlg.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.sjlbkw.cn/Article/details/gassgdwxs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/gjxamezjo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbwfrxlye.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/ggkubkpwk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gdvxsvqqn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gbmxmqynv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.sjlbkw.cn/Article/details/gijhjamov.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.yfazqb.com/Article/details/gnerncjdm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gwbqqapod.sHtML

[B03] switch / match / case
来源：http://baike.bbcook.cn/Article/details/gbemfoqme.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.yfazqb.com/Article/details/gppmqqfpr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gijmyonix.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gzyrsbzpx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gtakpnbxd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gpljxjbyt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gwbqowzog.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/grwpvkjcg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gnjkpheur.sHtML

[B04] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gxvernagc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.vehdjk.com/Article/details/gbbkmcdnf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/gwbmtreic.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gdzuxnajk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gkekqpsgp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fktsv.cn/Article/details/gibdqpwoj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.yfazqb.com/Article/details/gevuplcbf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.bbcook.cn/Article/details/gbonbzpag.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/gdocnttty.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/glgfoniiw.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/gqqbwyhcp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.vehdjk.com/Article/details/ghroewfwg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gmwugzoat.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gqjzxpndb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.tarul.cn/Article/details/gabgrrgft.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gtbzzylmx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.yfazqb.com/Article/details/gailznmak.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/gqouwapxq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.tarul.cn/Article/details/gxgqhuvzo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.vehdjk.com/Article/details/gyypukixd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.vehdjk.com/Article/details/gmdwtuajb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gwetyjiky.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gjxcgvjfm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gigjxnrmd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.bbcook.cn/Article/details/gxrzplize.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/guxxqqeqd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gsnextucr.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/grjpbmivi.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gwvfkrqoo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.tarul.cn/Article/details/gedyggvro.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gqvikvaxg.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gbmwqfspm.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gfubotqhm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.yfazqb.com/Article/details/gjegqyqkb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/gcfstxcza.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gsspbuicz.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/gsmaqpltt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/gbdgqdhug.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.yfazqb.com/Article/details/gwoiyiijl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/ggqrlwrkc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gbcuptlin.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gtoalmizg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.tarul.cn/Article/details/gyhpwslsw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gwiliubqi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gififizdo.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/gjufhzwjo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/gimxnybhq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gxepkzgkd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/ggrdqwqmg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/ggwbdojac.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/grzwdgkhs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.tarul.cn/Article/details/gnrtfdgwp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gudzsfkup.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gksgbytmj.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.sjlbkw.cn/Article/details/gkvhxtqar.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/ggenuhkzl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gsaxxssjl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gnexnokgl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gqzggwbjo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fktsv.cn/Article/details/gclwbnfvy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/gajherkor.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/gwuyiitoy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gaxwopati.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gntdvkiil.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fktsv.cn/Article/details/gsxcettgl.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/glpfdtmef.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gmfimickl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gxwfvuajm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.sjlbkw.cn/Article/details/ghbrxsaub.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.yfazqb.com/Article/details/gwfgjqgzz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gdhmkeyht.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gvwgoveja.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/gwsnfwtpd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gbryjnrdr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/ggfhfikqn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gqdejxinp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gskqkwhnq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gdjxlcvlw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/gvjbfdzub.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.yfazqb.com/Article/details/gugbwcrbt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gogegnnnh.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/gecsfllgq.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.tarul.cn/Article/details/gpeaamrrv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.epnwcf.com/Article/details/gxcpraeis.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gnmcuroph.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gpqdmovbe.sHtML

Java: x instanceof Number
来源：http://www.m.share.tarul.cn/Article/details/gmyajierw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gkkpheulw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.epnwcf.com/Article/details/gcajtsxsu.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gzlkmelmk.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/gfnejtzkl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fktsv.cn/Article/details/gzpkmvxti.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/gnjizajac.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gdwhipcbz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gjkrugxon.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.tarul.cn/Article/details/gwakbantl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gjsgiujuj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/gqppgdfhn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/ghpapvues.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.vehdjk.com/Article/details/grkebkgxj.sHtML

Py:   a and b or not c
来源：http://wap.yfazqb.com/Article/details/gggxlxtde.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gqxhdujdx.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gyqiqfxyi.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gmooonewj.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/ggpeodgzo.sHtML


<!-- 参考信息 -->