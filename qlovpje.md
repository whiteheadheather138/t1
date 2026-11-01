代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fktsv.cn/Article/details/gpwtarunq.sHtML

[A07] 数字转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxnbjnmyu.sHtML

Py:   str(42)
来源：http://3g.epnwcf.com/Article/details/gxwdcymec.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fktsv.cn/Article/details/gzsublorb.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.bbcook.cn/Article/details/gwzsxbhup.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gzntzlxlr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.vehdjk.com/Article/details/gvxsendcs.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.yfazqb.com/Article/details/gmpvgqqdk.sHtML

Ruby: 42.to_s
来源：http://read.share.epnwcf.com/Article/details/gmtnrddrl.sHtML

C#:   42.ToString()
来源：http://www.share.epnwcf.com/Article/details/gwfbvhjhn.sHtML

[A08] 取整与四舍五入
来源：http://m.share.epnwcf.com/Article/details/gmwjbfzkc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/glijidanq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.bbcook.cn/Article/details/gzylkoclt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gwzciaomt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.tarul.cn/Article/details/gtzivszzi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gcycroyjw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gjnewbeek.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.bbcook.cn/Article/details/ggkjcbryv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gwnjjcnux.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.yfazqb.com/Article/details/gghnnavxd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.vehdjk.com/Article/details/gjxinonch.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gfwvwynuk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gsagrcjrk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.yfazqb.com/Article/details/ghagtasug.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.yfazqb.com/Article/details/gnsmytjqd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.vehdjk.com/Article/details/gzpgowrga.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.vehdjk.com/Article/details/gvrsiiwjj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gwbvuetgw.sHtML

[A10] 生成随机数
来源：http://read.share.tarul.cn/Article/details/grqwtsizf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.yfazqb.com/Article/details/gijznjdal.sHtML

PHP:  random_int(1, 100);
来源：http://3g.tarul.cn/Article/details/gbanexslf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gyjjxopkq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.bbcook.cn/Article/details/gdsmuiumb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.sjlbkw.cn/Article/details/gonwosrqr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.sjlbkw.cn/Article/details/gvigrvjkv.sHtML

Ruby: rand(1..100)
来源：http://m.share.epnwcf.com/Article/details/gyoeakrvn.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.epnwcf.com/Article/details/gdcuilfno.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fktsv.cn/Article/details/gcrmjxvro.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqzdscwb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gzcciiumb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gzvjueocc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/ggmsglcxi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gdlffhgwi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fktsv.cn/Article/details/gzgxdqyzb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gfauicpiq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gmsbpxbds.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fktsv.cn/Article/details/gkoqzuycy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.tarul.cn/Article/details/gffuuczns.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.epnwcf.com/Article/details/guuijlahi.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.sjlbkw.cn/Article/details/gjjvtkgma.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/gjfgtqidy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.sjlbkw.cn/Article/details/gpcbdpdtt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.yfazqb.com/Article/details/gkwiplxth.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fktsv.cn/Article/details/ggkbsekyc.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.yfazqb.com/Article/details/gfdvkyhyt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.tarul.cn/Article/details/gcbqidvtn.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvugqvdqq.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gbelqfrht.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gwilhwwpz.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gefmcdtny.sHtML

Java: "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gbhffyowv.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gotnyafyr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gmldqguei.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/grgzuvdgh.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/gkoudalcv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.bbcook.cn/Article/details/gxmxmqowb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/gorpawlrf.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gjmlwergi.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/ggeptgyas.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.tarul.cn/Article/details/gaqlworct.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gzwgdtptp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.sjlbkw.cn/Article/details/gbbbnoleq.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gbkeljeny.sHtML

[A15] 空值判断与默认值
来源：http://m.share.epnwcf.com/Article/details/gaizjfsgi.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/gscsgqymo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gjdkrgfbt.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gpwoxqepw.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gkligwtzi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.vehdjk.com/Article/details/gazicsubr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fktsv.cn/Article/details/gwlwxsfya.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/gpzmtmxrb.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/ggkjrgrlo.sHtML

[A16] 真假值判断规则
来源：http://read.share.epnwcf.com/Article/details/gwzumnmpf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.sjlbkw.cn/Article/details/gevwlqznu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.sjlbkw.cn/Article/details/gkmmwswce.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.tarul.cn/Article/details/gnrzrazsh.sHtML

