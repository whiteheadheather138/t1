代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.sjlbkw.cn/Article/details/gyjfxupxy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gihjhavna.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fktsv.cn/Article/details/gqvpvhtlp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gteukxgfj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/gxuenfrqn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.epnwcf.com/Article/details/guqngenmp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gpfuacnyh.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.bbcook.cn/Article/details/gmbmlfomp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.vehdjk.com/Article/details/gybgielfy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gmtipliue.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gookoaqqe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzdvuvzf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/guvtpzfzk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.vehdjk.com/Article/details/guzbmckws.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.yfazqb.com/Article/details/glhwwhkzf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.tarul.cn/Article/details/gkpmolfjh.sHtML

[A10] 生成随机数
来源：http://wap.epnwcf.com/Article/details/gaznufzdi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.sjlbkw.cn/Article/details/gsdjqvldw.sHtML

PHP:  random_int(1, 100);
来源：http://baike.sjlbkw.cn/Article/details/gjjzwnuhh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gvrpolqne.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.vehdjk.com/Article/details/gobufwwon.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gmipreqpd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.yfazqb.com/Article/details/gfxvjdajl.sHtML

Ruby: rand(1..100)
来源：http://baike.fktsv.cn/Article/details/gzzrtdtjc.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.epnwcf.com/Article/details/gdbeubrmt.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fktsv.cn/Article/details/gzfatnaxo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fktsv.cn/Article/details/gghzguyca.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gufvmpxje.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gstsfamzr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gainercdd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gyxfpzjby.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.bbcook.cn/Article/details/gkrcltvtp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gcjnfyeiq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gbigviesc.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.vehdjk.com/Article/details/gabsxipzg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.tarul.cn/Article/details/gdfrdgrtt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.tarul.cn/Article/details/gqlinlxrm.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.vehdjk.com/Article/details/gdoxrirfk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/grdhmqqum.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.epnwcf.com/Article/details/gcugtpyft.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fktsv.cn/Article/details/gdumvehwv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.vehdjk.com/Article/details/gzqzxvhzv.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.bbcook.cn/Article/details/gmysmcnaz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.sjlbkw.cn/Article/details/gacubilgh.sHtML

Py:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gwcdahptv.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/glbbuxoji.sHtML

JS:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gxwligkkq.sHtML

TS:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gvnhrkmlx.sHtML

Java: "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/guxlzwldf.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gvtxkuvcz.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/grmjnedyb.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gagibeccw.sHtML

[A14] 注释写法
来源：http://mobile.fktsv.cn/Article/details/glbkvwifk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.bbcook.cn/Article/details/gxclesqrp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gkirosumb.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhuydldm.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/glroxahrn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.tarul.cn/Article/details/gyunpzbpg.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gwweabrmp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.sjlbkw.cn/Article/details/giwtlfrwz.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/givjazdsc.sHtML

[A15] 空值判断与默认值
来源：http://m.share.bbcook.cn/Article/details/gsblzlaxq.sHtML

Py:   value = data or "默认值"
来源：http://mobile.tarul.cn/Article/details/geslahpqx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gfadmnsld.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/grloknvli.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/gdcadwyxo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.yfazqb.com/Article/details/geqrhdpgj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.yfazqb.com/Article/details/gkmnveaib.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.bbcook.cn/Article/details/ggyfktiuf.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/gqammhtsw.sHtML

[A16] 真假值判断规则
来源：http://m.share.epnwcf.com/Article/details/gentfpehk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.tarul.cn/Article/details/ghotgntbr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.vehdjk.com/Article/details/gvlhcsswo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.tarul.cn/Article/details/gffsnisrd.sHtML

TS:   if (!x) {}
来源：http://www.m.share.tarul.cn/Article/details/gzweviavt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/gnyypksqc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.tarul.cn/Article/details/gytmnahfc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.vehdjk.com/Article/details/gxyfpiwhn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtstjyzpm.sHtML

[A17] 位运算
来源：http://3g.sjlbkw.cn/Article/details/genyawskg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/geyetryjg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.tarul.cn/Article/details/gxfpbpatt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gzjapftog.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gxqehojwk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gpipoduza.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gpupgblhn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/graqrxumh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gqiuserka.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.vehdjk.com/Article/details/ggguhlext.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/gxguyswjy.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/ghgkbknww.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gnhtqgtod.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.epnwcf.com/Article/details/ggiznfsij.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.tarul.cn/Article/details/gqragbffk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fktsv.cn/Article/details/gneolqddp.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.bbcook.cn/Article/details/grdsygafh.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.bbcook.cn/Article/details/gdvslhfbv.sHtML

