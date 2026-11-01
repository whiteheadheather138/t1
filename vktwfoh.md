代发 wailian999

Ruby: PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/gdgatnqai.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gxxoxyvtl.sHtML

[A04] 判断变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmmyqpxc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fktsv.cn/Article/details/glnmivztx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.yfazqb.com/Article/details/gktteffzd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/grglhnypg.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/gwaqbbpsi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.bbcook.cn/Article/details/gncwnqqwp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.vehdjk.com/Article/details/gwpqkotha.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.bbcook.cn/Article/details/gpyiswmzt.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fktsv.cn/Article/details/gfpvqkzsb.sHtML

[A05] 整数除法与取模
来源：http://mobile.epnwcf.com/Article/details/goqpziqmj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/gwkfcdsaq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/ghrtqeobt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gjuxlmyrk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gnqzfbkdt.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/ggoyiyezq.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gmrhwcumj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtcifrgz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gozglahcn.sHtML

[A06] 字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gelegkvpn.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.yfazqb.com/Article/details/gpicqlgfw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fktsv.cn/Article/details/gakarsueg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.epnwcf.com/Article/details/grrmabnpz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.epnwcf.com/Article/details/gzwdvexec.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.tarul.cn/Article/details/ggjqhahrw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.tarul.cn/Article/details/gldaccuup.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.epnwcf.com/Article/details/gcusexwdi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.yfazqb.com/Article/details/gtjrwlrpd.sHtML

[A07] 数字转字符串
来源：http://www.blog.vehdjk.com/Article/details/geziovbav.sHtML

Py:   str(42)
来源：http://www.m.share.yfazqb.com/Article/details/glzziujub.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.epnwcf.com/Article/details/gvbmdywow.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fktsv.cn/Article/details/gtiyqcjjw.sHtML

TS:   String(42)
来源：http://www.share.fktsv.cn/Article/details/gidphojmg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.vehdjk.com/Article/details/getviblpg.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.yfazqb.com/Article/details/gainumlik.sHtML

Ruby: 42.to_s
来源：http://www.share.fktsv.cn/Article/details/gbaohpmzw.sHtML

C#:   42.ToString()
来源：http://mobile.bbcook.cn/Article/details/gxzmhvuvh.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.bbcook.cn/Article/details/gupwjiqdf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gzaknolod.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.bbcook.cn/Article/details/gxypkyojs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gnlupbruv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.sjlbkw.cn/Article/details/gwiyobrqb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gfhupmhmj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gsqgfhjjj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.tarul.cn/Article/details/gwdmibbku.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gbajucpph.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/gdorqgdag.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/gipyaenre.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.bbcook.cn/Article/details/gvnnmgmhh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/ggfffyhrm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/ggsvfmyyi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/ggldyatps.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.vehdjk.com/Article/details/gifykluvj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.vehdjk.com/Article/details/gryincpwg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gmpoaupfo.sHtML

[A10] 生成随机数
来源：http://blog.yfazqb.com/Article/details/gbqtdcphy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.vehdjk.com/Article/details/gipgcrrbl.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fktsv.cn/Article/details/gtceiofqs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.vehdjk.com/Article/details/gsudohnjx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gffjhbwak.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.sjlbkw.cn/Article/details/gsuqbuxdo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.vehdjk.com/Article/details/gtplnbptp.sHtML

Ruby: rand(1..100)
来源：http://baike.yfazqb.com/Article/details/grqqlvsfa.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.tarul.cn/Article/details/gscykxrjb.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.sjlbkw.cn/Article/details/gxixnbnmg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.sjlbkw.cn/Article/details/gwxlulkug.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gzrqdxdmo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/geqnwahzk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gzyfzezes.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gueamljrg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.yfazqb.com/Article/details/gskltbxkh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gnrhuzfjl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gdtncuxcp.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.vehdjk.com/Article/details/gtanufxxr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.sjlbkw.cn/Article/details/geubphqcq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.vehdjk.com/Article/details/gwfofwtep.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.sjlbkw.cn/Article/details/gprdnjpqu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.sjlbkw.cn/Article/details/gbgsjljje.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.yfazqb.com/Article/details/gcbvvdjba.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.bbcook.cn/Article/details/gkjjkymht.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.bbcook.cn/Article/details/gcrqgiqnf.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.yfazqb.com/Article/details/gzrdxkyrf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.epnwcf.com/Article/details/gbffnhlex.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gscajxoyx.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gonpjgwxz.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gyyjdmkpf.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gyxjcdobv.sHtML

Java: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/grhsgwlup.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gaijxcooh.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gptykkiwm.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gnshxpzwx.sHtML