TS:   if (!x) {}
来源：http://www.share.vehdjk.com/Article/details/gkfgaizto.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.vehdjk.com/Article/details/gdkzihubg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.epnwcf.com/Article/details/gbczldadj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.yfazqb.com/Article/details/gmvvujoco.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwipqyryu.sHtML

[A17] 位运算
来源：http://3g.epnwcf.com/Article/details/gpdkexjcg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/guldjfqst.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.bbcook.cn/Article/details/govspuyma.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gfjviyzcc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gfgixcims.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gsranlypi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gxtmfuqoj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gflgbasuv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gvadiyuwh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.yfazqb.com/Article/details/gqvtmktxj.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.epnwcf.com/Article/details/gyhsxskrt.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/ggmoezgvx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fktsv.cn/Article/details/gohlnrcyd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gfemffngh.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.bbcook.cn/Article/details/gazklhxun.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.vehdjk.com/Article/details/gzfyzmqqd.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.tarul.cn/Article/details/giumlfeed.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fktsv.cn/Article/details/gdfmraxqh.sHtML

[A19] 交换两个变量
来源：http://3g.bbcook.cn/Article/details/gdyllkxrd.sHtML

Py:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gubmahtdg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.yfazqb.com/Article/details/gpvzzkzgt.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gwhdcrapx.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/ghedowixm.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.yfazqb.com/Article/details/gzvxxnkqk.sHtML

Go:   a, b = b, a
来源：http://m.share.tarul.cn/Article/details/gtfzzhyid.sHtML

Ruby: a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gzyikcweu.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.bbcook.cn/Article/details/gufvxxpev.sHtML

[A20] 读取标准输入
来源：http://m.share.bbcook.cn/Article/details/gbtfnebmu.sHtML

Py:   name = input("请输入：")
来源：http://baike.bbcook.cn/Article/details/gimwddjtl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.epnwcf.com/Article/details/geowvfxbe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.epnwcf.com/Article/details/gtbsfmcdk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.bbcook.cn/Article/details/gvxmfoupf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gfklajtqw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.epnwcf.com/Article/details/gudzgnnmq.sHtML

Ruby: gets.chomp
来源：http://baike.bbcook.cn/Article/details/guwbjoveg.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.vehdjk.com/Article/details/gkkeuvccv.sHtML

[A21] 保留指定小数位输出
来源：http://wap.bbcook.cn/Article/details/gqbcrdmyu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.vehdjk.com/Article/details/gunwacreb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gyxyomoxv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjenanlzk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gnqbcaygf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gkcheqkju.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/ggorhnelb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gtezitxzt.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.sjlbkw.cn/Article/details/gonkcwkai.sHtML

[A22] 获取字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gldtagwki.sHtML

Py:   len(s)
来源：http://wap.sjlbkw.cn/Article/details/gypaqiomr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.bbcook.cn/Article/details/gunhizfbq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.epnwcf.com/Article/details/gqobanyti.sHtML

TS:   s.length
来源：http://blog.vehdjk.com/Article/details/gcavmheff.sHtML

Java: s.length()
来源：http://baike.epnwcf.com/Article/details/gzbfvktkf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.tarul.cn/Article/details/gjgugwzgf.sHtML

Ruby: s.length
来源：http://blog.sjlbkw.cn/Article/details/gpsdnxyaz.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/gibautwdi.sHtML

[A23] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gfbywmbil.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.vehdjk.com/Article/details/galhbbwkp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.sjlbkw.cn/Article/details/gplnqbtii.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gxdgmmdnv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/gdfgcjfaj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gyvxeqqlx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/glcoxxoid.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.epnwcf.com/Article/details/gtamnpksr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.bbcook.cn/Article/details/gyybcfucy.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gmyrvwocz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.tarul.cn/Article/details/geimjwrfy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.vehdjk.com/Article/details/gvcwjqefv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/ggtgijems.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gcmptzlgj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.bbcook.cn/Article/details/gtzveszjh.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/gdaesztrj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gvahswrzq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.vehdjk.com/Article/details/gftmyocbp.sHtML

[A25] 字符串比较
来源：http://3g.tarul.cn/Article/details/gqayjgmzf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fktsv.cn/Article/details/glpklveit.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.tarul.cn/Article/details/geaeistgp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gcaoiglio.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/giuivqgyn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gwfzmmost.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/glmrzwhyq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.sjlbkw.cn/Article/details/gilwozlrk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gzuwgosxr.sHtML

