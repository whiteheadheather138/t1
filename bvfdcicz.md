代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://znh.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://pby.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://bxb.9152youxi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gfc.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://hju.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ibh.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zyw.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://doh.fzhhl.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iyn.aibaodan.cn

Java: String name = "Alex"; int age = 20;
来源：http://nqf.xinyue.icu

Go:   name := "Alex"; age := 20
来源：http://chl.meibo888.top

Ruby: name = "Alex"; age = 20
来源：http://klk.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eao.tanke756.top

[A03] 常量定义
来源：http://gfa.cqqwz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tmw.316326.xyz

PHP:  const PI = 3.14159;
来源：http://gpz.zhengqikj.top

JS:   const PI = 3.14159;
来源：http://pbn.0kj1m.cn

TS:   const PI: number = 3.14159;
来源：http://vws.kuanghao11.cn

Java: static final double PI = 3.14159;
来源：http://ors.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://bhr.yvedp.cn

Ruby: PI = 3.14159
来源：http://dbn.xziqi.cn

C#:   const double PI = 3.14159;
来源：http://hjf.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://kbl.iojbl.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zgu.meibo888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lra.cdnleiting.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://htg.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://btz.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bqr.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vqz.bbcook.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qzx.zhijiandao.cn

C#:   x.GetType().Name; x is int
来源：http://mjn.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://ihh.feifeiyinyue.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://plz.ywan-chungtsiang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://yna.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://roy.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pjb.bbcook.cn

Java: 7 / 2; 7 % 2
来源：http://ght.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://jpz.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://mbe.kuanghao11.cn

C#:   7 / 2; 7 % 2
来源：http://qtn.yuxming.cn

[A06] 字符串转数字
来源：http://hhc.yangfankeji.com

Py:   int("42"); float("3.14")
来源：http://kky.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jeh.yangfankeji.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://znu.yj20258.top

TS:   parseInt("42", 10); Number("42")
来源：http://asb.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kjv.zhijiandao.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qnc.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rod.vehdjk.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oin.chenlongwang.top

[A07] 数字转字符串
来源：http://nic.c1oappe.top

Py:   str(42)
来源：http://jbx.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://uqf.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://chh.hnqzz.top

TS:   String(42)
来源：http://nml.sweek.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bzi.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://xck.hfpthk.cn

Ruby: 42.to_s
来源：http://dbo.316326.xyz

C#:   42.ToString()
来源：http://dxk.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://shd.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jwy.andypj.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wwz.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gkg.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rng.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://asx.nanxuanxn.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qth.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qht.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tre.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://rkv.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qeh.yj20258.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tii.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rus.bbcook.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xmw.fktsv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://czn.xuetiantiany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://igp.feifeiyinyue.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bms.hnxiangtu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hwj.zdqjudy.top

[A10] 生成随机数
来源：http://yoa.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://usv.gotoacloud.top

PHP:  random_int(1, 100);
来源：http://wes.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qvd.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://asy.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://xge.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://flx.yueranfly.top

Ruby: rand(1..100)
来源：http://dms.zhengqikj.top

C#:   new Random().Next(1, 101)
来源：http://nnp.jqgfzy.top

[A11] 条件表达式（三元）
来源：http://ubz.yvedp.cn

Py:   "yes" if x > 0 else "no"
来源：http://sha.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jka.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://jde.shanyushiyangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://avc.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://ffo.dashuyun.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://joy.shzxlz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lmr.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://cbo.sjlbkw.cn

[A12] 字符串插值 / 格式化
来源：http://fyy.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ypa.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lbz.ywan-chungtsiang.top

JS:   `Hello, ${name}!`
来源：http://rzx.cucudq.cn

TS:   `Hello, ${name}!`
来源：http://vev.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://ysj.xziqi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ymr.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://uya.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://mvd.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://bgw.yonumen.top

Py:   "第一行\n第二行"
来源：http://ozq.tarul.cn

PHP:  "第一行\n第二行"
来源：http://ufl.vehdjk.com

JS:   "第一行\n第二行"
来源：http://qtv.yonumen.top

TS:   "第一行\n第二行"
来源：http://mgr.svipenyu.cn

Java: "第一行\n第二行"
来源：http://uth.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://nyt.kuanghao11.cn

Ruby: "第一行\n第二行"
来源：http://ujz.hnqzz.top

C#:   "第一行\n第二行"
来源：http://qwz.jqgufenzy.top

[A14] 注释写法
来源：http://oiw.9152youxi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://opm.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yhk.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://frt.andypj.xyz

TS:   // 单行；/* 多行 */
来源：http://nbv.vqdsnc.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ybi.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://sqc.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://xoj.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://scz.jqgufenzy.top

[A15] 空值判断与默认值
来源：http://nwa.bjfxy.top

Py:   value = data or "默认值"
来源：http://kyv.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://gjt.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://tqr.yuxming.cn

TS:   const value = data ?? "默认值";
来源：http://vku.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nry.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://wwd.ydzc1.top