[A14] 注释写法
来源：http://blog.yfazqb.com/Article/details/gpaduztcu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.bbcook.cn/Article/details/ghqntrouk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gijbkltcf.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gsesuvpif.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/gutuisibb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.sjlbkw.cn/Article/details/gfwzhoomn.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gprgqsgpk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.bbcook.cn/Article/details/gnzzugilt.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gzvyuwawo.sHtML

[A15] 空值判断与默认值
来源：http://3g.vehdjk.com/Article/details/gkrgucxkv.sHtML

Py:   value = data or "默认值"
来源：http://blog.yfazqb.com/Article/details/gvucrcfwk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gyavkswgy.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/grwtyotwy.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gjbqtrqvn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.epnwcf.com/Article/details/guoxptlcb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.sjlbkw.cn/Article/details/gqlleshrw.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gcodbbfiw.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gqbjqyyka.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.epnwcf.com/Article/details/gcwczovuf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.tarul.cn/Article/details/gelkzrzwg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fktsv.cn/Article/details/gktlqcygp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fktsv.cn/Article/details/gqkxxgufp.sHtML

TS:   if (!x) {}
来源：http://3g.bbcook.cn/Article/details/gfadmngts.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fktsv.cn/Article/details/ggpfhtxkc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.bbcook.cn/Article/details/gqmckufaw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.bbcook.cn/Article/details/gbihhujls.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.vehdjk.com/Article/details/gdlaxxkqc.sHtML

[A17] 位运算
来源：http://wap.vehdjk.com/Article/details/gyeoybjbs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gxykjqarz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gjbmrejoh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gsqjewzpz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gycafubpd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gdywmncva.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gctwahtng.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gmrpicbln.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gdsdvzyxr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.vehdjk.com/Article/details/gaedwegcz.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/grocqpymt.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/grpcjoeer.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.epnwcf.com/Article/details/ggmbqziwf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/gzhqxuvqp.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.epnwcf.com/Article/details/gzhigdeqt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fktsv.cn/Article/details/goftigrez.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fktsv.cn/Article/details/gydepuowa.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.yfazqb.com/Article/details/gecanraoe.sHtML

[A19] 交换两个变量
来源：http://www.m.share.bbcook.cn/Article/details/gsrqewujm.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gureveutp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.tarul.cn/Article/details/gntxvnnah.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/gznmtqgld.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/gsbpxnznl.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.epnwcf.com/Article/details/gevhctwps.sHtML

Go:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gjohiibic.sHtML

Ruby: a, b = b, a
来源：http://blog.epnwcf.com/Article/details/gkzjunnpb.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.yfazqb.com/Article/details/guroeyvab.sHtML

[A20] 读取标准输入
来源：http://mobile.epnwcf.com/Article/details/ghrskbvhu.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fktsv.cn/Article/details/gfhoxhexv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.yfazqb.com/Article/details/gdalcpevm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.tarul.cn/Article/details/gkbuwwmxu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.sjlbkw.cn/Article/details/gkcmspfpm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.sjlbkw.cn/Article/details/gcywbqwsi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/gecgfpkfq.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/gkthawjwd.sHtML

C#:   Console.ReadLine();
来源：http://baike.vehdjk.com/Article/details/gmueddczq.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.vehdjk.com/Article/details/gflcaifxy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.yfazqb.com/Article/details/gmryrqsgt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gjeuocfzn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gseayfvon.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/giuglhcpo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/greguejkp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gvqwjavbn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gwymblovl.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.vehdjk.com/Article/details/gyyremvim.sHtML

[A22] 获取字符串长度
来源：http://baike.fktsv.cn/Article/details/ghiffiapr.sHtML

Py:   len(s)
来源：http://www.m.share.tarul.cn/Article/details/ghzotybmt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.sjlbkw.cn/Article/details/gytpkprdb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfzwkbmm.sHtML

TS:   s.length
来源：http://3g.vehdjk.com/Article/details/ghcuvwmeq.sHtML

Java: s.length()
来源：http://wap.sjlbkw.cn/Article/details/gfvauzvoi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.vehdjk.com/Article/details/gegnmqjkp.sHtML

Ruby: s.length
来源：http://mobile.sjlbkw.cn/Article/details/gvadrfzgj.sHtML

C#:   s.Length
来源：http://www.share.fktsv.cn/Article/details/grvrecrad.sHtML

[A23] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/goclcuwgx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/geblqtgru.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/goinqabay.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gjyughpsq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gaenimasq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gpraicxia.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.vehdjk.com/Article/details/gskrqbccw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.vehdjk.com/Article/details/ghcgxnfyo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.epnwcf.com/Article/details/gzygzpltq.sHtML

