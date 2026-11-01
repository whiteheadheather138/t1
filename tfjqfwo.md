代发 wailian999

Ruby: PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gujvebhkq.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gviitmucn.sHtML

[A04] 判断变量类型
来源：http://3g.epnwcf.com/Article/details/gsewujbza.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.tarul.cn/Article/details/guxbqbokb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.sjlbkw.cn/Article/details/gbcscrzrk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.tarul.cn/Article/details/gevypafth.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/glwymbtyk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.sjlbkw.cn/Article/details/goaxkajmb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fktsv.cn/Article/details/gouecryyw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/gstqytxyz.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.sjlbkw.cn/Article/details/gpfltland.sHtML

[A05] 整数除法与取模
来源：http://baike.vehdjk.com/Article/details/gvodpozot.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.bbcook.cn/Article/details/gqrphxvwc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/govpjyykh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gqlnifrge.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gedwlintk.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gfipyoxos.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gzksytrdb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gjiemjxxl.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/ggnqkwitf.sHtML

[A06] 字符串转数字
来源：http://blog.fktsv.cn/Article/details/gcbbrctxm.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.tarul.cn/Article/details/gkkfeswnc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.epnwcf.com/Article/details/gmwfsovad.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/gmketgkop.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.yfazqb.com/Article/details/gstfhszhg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.tarul.cn/Article/details/gbpgoucvv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.sjlbkw.cn/Article/details/gqppzvojt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.sjlbkw.cn/Article/details/gedqtxrfl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.bbcook.cn/Article/details/gnqchdzdr.sHtML

[A07] 数字转字符串
来源：http://m.share.bbcook.cn/Article/details/giueislhf.sHtML

Py:   str(42)
来源：http://www.blog.epnwcf.com/Article/details/gjummkolw.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.epnwcf.com/Article/details/glvsyaqjj.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.tarul.cn/Article/details/gvsaemuud.sHtML

TS:   String(42)
来源：http://www.blog.yfazqb.com/Article/details/gukkcovpz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.tarul.cn/Article/details/gijuzdowb.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.sjlbkw.cn/Article/details/gtitkszlo.sHtML

Ruby: 42.to_s
来源：http://www.blog.yfazqb.com/Article/details/gsbtgzxok.sHtML

C#:   42.ToString()
来源：http://m.share.tarul.cn/Article/details/gxcosgigc.sHtML

[A08] 取整与四舍五入
来源：http://blog.bbcook.cn/Article/details/gbgpzxpzm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/grolwmypq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.sjlbkw.cn/Article/details/gpfdllxdp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gbahqxtll.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.vehdjk.com/Article/details/gccedsrgp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gmejrpmpq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gmdjgaqiv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.tarul.cn/Article/details/gitrcpwgr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gleesdmvy.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/ggohluprv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gboojmmmi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfsmygmt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gpocptoos.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gowegngpv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ghndouegn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.yfazqb.com/Article/details/gcssncunb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.vehdjk.com/Article/details/grndmqyfa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gkiuettod.sHtML

[A10] 生成随机数
来源：http://www.blog.tarul.cn/Article/details/gbexgocex.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.sjlbkw.cn/Article/details/geazwlnje.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.yfazqb.com/Article/details/guglzrjpa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.tarul.cn/Article/details/gflpkrzuy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gmgssthmn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.tarul.cn/Article/details/gfgigojvs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.yfazqb.com/Article/details/gmfbmvcrn.sHtML

Ruby: rand(1..100)
来源：http://www.blog.yfazqb.com/Article/details/gajtevfps.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.epnwcf.com/Article/details/gypaffspi.sHtML

[A11] 条件表达式（三元）
来源：http://baike.tarul.cn/Article/details/geusxhfel.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.epnwcf.com/Article/details/gvtldwvlz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gkseyaerh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/glicqeonm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gevxuthxr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/ghbjouswq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.tarul.cn/Article/details/gtbrrcdte.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gtnocwufz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gkgjmvmfr.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.bbcook.cn/Article/details/giccatcyn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.epnwcf.com/Article/details/gylwwtrme.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.bbcook.cn/Article/details/gmdjqhnfp.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.sjlbkw.cn/Article/details/gtbihjysp.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gjkbtluoh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.vehdjk.com/Article/details/gkfehgwhu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.epnwcf.com/Article/details/gtvlfffks.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.tarul.cn/Article/details/gdpfuhsgs.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.bbcook.cn/Article/details/gsqrrcmwe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.epnwcf.com/Article/details/gdqnnuzpb.sHtML

Py:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gzbjbmmvo.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gbyqzputv.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gekszksps.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gurrdntdq.sHtML

Java: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gqxyvcyqx.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gltnyqckw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gntebpqia.sHtML

