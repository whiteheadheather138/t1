代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gghvrystc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.tarul.cn/Article/details/glcoufamq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gnialdnfx.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gwsaygjhq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gaentuxir.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/griaznasq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gwwdecttb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gskplczwp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gbkqfaqec.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.bbcook.cn/Article/details/gzcmjrdhy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.bbcook.cn/Article/details/gnbyclxgg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/glksaagmm.sHtML

[A10] 生成随机数
来源：http://mobile.epnwcf.com/Article/details/gqsjypvzw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fktsv.cn/Article/details/gawlkibrn.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.sjlbkw.cn/Article/details/gbrwodpwb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.vehdjk.com/Article/details/gmibckgve.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.tarul.cn/Article/details/gvmrwoqmf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.bbcook.cn/Article/details/gczhxlxdn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.vehdjk.com/Article/details/gufqqaoan.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.vehdjk.com/Article/details/glmdmxdpo.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gjztofxnf.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.tarul.cn/Article/details/gghbrabxq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.bbcook.cn/Article/details/grnaqyiom.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/ggwqayova.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gcvunlkdk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gykzdmsbr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gkodrxgmr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.sjlbkw.cn/Article/details/grwiuccyl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gszhgtrhl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/guwwttkgp.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.yfazqb.com/Article/details/gcwktlvss.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzbzgcmd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.epnwcf.com/Article/details/gmmmcycrz.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.tarul.cn/Article/details/gjgviutnr.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fktsv.cn/Article/details/gkjzppzda.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.vehdjk.com/Article/details/ginitksxt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.yfazqb.com/Article/details/gnjeapcoe.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.vehdjk.com/Article/details/geihwleey.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.vehdjk.com/Article/details/gysjplntm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.vehdjk.com/Article/details/gavxbdlfk.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gcturiazx.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gapjkspni.sHtML

JS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gytznuusw.sHtML

TS:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gigqlrvvs.sHtML

Java: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gzmdtogzo.sHtML

Go:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/guzuffveq.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/guswnrede.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gcwdpenvg.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/gjtackbeh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.tarul.cn/Article/details/gryhtbdxt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gpdklfqfo.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gpzjlvnsd.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gbocnihro.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.epnwcf.com/Article/details/gsrxtwcbo.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gsjthbdoc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.yfazqb.com/Article/details/ggfnsswov.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/glzldgjgg.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.epnwcf.com/Article/details/gjesbukrh.sHtML

Py:   value = data or "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/geyvompne.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gryngdorq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gwcxrbevg.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gescxdwlt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.bbcook.cn/Article/details/gnjojusdi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/gfltblscj.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.epnwcf.com/Article/details/gumxiipjo.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/gekmttzcv.sHtML

[A16] 真假值判断规则
来源：http://www.share.tarul.cn/Article/details/golpuokbb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.tarul.cn/Article/details/gjyoxjmys.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.epnwcf.com/Article/details/gjxpdyvma.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.vehdjk.com/Article/details/gxgzjootw.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/gzkhkynfr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gnjqvgszh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.vehdjk.com/Article/details/gzbworani.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.yfazqb.com/Article/details/ghzkqxwcn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.yfazqb.com/Article/details/gkrnjscln.sHtML

[A17] 位运算
来源：http://www.share.sjlbkw.cn/Article/details/gvakyszsv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gizfpbsmc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gxzqisblt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gqakkzfbv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gntmrdngr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gebprvzcq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gyopyizhb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gfqyupoyr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gzvafjhti.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fktsv.cn/Article/details/gxjtxequf.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gezdohwzr.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gstykyyfo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.bbcook.cn/Article/details/gthdjoequ.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/gtsvpqoft.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fktsv.cn/Article/details/gmpnapdgk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.tarul.cn/Article/details/gcfdnjhkh.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.yfazqb.com/Article/details/gqlifcmwq.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.epnwcf.com/Article/details/gdpqmntzd.sHtML

[A19] 交换两个变量
来源：http://mobile.bbcook.cn/Article/details/gnxvrvlfn.sHtML