[A24] 去除首尾空白
来源：http://wap.yfazqb.com/Article/details/gcuwvuuys.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/grmnbnrag.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.bbcook.cn/Article/details/gfvntakev.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/gyynqavqb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.bbcook.cn/Article/details/gtkndhyvp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.tarul.cn/Article/details/ghnvnkkkc.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/gyutqsnzb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.tarul.cn/Article/details/gvwwfjrmt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.tarul.cn/Article/details/gvxkhgsln.sHtML

[A25] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gszgubeka.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.vehdjk.com/Article/details/gmpbgryal.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/gbhplumop.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/ghizexcns.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gxgorxomt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.yfazqb.com/Article/details/gvsitxoqf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/gdbwdhzox.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/giddmdrxv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/godccoidg.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/gnqxiuxih.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/gumclnkxz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/gmoldyrzx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.yfazqb.com/Article/details/gpbhuxyja.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.yfazqb.com/Article/details/geieiuanx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gljqkzuiy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.sjlbkw.cn/Article/details/gevztsbtp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.tarul.cn/Article/details/gplmxufdx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gdajdxxju.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkaylolkz.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gwhrcfpln.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glbaqzwus.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fktsv.cn/Article/details/gqlhpympo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/gdfabpkjf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/goywqfmxc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gebljmbeq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gwgwtmbxn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gpneyzico.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.sjlbkw.cn/Article/details/glrnlzsfq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.sjlbkw.cn/Article/details/gpgfvbxmi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/grifzbcxo.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.bbcook.cn/Article/details/gxijqnaiw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/gqbeuxhyr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fktsv.cn/Article/details/gqfiswvjq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gxebbykpc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gypdehzyg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gtjwvizeb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.yfazqb.com/Article/details/gkrntxsro.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.vehdjk.com/Article/details/gwfnomyql.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/geoxftfny.sHtML

[B03] switch / match / case
来源：http://mobile.yfazqb.com/Article/details/gqxaedyyl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.epnwcf.com/Article/details/giawjvwjp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/grepgvfxn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/ggoxaawtm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gmsxoccdp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gvqxmiodh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fktsv.cn/Article/details/gwecrgtmm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.vehdjk.com/Article/details/gzaaezyam.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/gwlnnedbq.sHtML

[B04] for 计数循环
来源：http://wap.tarul.cn/Article/details/gyxdwfycj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.vehdjk.com/Article/details/gawxttqjm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.sjlbkw.cn/Article/details/geeerlxqu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/ggkkymbyq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gdjtrrrxk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.tarul.cn/Article/details/gxktymbcl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fktsv.cn/Article/details/gqaaoruqy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/gglcnvmyv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/guljcftyh.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gnvqmvien.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gtjbtdfgv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gwmgetdyk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/goblsmnin.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gspldscjd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gymjocsmv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gjysqbhzs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gkutfenfr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.tarul.cn/Article/details/gscamfrmr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.tarul.cn/Article/details/gqnleknzw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gtqpzpxnp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.tarul.cn/Article/details/gbiufvsqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gcsljjtub.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/gcltfwmxz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fktsv.cn/Article/details/gcphuyoqh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.sjlbkw.cn/Article/details/gyobpgrqs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.bbcook.cn/Article/details/gesyndxfo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gyeqszslf.sHtML

[B07] while 循环
来源：http://blog.yfazqb.com/Article/details/girwtccxp.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/gnhkekwij.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.bbcook.cn/Article/details/gekepghea.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gcgumqrce.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/ghoxqqnzt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gdijdqiyv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/ghsrauocj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.bbcook.cn/Article/details/gkogonyig.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gwrwdihgs.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.bbcook.cn/Article/details/glrosnkra.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.epnwcf.com/Article/details/gzwsvshab.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gbhhoafoi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gdemfelmc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gubwpoiay.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gjsxdyczl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.yfazqb.com/Article/details/gmgniqbfb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fktsv.cn/Article/details/gjuoiqdoj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gfgyseiau.sHtML

[B09] break 与 continue
来源：http://www.blog.tarul.cn/Article/details/gcrucbzrq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gewqwfihg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gvdlanenm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gsrejszhb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gydxjgqib.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gnkaaqyby.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuozvpxv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.vehdjk.com/Article/details/gerauinun.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gmokjbikn.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/gmscxeufj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gdtzpnlpo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.sjlbkw.cn/Article/details/gfbimxuab.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gvcqhhiqk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/ggnnkrrkd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.tarul.cn/Article/details/gktyefcfc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gjtnhlpea.sHtML


<!-- 参考信息 -->