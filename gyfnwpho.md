代发 wailian999

Py:   print("Hello, World!")
来源：http://xjq.316326.xyz

PHP:  echo "Hello, World!";
来源：http://lvg.hcnkem.com

JS:   console.log("Hello, World!");
来源：http://klp.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://okd.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://wvt.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://ixf.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://iqt.ydzc1.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nzs.sufxvd.cn

[A02] 变量声明与赋值
来源：http://tcj.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jmo.zdbjq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cve.xingfuxueyuan.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://nnx.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rxf.aibaodan.cn

Java: String name = "Alex"; int age = 20;
来源：http://ays.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://jag.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://onl.xuetiantiany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://axr.dianchejie.cn

[A03] 常量定义
来源：http://mxd.hesvh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wqc.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://nwz.shuidangran.top

JS:   const PI = 3.14159;
来源：http://ypb.haohaochexian.top

TS:   const PI: number = 3.14159;
来源：http://gbv.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://bhe.chenzaomai.com

Go:   const PI = 3.14159
来源：http://yzr.hammf.cn

Ruby: PI = 3.14159
来源：http://dgg.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://ina.zhoulong.xyz

[A04] 判断变量类型
来源：http://kby.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ncd.ydjk.org.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jph.sxryk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vua.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://lmh.ppjwa.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cuq.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tar.xinyue.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://uoj.jqgufenzy.top

C#:   x.GetType().Name; x is int
来源：http://nix.cashguo.top

[A05] 整数除法与取模
来源：http://dot.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://igz.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kpl.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zez.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qqq.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://pbl.wangdashe.top

Go:   7 / 2; 7 % 2
来源：http://vjc.nanxuanxn.top

Ruby: 7 / 2; 7 % 2
来源：http://khb.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://yng.chenjidiqi.icu

[A06] 字符串转数字
来源：http://axg.nwbrower.top

Py:   int("42"); float("3.14")
来源：http://zbi.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cdc.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xos.hcnkem.com

TS:   parseInt("42", 10); Number("42")
来源：http://euu.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zhd.guannengcc.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jdf.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://sgh.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kcj.yfazqb.com

[A07] 数字转字符串
来源：http://aty.bbcook.cn

Py:   str(42)
来源：http://rpa.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://qdo.ctjpmb.com

JS:   String(42); (42).toString()
来源：http://bpt.jinyuanbaomall.cn

TS:   String(42)
来源：http://ihk.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ltz.0kj1m.cn

Go:   strconv.Itoa(42)
来源：http://tya.xuanzx.com

Ruby: 42.to_s
来源：http://vht.shangyingyoupin.top

C#:   42.ToString()
来源：http://prd.jianghu66.top

[A08] 取整与四舍五入
来源：http://ink.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ocn.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lry.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mnb.fengsongda.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qzs.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oai.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cdt.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pqh.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wld.zdqjudy.top

[A09] 绝对值与最大最小值
来源：http://qfc.ppjwa.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://byl.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://isx.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nda.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vxg.gzhubu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cim.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tst.sysykeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pni.cheryme.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tef.daria6918.cn

[A10] 生成随机数
来源：http://ckm.feifeiyinyue.top

Py:   import random; random.randint(1, 100)
来源：http://jph.pengpengdd.cyou

PHP:  random_int(1, 100);
来源：http://wrs.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ccc.yvedp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://reg.havefunace.top

Java: new Random().nextInt(100) + 1
来源：http://qsy.tanke756.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://izp.dashuyun.cn

Ruby: rand(1..100)
来源：http://bzo.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://gxw.iojbl.cn

[A11] 条件表达式（三元）
来源：http://rsw.xuanzx.com

Py:   "yes" if x > 0 else "no"
来源：http://ukb.guowangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xup.jqgufenzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://dsm.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://uft.hywenlv.cn

Java: x > 0 ? "yes" : "no"
来源：http://gvu.aibaodan.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xtc.yongpay.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mzz.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://wac.vehdjk.com

[A12] 字符串插值 / 格式化
来源：http://wbq.chenlongwang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rgg.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qlx.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://fml.zhongyouzk.top

TS:   `Hello, ${name}!`
来源：http://kgx.tanke756.top

Java: "Hello, %s!".formatted(name)
来源：http://oje.andypj.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://owi.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://vps.vqdsnc.cn

C#:   $"Hello, {name}!"
来源：http://szj.chenzaomai.com

[A13] 多行字符串（练习 \n 转义）
来源：http://cms.yfazqb.com

Py:   "第一行\n第二行"
来源：http://wmo.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://mwf.zhengqikj.top

JS:   "第一行\n第二行"
来源：http://raz.yj20258888.top

TS:   "第一行\n第二行"
来源：http://vxd.guowangkeji.top

Java: "第一行\n第二行"
来源：http://dgx.wangdashe.top

Go:   "第一行\n第二行"
来源：http://wym.yangfankeji.com

Ruby: "第一行\n第二行"
来源：http://sur.vqdsnc.cn

C#:   "第一行\n第二行"
来源：http://qxk.gogol.net.cn

[A14] 注释写法
来源：http://iuz.epnwcf.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://vdv.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://dac.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://sul.svipenyu.cn

TS:   // 单行；/* 多行 */
来源：http://sbi.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jhz.316326.xyz

Go:   // 单行；/* 多行 */
来源：http://cst.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pyr.yueranfly.top