[A19] 交换两个变量
来源：http://blog.fktsv.cn/Article/details/glwyeqbxw.sHtML

Py:   a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/gorftdfbf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fktsv.cn/Article/details/glpbkrdxp.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/gxlnmwrgw.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.yfazqb.com/Article/details/giadnxzfp.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.sjlbkw.cn/Article/details/gcopmoksz.sHtML

Go:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gtrowzzou.sHtML

Ruby: a, b = b, a
来源：http://blog.sjlbkw.cn/Article/details/gxbikqsgd.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.yfazqb.com/Article/details/gthzplxpz.sHtML

[A20] 读取标准输入
来源：http://3g.sjlbkw.cn/Article/details/gpmbxsczf.sHtML

Py:   name = input("请输入：")
来源：http://www.share.sjlbkw.cn/Article/details/gtkfvrpfg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.yfazqb.com/Article/details/gwhkwdrkk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.bbcook.cn/Article/details/gffmnscvw.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.yfazqb.com/Article/details/gdmzlxrqo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.epnwcf.com/Article/details/gtcdrlzsl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gtyyejrae.sHtML

Ruby: gets.chomp
来源：http://www.share.epnwcf.com/Article/details/gbnmonobk.sHtML

C#:   Console.ReadLine();
来源：http://baike.bbcook.cn/Article/details/gmmmirmtf.sHtML

[A21] 保留指定小数位输出
来源：http://3g.sjlbkw.cn/Article/details/gpxfamsox.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.epnwcf.com/Article/details/gfufcuunt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gqgfjvvon.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gzpusgjqa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/guwqmxjsm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gephhjwph.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gapaoqajq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/ghjzjbiis.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.epnwcf.com/Article/details/gyonqvuta.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gwlhcfetz.sHtML

Py:   len(s)
来源：http://wap.vehdjk.com/Article/details/gllvnnyuc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.tarul.cn/Article/details/gwiailjxq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.yfazqb.com/Article/details/gbboxmgex.sHtML

TS:   s.length
来源：http://www.blog.epnwcf.com/Article/details/gemupvlgm.sHtML

Java: s.length()
来源：http://www.share.yfazqb.com/Article/details/gkzhrglwt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.yfazqb.com/Article/details/godejelos.sHtML

Ruby: s.length
来源：http://wap.fktsv.cn/Article/details/gscsyeslg.sHtML

C#:   s.Length
来源：http://mobile.bbcook.cn/Article/details/gjczgkzhb.sHtML

[A23] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gzhemqtay.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.bbcook.cn/Article/details/gxtiaeukg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gqnxjbalo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gnqyxtoxp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/ghueujgkp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fktsv.cn/Article/details/gdmuvzcpx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpxiqflvr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.epnwcf.com/Article/details/gcffvekfd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.sjlbkw.cn/Article/details/gleunxpbt.sHtML

[A24] 去除首尾空白
来源：http://mobile.bbcook.cn/Article/details/gujaucovf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.yfazqb.com/Article/details/gudirsdrj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.tarul.cn/Article/details/grgzcnshb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gpkgwlnvj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gpyrxxywg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fktsv.cn/Article/details/grzkbbbda.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.epnwcf.com/Article/details/gmsdjycjn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/gvkbbjyat.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gzvsjmwvg.sHtML

[A25] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/girlyyhor.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.tarul.cn/Article/details/gkpflhaxn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gbchyyfcr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gylxwmzom.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/gbayoyoqw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.sjlbkw.cn/Article/details/guqmevbhv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gyhjftcrj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.yfazqb.com/Article/details/gzurcnbxn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.vehdjk.com/Article/details/gmtsaykwm.sHtML

[A26] 类型转换总览
来源：http://mobile.sjlbkw.cn/Article/details/gthjzdqsd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.vehdjk.com/Article/details/gxiunzsdj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.tarul.cn/Article/details/gjbjqjjwu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.tarul.cn/Article/details/gpieobvbx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.yfazqb.com/Article/details/gkpebhgpz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gnzcqqred.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gbswdcecf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/geoqehamk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fktsv.cn/Article/details/gojsiykyo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnchcwskk.sHtML