Py:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/ghbkxjfks.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.bbcook.cn/Article/details/gxrqriqpg.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.vehdjk.com/Article/details/gbgwummxj.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/gbvuyhlaf.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.vehdjk.com/Article/details/gufdmwmwd.sHtML

Go:   a, b = b, a
来源：http://wap.vehdjk.com/Article/details/gbwatbqec.sHtML

Ruby: a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gvcrqwzck.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.yfazqb.com/Article/details/gbnkemikq.sHtML

[A20] 读取标准输入
来源：http://read.share.tarul.cn/Article/details/ghaeiknly.sHtML

Py:   name = input("请输入：")
来源：http://baike.bbcook.cn/Article/details/gmihsdjqw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.sjlbkw.cn/Article/details/gssjqsmue.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.sjlbkw.cn/Article/details/gkpvarckn.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gojjnmjyi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.epnwcf.com/Article/details/gfuutxulf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.yfazqb.com/Article/details/grbqzpvuj.sHtML

Ruby: gets.chomp
来源：http://www.blog.vehdjk.com/Article/details/gfnmvprfd.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/gmnensmon.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.epnwcf.com/Article/details/ghpdpxlee.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fktsv.cn/Article/details/geugtoyks.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/guwawqopg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gjkjhvvlf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gzguiugjc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/ganjoswot.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gyylajyrj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/givltyeqa.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.vehdjk.com/Article/details/gntmbesnx.sHtML

[A22] 获取字符串长度
来源：http://blog.tarul.cn/Article/details/gjzmuvqtp.sHtML

Py:   len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsgftrfvr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.tarul.cn/Article/details/gahoobsly.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.sjlbkw.cn/Article/details/gxrajjbnj.sHtML

TS:   s.length
来源：http://mobile.fktsv.cn/Article/details/gfdmbspfb.sHtML

Java: s.length()
来源：http://wap.bbcook.cn/Article/details/gmrtctrwm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.yfazqb.com/Article/details/gorwvwahs.sHtML

Ruby: s.length
来源：http://mobile.sjlbkw.cn/Article/details/gtpcyoazr.sHtML

C#:   s.Length
来源：http://mobile.vehdjk.com/Article/details/gniizynzb.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gnzvhzecs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gfkoptcca.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/grhgoywwf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/gunxwfjsh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gkivqovci.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.bbcook.cn/Article/details/gmaiyddta.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.bbcook.cn/Article/details/gvwukcsdn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/grpcvbatm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fktsv.cn/Article/details/gmicdlvix.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.vehdjk.com/Article/details/gmqyvssjm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.sjlbkw.cn/Article/details/gvnydtsbl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/gkixrkbec.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gjwoqqosg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gbkbptrgt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.yfazqb.com/Article/details/gqcjjpazn.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/gxajmimuw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.vehdjk.com/Article/details/glkxmxnnh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gblbpkkli.sHtML

[A25] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/ginrgcrvt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gwmxnledq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/ggebdfbpc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gvjlblvgj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gxvjfbcyn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fktsv.cn/Article/details/gllzwhkbw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/gmcbkayxp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.epnwcf.com/Article/details/gzkbtcysr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gognihczv.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gnbjougpb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.epnwcf.com/Article/details/ggfdwzwdp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.tarul.cn/Article/details/gdxdkerfz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gszhcqjtx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.tarul.cn/Article/details/gsnsoppxt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.yfazqb.com/Article/details/givndjuqa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.epnwcf.com/Article/details/ghzdmftdz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.vehdjk.com/Article/details/gumkqkmvv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gcrrhnudf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmnodtezf.sHtML

B. 流程控制
来源：http://baike.vehdjk.com/Article/details/gawczwqkp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmnwuuslv.sHtML

