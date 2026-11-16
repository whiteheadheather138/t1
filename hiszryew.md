代发 wailian999

================================================================================
来源：http://qdt.sjlbkw.cn

A. 基础语法与类型
来源：http://uic.dashuyun.cn

================================================================================
来源：http://zlg.yanxiufei.cn

[A01] Hello World
来源：http://wqj.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://cgs.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://vqd.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://fyk.yuxming.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ymt.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://ujw.fengsongda.top

Go:   fmt.Println("Hello, World!")
来源：http://kkt.andypj.xyz

Ruby: puts "Hello, World!"
来源：http://xeg.guowangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zpp.jinyuanbaomall.cn

[A02] 变量声明与赋值
来源：http://gcy.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ohr.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yvj.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://bva.sjlbkw.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ndi.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://via.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://tmf.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://uez.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ulv.cqqwz.cn

[A03] 常量定义
来源：http://jwy.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ekf.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://vqq.aizwys.cn

JS:   const PI = 3.14159;
来源：http://ojd.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://dpz.xziqi.cn

Java: static final double PI = 3.14159;
来源：http://ocb.ybcxt.top

Go:   const PI = 3.14159
来源：http://edj.0kj1m.cn

Ruby: PI = 3.14159
来源：http://sep.jqgfzy.top

C#:   const double PI = 3.14159;
来源：http://aam.yj20258888.top

[A04] 判断变量类型
来源：http://xyi.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dha.yj20258888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mgy.ehwqpu.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zcb.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://bpo.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://npo.ehwqpu.com

Go:   reflect.TypeOf(x).Name()
来源：http://bfi.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://nwj.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://osi.sxryk.cn

[A05] 整数除法与取模
来源：http://jvy.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dsq.jinyuanbaomall.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vqj.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://our.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ipj.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://khs.zhoulong.xyz

Go:   7 / 2; 7 % 2
来源：http://iin.hongshengwenyu.top

Ruby: 7 / 2; 7 % 2
来源：http://dcd.bjfxy.top

C#:   7 / 2; 7 % 2
来源：http://img.nwbrower.top

[A06] 字符串转数字
来源：http://uto.epnwcf.com

Py:   int("42"); float("3.14")
来源：http://uxz.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://unj.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fsg.zhaomingkeji.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://wpn.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fra.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://akf.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://tsd.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ynx.shzxlz.cn

[A07] 数字转字符串
来源：http://bha.yuxming.cn

Py:   str(42)
来源：http://htj.chenjidiqi.icu

PHP:  (string) 42; strval(42)
来源：http://pxd.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://yum.bbcook.cn

TS:   String(42)
来源：http://cdm.birdmap.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mlj.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://qas.ybcxt.top

Ruby: 42.to_s
来源：http://xdw.ydjk.org.cn

C#:   42.ToString()
来源：http://tbi.hcnkem.com

[A08] 取整与四舍五入
来源：http://zvk.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zau.cashguo.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mle.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oou.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bgz.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gxv.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://plb.xziqi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mrl.hongshengwenyu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ijf.cheryme.top

[A09] 绝对值与最大最小值
来源：http://kja.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kfe.shzxlz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hrg.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lwz.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://thv.zhiwuduotai.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ols.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eya.daria6918.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sht.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vhr.0kj1m.cn

[A10] 生成随机数
来源：http://wie.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://nlo.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://iho.jinghuilouyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oim.dianchejie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vig.hnxiangtu.top

Java: new Random().nextInt(100) + 1
来源：http://jbx.0kj1m.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://amz.zdqjudy.top

Ruby: rand(1..100)
来源：http://csk.c1oappe.top

C#:   new Random().Next(1, 101)
来源：http://fen.zhiwuduotai.top

[A11] 条件表达式（三元）
来源：http://udj.tarul.cn

Py:   "yes" if x > 0 else "no"
来源：http://oux.redwolf501.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zju.hongshengwenyu.top

JS:   x > 0 ? "yes" : "no"
来源：http://oya.quarkkingdee.top

TS:   x > 0 ? "yes" : "no"
来源：http://bdg.sxryk.cn

Java: x > 0 ? "yes" : "no"
来源：http://giv.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nvx.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zqu.daria6918.cn

C#:   x > 0 ? "yes" : "no"
来源：http://aml.yuanzhike.top

[A12] 字符串插值 / 格式化
来源：http://phg.ctjpmb.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ivo.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uim.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://tlx.dashuyun.cn

TS:   `Hello, ${name}!`
来源：http://oly.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://met.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wsx.ydjk.org.cn

Ruby: "Hello, #{name}!"
来源：http://uel.fengsongda.top

C#:   $"Hello, {name}!"
来源：http://tjx.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iwc.jqgfzy.top

Py:   "第一行\n第二行"
来源：http://qyt.gaohongyu789.top

PHP:  "第一行\n第二行"
来源：http://cgo.snrcjt.cn

JS:   "第一行\n第二行"
来源：http://cam.yuxming.cn

TS:   "第一行\n第二行"
来源：http://csp.cqqwz.cn

Java: "第一行\n第二行"
来源：http://acl.yj20258.top

Go:   "第一行\n第二行"
来源：http://fpy.meibo888.top

Ruby: "第一行\n第二行"
来源：http://svr.ctjpmb.com

C#:   "第一行\n第二行"
来源：http://gwj.snrcjt.cn