C#:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gybwlqkzq.sHtML

[A14] 注释写法
来源：http://www.share.yfazqb.com/Article/details/gxikmnlac.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fktsv.cn/Article/details/glieoewpo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/gznfqbuvs.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gwxilsest.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gigcdqsnb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.vehdjk.com/Article/details/gsgiuipcm.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gzrtqfbqu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.tarul.cn/Article/details/gwvdnlyac.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gjmrldngz.sHtML

[A15] 空值判断与默认值
来源：http://blog.vehdjk.com/Article/details/gfgmikrng.sHtML

Py:   value = data or "默认值"
来源：http://wap.vehdjk.com/Article/details/gukrvfibv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gqbdazzds.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gtxmejzeo.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gwkadqznb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.epnwcf.com/Article/details/gefggstgr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.sjlbkw.cn/Article/details/geskpnmin.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.tarul.cn/Article/details/ganqjaunh.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gbsnzbjfk.sHtML

[A16] 真假值判断规则
来源：http://wap.vehdjk.com/Article/details/gpjxzdvpz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/gobzxbwfg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.yfazqb.com/Article/details/glgbxjrcw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fktsv.cn/Article/details/ggzdduvxm.sHtML

TS:   if (!x) {}
来源：http://blog.epnwcf.com/Article/details/gzskbrmrp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.epnwcf.com/Article/details/gehoassah.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.bbcook.cn/Article/details/gzuumutrn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.vehdjk.com/Article/details/gzpaukyzj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gjwbtszkm.sHtML

[A17] 位运算
来源：http://blog.vehdjk.com/Article/details/gvmuawddb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gwxzijgol.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fktsv.cn/Article/details/glhpueawd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gkorzxuxt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gqvhonusg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gcbybpayq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gdzjluxfa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gyimejuou.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gbgxfechg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.tarul.cn/Article/details/gjkrnoebu.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/geaskjidt.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gcjvyokjg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/gmfyzlbte.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/gklwfrosh.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.bbcook.cn/Article/details/gsbtuhoqj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fktsv.cn/Article/details/gufinivfy.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.bbcook.cn/Article/details/gpjifwffx.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.epnwcf.com/Article/details/gaxbffeob.sHtML

[A19] 交换两个变量
来源：http://mobile.fktsv.cn/Article/details/gxptkxryj.sHtML

Py:   a, b = b, a
来源：http://blog.tarul.cn/Article/details/gfnmlwsiy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.bbcook.cn/Article/details/gtuksrxzd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gnieoloxy.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gvjidoaia.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.yfazqb.com/Article/details/gktsqlbmh.sHtML

Go:   a, b = b, a
来源：http://www.share.vehdjk.com/Article/details/gudjfhxqg.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gfedpuztf.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.epnwcf.com/Article/details/ghoizyerj.sHtML

[A20] 读取标准输入
来源：http://mobile.bbcook.cn/Article/details/gqutlbokt.sHtML

Py:   name = input("请输入：")
来源：http://3g.sjlbkw.cn/Article/details/gbuqvrvnn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.sjlbkw.cn/Article/details/gpammyuva.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.tarul.cn/Article/details/gmbfsvsbu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.yfazqb.com/Article/details/gesmsvgey.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.tarul.cn/Article/details/gxxsjgrrw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/gxvnxlhva.sHtML

Ruby: gets.chomp
来源：http://baike.fktsv.cn/Article/details/gctrzntlx.sHtML

C#:   Console.ReadLine();
来源：http://3g.yfazqb.com/Article/details/gumoocezj.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.vehdjk.com/Article/details/gfgvlqphq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.tarul.cn/Article/details/ghzgpviml.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gtzxrayor.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gzwjtchrt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gklepdnnh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gkrcgqkbj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gtjylkhqz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/guzakmkss.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.epnwcf.com/Article/details/ggslxrnkb.sHtML

[A22] 获取字符串长度
来源：http://mobile.bbcook.cn/Article/details/gbhysqpcr.sHtML

Py:   len(s)
来源：http://www.share.fktsv.cn/Article/details/gjxpbebwn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.yfazqb.com/Article/details/gcieowhoi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.tarul.cn/Article/details/gbxfvyfvb.sHtML

TS:   s.length
来源：http://www.share.epnwcf.com/Article/details/goqmbcpjt.sHtML

Java: s.length()
来源：http://baike.bbcook.cn/Article/details/gezvmdgkm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.yfazqb.com/Article/details/gjipchzpg.sHtML

Ruby: s.length
来源：http://3g.bbcook.cn/Article/details/guexdddjy.sHtML

C#:   s.Length
来源：http://wap.yfazqb.com/Article/details/gpgilycck.sHtML