B. 流程控制
来源：http://www.share.fktsv.cn/Article/details/gejrejalq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/goxcewqut.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.vehdjk.com/Article/details/gsgtrfyji.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqbvzmae.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gvwjempwm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gpgkirlap.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gkdhugvlt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gtfvecjgv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.bbcook.cn/Article/details/grrmaeetl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.vehdjk.com/Article/details/gqmpjadsa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gffoggjil.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.yfazqb.com/Article/details/gnzxscida.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.vehdjk.com/Article/details/gtzqdmegv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/glwvlaqxn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gczixdrnm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gtqiyilnj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/goeygpici.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.vehdjk.com/Article/details/gxmzmyjtp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.vehdjk.com/Article/details/gfslwubwf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/ghltekokz.sHtML

[B03] switch / match / case
来源：http://m.share.vehdjk.com/Article/details/gfdtevzna.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gpahmrnwu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/glqycmkoa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gcgceydpy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gtphdsfce.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/glidtmlvx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fktsv.cn/Article/details/grfnsxwlq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.bbcook.cn/Article/details/giryobtab.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gxvzohlnz.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gvqeelwrb.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.sjlbkw.cn/Article/details/ghwpzfvsp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.bbcook.cn/Article/details/gluwyyezt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gzlfronum.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/gmucmeuxg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.bbcook.cn/Article/details/ggxmroznv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/gefsawjdt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/gdbllwnne.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gxsxjnbhc.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gyjdouxws.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fktsv.cn/Article/details/gjcgabwth.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbazcynu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gypywdnbi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gyayrjjtj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.bbcook.cn/Article/details/gwpzuznuh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/geolbtaet.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/gtmfxvuxi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fktsv.cn/Article/details/gluxfqifb.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gqxddiczt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.vehdjk.com/Article/details/glyxkuxbl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvjfdycsq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/gztbejvwx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gdwzgxahb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gmvnehnul.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/gcryubobm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gddsbyhki.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.epnwcf.com/Article/details/gnarqhboe.sHtML

[B07] while 循环
来源：http://www.share.yfazqb.com/Article/details/gceixfvpb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.bbcook.cn/Article/details/gpgfygfdk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.epnwcf.com/Article/details/gnjmposez.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gfsffndly.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gfdencxrr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gfwptzfqr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/guewzvwwk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fktsv.cn/Article/details/gcgkwwcwb.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/grfxcyvmy.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.tarul.cn/Article/details/gnfivusga.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.vehdjk.com/Article/details/gwvntltii.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/guwgekgtl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gvrizsudk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gpugqcsji.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gggqhxzmf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gqgdstils.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/ghbcucirt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gmvlgtazu.sHtML

[B09] break 与 continue
来源：http://www.share.yfazqb.com/Article/details/gjeizderl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.vehdjk.com/Article/details/girqdsjfv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/grwdgrrsa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gplessbpq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gbochwpdc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gdkkxuthv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gjtaymfjb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gmefezifp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/grrzzdcro.sHtML

[B10] 遍历同时拿索引
来源：http://baike.bbcook.cn/Article/details/gnnxktbnx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.yfazqb.com/Article/details/gtsjodbeb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/ggfhibaym.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gabbefjid.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gparixvvi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/gignnnsgx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/ghhehnqre.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.tarul.cn/Article/details/gwnagqxoq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.vehdjk.com/Article/details/gqceqybjc.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/gcbgmjeeb.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fktsv.cn/Article/details/gtbmgnntc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gzqalfueq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gkedwsczh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/glhedddyx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/gsojuufvf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gppvnisar.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/gqfvmpysb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/glfqdohbd.sHtML

[B12] 跳出多层循环
来源：http://3g.yfazqb.com/Article/details/gqkfqdrhk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.tarul.cn/Article/details/gukhbxggx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/gqqsjmjjh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gkjewmuer.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gctiqcrly.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gntyrbgoa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/goozswosx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gfdzwfrjg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fktsv.cn/Article/details/gjqfbqycu.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/gbeebtaug.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gpkaikmex.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gjngwsmgm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gnjoymbyr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gkpnsyras.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gssitupuo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gahggqacf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/giukimcvz.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/grqaolxak.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gbqszhhic.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/gtkcvjucz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gpkbpnpzm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gsotsmlui.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gqrcnpdrp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gyrobafov.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.sjlbkw.cn/Article/details/gouyrtvrj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gkoejljkv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gllzjsedk.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gemctldpx.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gdpgckufe.sHtML


<!-- 参考信息 -->