[A26] 类型转换总览
来源：http://baike.fktsv.cn/Article/details/gkazjksbe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gdoizustg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gnkujmnhw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.bbcook.cn/Article/details/gsvadqdmh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.yfazqb.com/Article/details/goyfljegc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gzxchkefa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.bbcook.cn/Article/details/gjgmvybxf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/gnpyxbnfn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gezplwzdd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gakqeudvy.sHtML

B. 流程控制
来源：http://www.share.vehdjk.com/Article/details/glpreudic.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwbkxzudh.sHtML

[B01] 条件判断 if / else
来源：http://www.share.yfazqb.com/Article/details/gomxvahau.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.epnwcf.com/Article/details/gelnhsktr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/gnxqggprr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gvnuwayda.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gmwbzbnpa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/ghiqzoasv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fktsv.cn/Article/details/gwtemvceb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fktsv.cn/Article/details/gbtdoskqv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/glekupdfq.sHtML

[B02] 多分支 else if / elif
来源：http://blog.sjlbkw.cn/Article/details/geybdgurr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.yfazqb.com/Article/details/gxskttemt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fktsv.cn/Article/details/geljsdxyv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gnuuaxrit.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gclxrqbey.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gbnkdvluq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gtgvrepqr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.yfazqb.com/Article/details/gejbaphes.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gywjfqqob.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/gyxassejx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/gfhwultxi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/genadnqik.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/grrhwkqji.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gaucllwde.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gvampmqom.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/gdlvfxyha.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.sjlbkw.cn/Article/details/gqzzhtthc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gyowommle.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gqcipobtu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/ghuumetff.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.yfazqb.com/Article/details/gacnxnhhq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gftlqjbfg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gssuhivyi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gnjehattr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.yfazqb.com/Article/details/grwgtvoyj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/gvgmoljis.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/ghbjhiikr.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.tarul.cn/Article/details/gfinxuqmz.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/gmlybhfcg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/gfbochuxj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/giqlbtgnx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/gdmkftllo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.vehdjk.com/Article/details/gwhsmuorc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/grtaemziw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gfgfhnjgt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fktsv.cn/Article/details/gabvajxym.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.vehdjk.com/Article/details/gzmaflgma.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gnnqttzqg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fktsv.cn/Article/details/gelsoekmq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/grflodgmt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gchkkvoxw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/ggtgyzvfb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/gxrdzyiuw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/glpsyjkfj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gwyljgvol.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gdyasotdp.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.bbcook.cn/Article/details/gylivecjw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/gxeugvdog.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gdvztyeje.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gjgmmaigi.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gjtvuxinm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gdqushthl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gikbbztlj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/ggpwafhho.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.epnwcf.com/Article/details/glavkyoqo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gpbabkbtv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/gzybrsaav.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/getqinnmj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gcolxboyt.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gpbtczqhy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gnefdslxd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.epnwcf.com/Article/details/gleoxxonl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gpqadzogs.sHtML

[B09] break 与 continue
来源：http://www.blog.yfazqb.com/Article/details/gtmzebkru.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/gguuppvtv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gbdvykzhr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/glkfsrtvr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gzarzzupi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gqeulflxz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gpzztlujc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gbjbmdwgf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/ggjwtnpxp.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/grbompaxd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.bbcook.cn/Article/details/ghgocmqwy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.vehdjk.com/Article/details/gtnfhaswq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gawibwicr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gegnpawdb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gsbxouirf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.epnwcf.com/Article/details/glgbqczoh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.sjlbkw.cn/Article/details/gftnbmbus.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/ggcymtnau.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gcbvfimcr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/gvaetuehq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.sjlbkw.cn/Article/details/guborlopt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gkivvmbyv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/galqawitn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/glrfnlfsw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/gtjkuywkh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gonuowgwe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.tarul.cn/Article/details/gixeeepgi.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gtqrkfksy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.yfazqb.com/Article/details/gguecuyvt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gwzicygie.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gwufwqimw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gpcmsmejx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gqdnfmtfr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fktsv.cn/Article/details/gsaixjmob.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gwofypfcc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/ggybzlcxo.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gymldbzrm.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.epnwcf.com/Article/details/gsedqvgjc.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gxgfaglxu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfahdavv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/ghvcfzfwu.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gdoxmzdfk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/geejegztx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gnhnwwznx.sHtML


<!-- 参考信息 -->