Ruby: value = data || "默认值"
来源：http://xzz.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://gqo.yvedp.cn

[A16] 真假值判断规则
来源：http://gsf.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iby.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cqs.sjlbkw.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rgy.gotoacloud.top

TS:   if (!x) {}
来源：http://wni.xingfuxueyuan.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kto.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lcc.tianlin.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://viu.yangfankeji.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xcx.zhongyouzk.top

[A17] 位运算
来源：http://roa.jiagoushi.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nwh.hammf.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fgf.nanxinkj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ydm.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wea.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcp.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kxg.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bqn.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oxw.ehwqpu.com

[A18] 字符与 ASCII 码互转
来源：http://fju.fehbvm.com

Py:   ord("A"); chr(65)
来源：http://rvi.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://uap.jlsjyb.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mjx.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aln.wangdashe.top

Java: (int) 'A'; (char) 65
来源：http://waj.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xcr.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://cvv.pycfn.com

C#:   (int)'A'; (char)65
来源：http://oli.tian-w.cn

[A19] 交换两个变量
来源：http://aqp.yj20258888.top

Py:   a, b = b, a
来源：http://gyr.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xac.xingfuxueyuan.xyz

JS:   [a, b] = [b, a];
来源：http://xgb.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://fnf.ctjpmb.com

Java: int t = a; a = b; b = t;
来源：http://djj.bjfxy.top

Go:   a, b = b, a
来源：http://nrr.jqgufenzy.top

Ruby: a, b = b, a
来源：http://cjj.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://zlb.yfazqb.com

[A20] 读取标准输入
来源：http://dsh.cashguo.top

Py:   name = input("请输入：")
来源：http://qfw.ybcxt.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fnc.316326.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nsf.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://fpd.zhengqikj.top

Java: new Scanner(System.in).nextLine()
来源：http://ida.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ssc.guannengcc.top

Ruby: gets.chomp
来源：http://muw.yangfankeji.com

C#:   Console.ReadLine();
来源：http://udw.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://zyc.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://qpg.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eev.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://sfk.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://dwp.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://jsz.52xcode.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jba.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://grv.svipenyu.cn

C#:   3.14159.ToString("F2")
来源：http://nwy.xuetiantiany.cn

[A22] 获取字符串长度
来源：http://ary.yuxming.cn

Py:   len(s)
来源：http://adl.9152youxi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bqn.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tsv.xingfuxueyuan.xyz

TS:   s.length
来源：http://qmi.tarul.cn

Java: s.length()
来源：http://btw.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gpc.dianchejie.cn

Ruby: s.length
来源：http://kvb.epnwcf.com

C#:   s.Length
来源：http://amr.xuanzx.com

[A23] 大小写转换
来源：http://bxn.fehbvm.com

Py:   s.upper(); s.lower(); s.title()
来源：http://xip.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nfw.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ptr.wangdashe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rcr.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://umn.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pgp.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://scz.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nev.tianlin.xyz

[A24] 去除首尾空白
来源：http://dot.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ayj.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rwv.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sot.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cmf.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hzr.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://isb.jiagoushi.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://obh.shzxlz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zac.xinyue.icu

[A25] 字符串比较
来源：http://igv.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://xsy.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://owi.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgr.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bty.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tkn.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kci.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://inn.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sny.nwbrower.top

[A26] 类型转换总览
来源：http://juo.gogol.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ent.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fqq.zhixingplan.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ffs.yfazqb.com

TS:   Number() String() Boolean() x as number
来源：http://fen.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://imh.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hld.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ekl.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bel.guannengcc.top

================================================================================
来源：http://rvb.chenlongwang.top

B. 流程控制
来源：http://hms.shzxlz.cn

================================================================================
来源：http://ydv.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://nld.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://drn.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pnh.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sya.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://euk.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yuc.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rqm.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aor.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kdx.pycfn.com

[B02] 多分支 else if / elif
来源：http://vtw.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cah.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://myz.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aun.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qjl.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqz.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fdo.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zla.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ige.chenzaomai.com

[B03] switch / match / case
来源：http://tpm.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wwf.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://moo.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ymd.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rob.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kdw.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iur.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bpa.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uii.ywan-chungtsiang.top

[B04] for 计数循环
来源：http://jji.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://izu.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yzv.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://edp.xuetiantiany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zod.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lvj.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xli.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://tni.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dcr.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://ofd.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://ceu.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pyp.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zuu.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vuk.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fot.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://imb.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://igb.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nuu.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://ixl.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yst.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hwu.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dja.guowangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vub.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqe.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sal.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fco.yuanzhike.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rmg.pycfn.com

[B07] while 循环
来源：http://xtw.daria6918.cn

Py:   while i < 10: i += 1
来源：http://dbw.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://goz.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://xgx.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://zjb.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://bqo.ivvv.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qdq.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://slj.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://xad.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://ijt.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://ilh.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tag.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://jfe.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://fqo.xuetiantiany.cn


<!-- 参考信息 -->