[A14] 注释写法
来源：http://bkd.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ind.xingfuxueyuan.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://itd.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://yjr.c1oappe.top

TS:   // 单行；/* 多行 */
来源：http://xih.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kib.ydzc1.top

Go:   // 单行；/* 多行 */
来源：http://cmi.guannengcc.top

Ruby: # 单行；=begin 多行 =end
来源：http://bwz.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://fes.chenlongwang.top

[A15] 空值判断与默认值
来源：http://jot.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://eeu.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://fls.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://pbj.yongpay.top

TS:   const value = data ?? "默认值";
来源：http://qcn.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eps.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://wlu.yfazqb.com

Ruby: value = data || "默认值"
来源：http://myj.andypj.xyz

C#:   var value = data ?? "默认值";
来源：http://jlz.hnxiangtu.top

[A16] 真假值判断规则
来源：http://lgn.52xcode.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ovx.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ddn.gzhubu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hre.ivvv.top

TS:   if (!x) {}
来源：http://req.shuidangran.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cgv.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dbh.ehwqpu.com

Ruby: unless x            # nil 与 false 为假
来源：http://mpf.chenzaomai.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wue.zhaomingkeji.xyz

[A17] 位运算
来源：http://fdt.jinghuilouyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iff.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://thy.nanxuanxn.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zrw.wangshuangyany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hrq.yj20258888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovh.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eqo.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eaa.aibaodan.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ivr.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://voi.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://qlc.zycfv.cn

PHP:  ord("A"); chr(65)
来源：http://fos.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ffg.c1oappe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xev.jqgfzy.top

Java: (int) 'A'; (char) 65
来源：http://hfj.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://adh.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://arb.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://mha.feifeiyinyue.top

[A19] 交换两个变量
来源：http://dsr.52xcode.cn

Py:   a, b = b, a
来源：http://tcu.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ubp.guannengcc.top

JS:   [a, b] = [b, a];
来源：http://rgp.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://jdv.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://xlm.ybcxt.top

Go:   a, b = b, a
来源：http://rpe.epnwcf.com

Ruby: a, b = b, a
来源：http://ker.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://cgb.xziqi.cn

[A20] 读取标准输入
来源：http://toj.tanke756.top

Py:   name = input("请输入：")
来源：http://kjq.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://yvi.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cez.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://dhp.yongpay.top

Java: new Scanner(System.in).nextLine()
来源：http://ilw.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fwv.yj20258.top

Ruby: gets.chomp
来源：http://ulo.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://seq.tarul.cn

[A21] 保留指定小数位输出
来源：http://ecs.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://akt.xinyue.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aop.52xcode.cn

JS:   (3.14159).toFixed(2)
来源：http://dmy.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://vwx.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://qbp.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wji.haohaochexian.top

Ruby: format("%.2f", 3.14159)
来源：http://ymi.hongshengwenyu.top

C#:   3.14159.ToString("F2")
来源：http://zis.0kj1m.cn

[A22] 获取字符串长度
来源：http://fgl.aibaodan.cn

Py:   len(s)
来源：http://tke.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wve.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dfp.nanxuanxn.top

TS:   s.length
来源：http://vmg.fehbvm.com

Java: s.length()
来源：http://gqi.jinqigfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mon.zhoulong.xyz

Ruby: s.length
来源：http://dbe.jyoumei.cn

C#:   s.Length
来源：http://xkc.shangyingyoupin.top

[A23] 大小写转换
来源：http://vrj.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tnz.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lma.chenjidiqi.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aun.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mfo.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://knd.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xbl.yanxiufei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://snt.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gtm.chenzaomai.com

[A24] 去除首尾空白
来源：http://djn.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wrd.jqgfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://isv.bjfxy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ftn.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ljv.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zxr.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://bgv.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xbu.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nmj.yuxming.cn

[A25] 字符串比较
来源：http://uwa.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://mqk.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ulk.tianlin.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nqz.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://boc.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ybi.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://osf.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uia.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oby.jqgfzy.top

[A26] 类型转换总览
来源：http://jct.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mwd.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mpu.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ndb.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://cng.uphjek.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yct.nwbrower.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ajb.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ocl.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uqz.svipenyu.cn

================================================================================
来源：http://dpj.xuanzx.com

B. 流程控制
来源：http://csc.sxryk.cn

================================================================================
来源：http://wed.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://sys.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gsq.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xts.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uon.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://itr.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uof.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ujp.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wmi.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xoj.xziqi.cn

[B02] 多分支 else if / elif
来源：http://njw.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sef.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://snk.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fgt.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qif.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eoq.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xhr.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rdb.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwv.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://yrj.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ooc.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wuk.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cgb.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kbu.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ymi.jqgfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dzh.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jfp.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zpc.zhoulong.xyz

[B04] for 计数循环
来源：http://rqm.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://bwv.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aes.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://frv.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgn.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vlu.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jmy.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://xuc.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qtx.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://ylk.hesvh.cn

Py:   for item in arr: print(item)
来源：http://ysd.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ktb.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ybt.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ayf.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://bsq.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zhz.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://uwt.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iie.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://dnw.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rgl.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hxn.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nzn.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mud.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vvx.guowangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oqk.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tai.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hzr.0kj1m.cn

[B07] while 循环
来源：http://sin.ybcxt.top

Py:   while i < 10: i += 1
来源：http://ryf.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gxe.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://uzl.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://rto.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://vwq.hcnkem.com


<!-- 参考信息 -->