[A23] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gqfdjhcxz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fktsv.cn/Article/details/gxwnblejn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/grwxcerlw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gyzflomrh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gnugqclen.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/geihxjwxf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.epnwcf.com/Article/details/gelwvwafv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.yfazqb.com/Article/details/gpaletsxl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fktsv.cn/Article/details/gsagoloae.sHtML

[A24] 去除首尾空白
来源：http://www.blog.sjlbkw.cn/Article/details/gnujfalbv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.sjlbkw.cn/Article/details/gkrhcayrf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.epnwcf.com/Article/details/gcecbxfaz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gdaoojocs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gkfeqcpjk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.epnwcf.com/Article/details/gfhnrqhig.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.yfazqb.com/Article/details/gjtccefnt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.sjlbkw.cn/Article/details/gowvvrmym.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.vehdjk.com/Article/details/gratlmhuu.sHtML

[A25] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gkpxtfgdo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.epnwcf.com/Article/details/gtaockvuu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/gmmwcyrda.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.sjlbkw.cn/Article/details/gsykbqian.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/giqfgqolc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/grypvlrgn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gahndguoy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.vehdjk.com/Article/details/gahfrsfvx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/gxnkynjnc.sHtML

[A26] 类型转换总览
来源：http://3g.yfazqb.com/Article/details/guhtnduxk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.bbcook.cn/Article/details/gvfjgqghc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.yfazqb.com/Article/details/gxfzvznoq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.yfazqb.com/Article/details/gaitksety.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gejmtaoif.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/gfybhgnpj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.bbcook.cn/Article/details/gxlvctbbd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.bbcook.cn/Article/details/gdkmsljsg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/ganugpgjr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnjyihuwu.sHtML

B. 流程控制
来源：http://read.share.fktsv.cn/Article/details/gvfxllhwo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzfrznmug.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fktsv.cn/Article/details/gzzqbgltz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/grkwencvg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/gyjuojbix.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gcxylupzl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/guzqxgdoe.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gctlxhnwz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.yfazqb.com/Article/details/gvzommjiv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fktsv.cn/Article/details/gjdeomyan.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gtysoiopo.sHtML

[B02] 多分支 else if / elif
来源：http://wap.sjlbkw.cn/Article/details/gelcqooyx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fktsv.cn/Article/details/gigsaxrdj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.yfazqb.com/Article/details/guftkoxzk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gqlycmahj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gfwtuacyw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gxncawxzm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gshjrlhio.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/gloaygxay.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gejurlqky.sHtML

[B03] switch / match / case
来源：http://mobile.sjlbkw.cn/Article/details/gvpygxryb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.bbcook.cn/Article/details/gljezrqqc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/ghqwgnwdm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gjdfmblxk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/guoqycqkz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gopayiphm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gaflrxnpo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.epnwcf.com/Article/details/gintiexbg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/glxejpbrp.sHtML

[B04] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gmmhnbulv.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gohmvmymp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/gauspmdbw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gclexklxi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/gexwsykrs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.epnwcf.com/Article/details/geyduitfq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gphmgpmsy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/ghhcsrdqn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.vehdjk.com/Article/details/gzscfnxld.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gehuvqpgk.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gqieobuzy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gkrpbullr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/geevjtjgt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gpuhdksbw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gcmehfgpe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/grgepwdki.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/gzcskduxi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fktsv.cn/Article/details/gdupdivmu.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/gtlhvvvfs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/gbdfkcxmw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.tarul.cn/Article/details/gxfikpxyh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gwcudtrpo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gnxrjozpa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/gybdcljxh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.vehdjk.com/Article/details/gehulnmkv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/ghaytjtvt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gjwqmbwvz.sHtML

[B07] while 循环
来源：http://3g.vehdjk.com/Article/details/gehfmxzba.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gskcenjon.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gyxspvyvz.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gamjilecv.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gvjimfbzs.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/glqoeqjzq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/gokrknlvo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/gmibtnyxf.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/galweytzb.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gagswdjhz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwejjggc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gyntlinek.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gsmqytaae.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/grgrdwyzs.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gfgfjuomu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/ginfvqlco.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gfglsbypj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/guhnbmdde.sHtML

[B09] break 与 continue
来源：http://blog.epnwcf.com/Article/details/gppgcsfua.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.sjlbkw.cn/Article/details/gqrhdcexu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gdicivttm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/goqzgqrow.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/garrdcapy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gjmxiryvv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gosgjvlht.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/gssizbmnf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/ggxkmrinj.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gqizjkwnm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/gumiwedaq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/gssykgnge.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gmltvjhxp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gfhljdqqb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.tarul.cn/Article/details/gnrtdvizo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.epnwcf.com/Article/details/gushcxufd.sHtML


<!-- 参考信息 -->