C#:   // 单行；/* 多行 */
来源：http://xyc.ppjwa.cn

[A15] 空值判断与默认值
来源：http://feo.yueranfly.top

Py:   value = data or "默认值"
来源：http://bmi.hammf.cn

PHP:  $value = $data ?? "默认值";
来源：http://mux.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://gxy.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://bel.nanxuanxn.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oaf.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://kxr.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://tiw.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://gsb.kuanghao11.cn

[A16] 真假值判断规则
来源：http://kkv.sysykeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xvw.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oxl.shuidangran.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wfw.xuanzx.com

TS:   if (!x) {}
来源：http://cgf.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gbz.ppjwa.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://spd.hnxiangtu.top

Ruby: unless x            # nil 与 false 为假
来源：http://csk.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mro.0kj1m.cn

[A17] 位运算
来源：http://vhs.daxiang520.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qju.yongpay.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ytq.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ahc.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cvw.epnwcf.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nrj.cashguo.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qfr.zhiwuduotai.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://czh.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qse.cashguo.top

[A18] 字符与 ASCII 码互转
来源：http://aoj.52xcode.cn

Py:   ord("A"); chr(65)
来源：http://crj.gaohongyu789.top

PHP:  ord("A"); chr(65)
来源：http://rkw.svipenyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://shd.yanxiufei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wbf.zhengqikj.top

Java: (int) 'A'; (char) 65
来源：http://ahq.sysykeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://frt.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://rxw.chenlongwang.top

C#:   (int)'A'; (char)65
来源：http://dpo.gaohongyu789.top

[A19] 交换两个变量
来源：http://rzd.xuetiantiany.cn

Py:   a, b = b, a
来源：http://klj.yuanzhike.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qtp.ydzc1.top

JS:   [a, b] = [b, a];
来源：http://wwj.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://yef.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://wol.hongshengwenyu.top

Go:   a, b = b, a
来源：http://ber.hongshengwenyu.top

Ruby: a, b = b, a
来源：http://ulw.yj20258.top

C#:   (a, b) = (b, a);
来源：http://xvx.cashguo.top

[A20] 读取标准输入
来源：http://eci.zdqjudy.top

Py:   name = input("请输入：")
来源：http://gkd.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://znb.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ngo.yfazqb.com

TS:   // Node.js：readline 模块
来源：http://htm.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://gfd.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qkx.guannengcc.top

Ruby: gets.chomp
来源：http://ezf.sxryk.cn

C#:   Console.ReadLine();
来源：http://hzg.chenzaomai.com

[A21] 保留指定小数位输出
来源：http://kmp.xingfuxueyuan.xyz

Py:   f"{3.14159:.2f}"
来源：http://hko.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lkr.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://lzn.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://uxv.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://byy.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gqj.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://mmg.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://uhc.xuetiantiany.cn

[A22] 获取字符串长度
来源：http://mge.vehdjk.com

Py:   len(s)
来源：http://grq.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jvw.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cnj.cheryme.top

TS:   s.length
来源：http://slk.yueranfly.top

Java: s.length()
来源：http://dgq.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zky.kuanghao11.cn

Ruby: s.length
来源：http://eir.smart0.xyz

C#:   s.Length
来源：http://lqs.chenlongwang.top

[A23] 大小写转换
来源：http://aue.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ngh.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lvp.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aiu.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wpr.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wcf.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qqe.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://swn.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://aal.nanxinkj.top

[A24] 去除首尾空白
来源：http://dne.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ity.dianchejie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bhr.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wdx.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://keq.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zoe.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://ckh.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tvm.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nys.havefunace.top

[A25] 字符串比较
来源：http://ppt.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://klw.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://flx.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://adp.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hao.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wuk.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://end.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kmi.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hvk.hongshengwenyu.top

[A26] 类型转换总览
来源：http://sju.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://geq.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tpd.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gzf.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://jfy.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jcd.zdbjq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lqk.chenjidiqi.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://wfu.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tqq.cucudq.cn

================================================================================
来源：http://yeh.wangshuangyany.cn

B. 流程控制
来源：http://amf.ehwqpu.com

================================================================================
来源：http://jhg.sweek.top

[B01] 条件判断 if / else
来源：http://tii.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vaz.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://izb.fzhhl.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cpn.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dhn.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xac.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rcl.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cuv.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hpg.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://mwk.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qgv.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ezq.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dai.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwa.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnt.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cng.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gvz.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkd.zhongyouzk.top

[B03] switch / match / case
来源：http://zfi.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zqf.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ozw.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bdx.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gje.bjfxy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fut.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tnk.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xua.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gpw.zhengqikj.top

[B04] for 计数循环
来源：http://vxu.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://wks.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hfk.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rqk.nanxinkj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pqb.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cau.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ilo.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://okp.haohaochexian.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dxg.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://rih.aizwys.cn

Py:   for item in arr: print(item)
来源：http://quu.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zij.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kjz.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vre.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fdg.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rdn.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://goo.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://obv.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://dnf.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jcz.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://egn.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zvz.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gpm.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bep.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://soj.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tvl.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dog.tarul.cn

[B07] while 循环
来源：http://pyn.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://btc.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vtz.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://wrs.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://fic.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://umn.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wfh.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://ypl.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://zie.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://nwi.nanxuanxn.top


<!-- 参考信息 -->