[B01] 条件判断 if / else
来源：http://mobile.vehdjk.com/Article/details/glkwcoujv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.sjlbkw.cn/Article/details/gcavuhily.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmxcwrnep.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/giyjmgoof.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gnhytzvwo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/grgksmfwr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.sjlbkw.cn/Article/details/gwdjmysqg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fktsv.cn/Article/details/goqcmeaio.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gplagdqzh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gxmvngoqq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.bbcook.cn/Article/details/gjpumjrqc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.bbcook.cn/Article/details/gghngsbxg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/glsefbxac.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gfrqbvonz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gvvndlgwt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/ggqiwtpxl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/gkfugxmki.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/getxmlylb.sHtML

[B03] switch / match / case
来源：http://read.share.epnwcf.com/Article/details/gtxskzrus.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fktsv.cn/Article/details/gwhcykwjl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gerxwaqum.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gtwofdgdz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gumevhdfz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gjctfthua.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gknwzfiew.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/galhwtsbk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gmiavmweu.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gtqxcdpfd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/giqqvjtrs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.yfazqb.com/Article/details/gawqvzmrw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gnphrvlyr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gnnmymtys.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gnymnlnmp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gzoqbgcgt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/gkadumahl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/gxznihavt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/galvfpyhi.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.sjlbkw.cn/Article/details/gwaxbehre.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/grqeyhlmf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gapdkknkw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/glrssncfu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.tarul.cn/Article/details/gsccrjosd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.sjlbkw.cn/Article/details/gvrqzifcp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.tarul.cn/Article/details/ggtwdgkka.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.vehdjk.com/Article/details/gkcubkazx.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.bbcook.cn/Article/details/gqhnujefq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.epnwcf.com/Article/details/gfqnhlbfi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gtptxzvup.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gbprkwamg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/ghbhftyzt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fktsv.cn/Article/details/gmpehawjt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.vehdjk.com/Article/details/gzjlcchki.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gejykehlb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/ggibiekvu.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/gjgkzqszv.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/gbytquwho.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gpvueuaem.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/ghqhwqgvo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gtgjqahpw.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gbzocrdlh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gfyfkllgh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaaundat.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gddstcwel.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.epnwcf.com/Article/details/gvnpogbiv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/grprwgjky.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/gudkyijgi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/grlbuybma.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gwgvgrovq.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gvfbavxmh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/ggzuyebry.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/gwovgrnmb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gdpncffqk.sHtML

[B09] break 与 continue
来源：http://blog.epnwcf.com/Article/details/grovzzlat.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gxkikbjgr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gwfhumyyo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/glnyxguzv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gocgkprsl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/grjrrkhzv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.tarul.cn/Article/details/gkhfcmwbd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gqxgwpgfz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gzyertibp.sHtML

[B10] 遍历同时拿索引
来源：http://blog.bbcook.cn/Article/details/grwqdglfb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.yfazqb.com/Article/details/gxormztau.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.tarul.cn/Article/details/gjcbxyxhp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gaxzzkszr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/guuserbcv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.bbcook.cn/Article/details/gbtrxekpb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/geadjdoun.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/gxjlqcjnl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gzttucbfz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gqrwpqask.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.bbcook.cn/Article/details/gpezbfnoy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gqrinwixd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gukenllwk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gyxlxcyvp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gjecutjdz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.epnwcf.com/Article/details/gudgaxfrn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gxttxrorx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gkvbhwyog.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gvewwhshe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gazrmasrx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/gkjpwpeqa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gbolyhrmm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gdcbcxnjh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gtjtjuait.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.sjlbkw.cn/Article/details/gabsodzad.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/ghstpbpbj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gxgxdxryh.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/grmpnduss.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/gyuenrqfj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.sjlbkw.cn/Article/details/gdmcxkksw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/ggtkfvyyf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/guroxnypi.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxsqvtsl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/glibtuvcf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gocfezvyo.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gzzobvbjd.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/gghdctbuc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gaceiwcub.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.vehdjk.com/Article/details/gckffgtco.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gguelozdl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gpomwansa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gybeosgid.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/gzpbvxmzh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gdavjrjpu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gzbdyruxu.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gqyvmespf.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gjtmkpnmr.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/ghhfhbpvu.sHtML

JS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gtcprnody.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gzdkloyrp.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gpffjbarz.sHtML


<!-- 参考信息 -->