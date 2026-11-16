代发 wailian999

================================================================================
来源：http://who.9152youxi.cn

A. 基础语法与类型
来源：http://qzd.jianghu66.top

================================================================================
来源：http://rgz.sweek.top

[A01] Hello World
来源：http://txr.daxiang520.top

Py:   print("Hello, World!")
来源：http://koa.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://dgy.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://hiy.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rxq.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://pbg.shanyushiyangtech.top

Go:   fmt.Println("Hello, World!")
来源：http://dtu.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://teu.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wip.pycfn.com

[A02] 变量声明与赋值
来源：http://lsl.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fsx.zhoulong.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://kbw.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://qre.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sln.shuidangran.top

Java: String name = "Alex"; int age = 20;
来源：http://quh.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://fpr.gzhubu.top

Ruby: name = "Alex"; age = 20
来源：http://xgl.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hkz.andypj.xyz

[A03] 常量定义
来源：http://mqp.chenjidiqi.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://noe.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://nsz.yuxming.cn

JS:   const PI = 3.14159;
来源：http://jhh.xziqi.cn

TS:   const PI: number = 3.14159;
来源：http://lpf.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://xbz.fzhhl.top

Go:   const PI = 3.14159
来源：http://feb.pengpengdd.cyou

Ruby: PI = 3.14159
来源：http://ozh.0kj1m.cn

C#:   const double PI = 3.14159;
来源：http://xxr.yonumen.top

[A04] 判断变量类型
来源：http://imt.epnwcf.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://dcg.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ebg.aibaodan.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qqr.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://tos.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kjo.nanxinkj.top

Go:   reflect.TypeOf(x).Name()
来源：http://ttw.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dop.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://wne.xingfuxueyuan.xyz

[A05] 整数除法与取模
来源：http://cmx.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ube.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://skt.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bma.epnwcf.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mvn.meibo888.top

Java: 7 / 2; 7 % 2
来源：http://vwl.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://gsp.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://ers.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://ysz.meibo888.top

[A06] 字符串转数字
来源：http://llo.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://jcc.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ovo.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bob.shangyingyoupin.top

TS:   parseInt("42", 10); Number("42")
来源：http://lqa.pengpengdd.cyou

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jyk.zhiwuduotai.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sas.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jfh.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://brf.9152youxi.cn

[A07] 数字转字符串
来源：http://pah.jyoumei.cn

Py:   str(42)
来源：http://frv.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://fif.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://miw.tanke756.top

TS:   String(42)
来源：http://vot.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pfa.ehwqpu.com

Go:   strconv.Itoa(42)
来源：http://pbx.snrcjt.cn

Ruby: 42.to_s
来源：http://zfs.guannengcc.top

C#:   42.ToString()
来源：http://hqs.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://eng.jinyuanbaomall.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wez.aizwys.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ihd.tanke756.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vhw.jqgfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jab.guowangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dcw.hnqzz.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qpk.yueranfly.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xhh.ivvv.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qya.ydzc1.top

[A09] 绝对值与最大最小值
来源：http://lue.vqdsnc.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ajq.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hev.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uix.svipenyu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cuk.nanxinkj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lmx.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mas.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://onm.yvedp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://llx.hywenlv.cn

[A10] 生成随机数
来源：http://svk.dianchejie.cn

Py:   import random; random.randint(1, 100)
来源：http://zmn.zhaomingkeji.xyz

PHP:  random_int(1, 100);
来源：http://ytx.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://spo.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://twc.redwolf501.top

Java: new Random().nextInt(100) + 1
来源：http://brj.tanke756.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dyd.zhaomingkeji.xyz

Ruby: rand(1..100)
来源：http://wdd.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://qlu.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://gpa.cashguo.top

Py:   "yes" if x > 0 else "no"
来源：http://waw.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://aha.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kvd.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://fxm.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://ylp.jianghu66.top

Go:   // 无三元运算符，需用 if 语句
来源：http://utw.quarkkingdee.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vdj.yfazqb.com

C#:   x > 0 ? "yes" : "no"
来源：http://qau.nanxinkj.top

[A12] 字符串插值 / 格式化
来源：http://cud.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eef.yvedp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qht.zhongyouzk.top

JS:   `Hello, ${name}!`
来源：http://gpj.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://vso.cashguo.top

Java: "Hello, %s!".formatted(name)
来源：http://toi.cheryme.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yfv.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://ywn.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://ulu.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://mho.ybcxt.top

Py:   "第一行\n第二行"
来源：http://bzs.ywan-chungtsiang.top

PHP:  "第一行\n第二行"
来源：http://uqj.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://hdq.bbcook.cn

TS:   "第一行\n第二行"
来源：http://uqo.tian-w.cn

Java: "第一行\n第二行"
来源：http://rdt.hesvh.cn

Go:   "第一行\n第二行"
来源：http://ulj.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://jsn.xylfe.cn

C#:   "第一行\n第二行"
来源：http://xja.ctjpmb.com

[A14] 注释写法
来源：http://ptn.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zgb.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ikh.yuanzhike.top

JS:   // 单行；/* 多行 */
来源：http://ocb.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://kcw.iojbl.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mlj.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://sve.shuidangran.top

Ruby: # 单行；=begin 多行 =end
来源：http://wtb.jinqigfzy.top

C#:   // 单行；/* 多行 */
来源：http://uzd.guowangkeji.top

[A15] 空值判断与默认值
来源：http://xvc.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://wmb.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://anq.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://vzm.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://sgv.yfazqb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fyk.ydjk.org.cn

Go:   if data == "" { data = "默认值" }
来源：http://hdp.andypj.xyz

Ruby: value = data || "默认值"
来源：http://kid.dianchejie.cn

C#:   var value = data ?? "默认值";
来源：http://rqx.gotoacloud.top

[A16] 真假值判断规则
来源：http://jtx.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rwx.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mgg.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pqi.zdbjq.cn

TS:   if (!x) {}
来源：http://mvk.fengsongda.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://khv.316326.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://agm.tianlin.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://oap.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fnp.hongshengwenyu.top

[A17] 位运算
来源：http://xat.ydzc1.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://klr.xylfe.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://csk.yonumen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gmg.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dyr.guowangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cbp.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kxy.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ndu.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uod.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://puk.guannengcc.top

Py:   ord("A"); chr(65)
来源：http://ebu.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://gsa.nwbrower.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dqg.wangdashe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yzg.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://uyl.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://trd.shanyushiyangkeji.top

Ruby: "A".ord; 65.chr
来源：http://oab.shuidangran.top

C#:   (int)'A'; (char)65
来源：http://ito.jqgfzy.top

[A19] 交换两个变量
来源：http://gdu.yangfankeji.com

Py:   a, b = b, a
来源：http://tbx.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://vdm.zhoulong.xyz

JS:   [a, b] = [b, a];
来源：http://pru.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://ute.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://lms.shzxlz.cn

Go:   a, b = b, a
来源：http://cde.tarul.cn

Ruby: a, b = b, a
来源：http://pcf.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://vsd.fktsv.cn

[A20] 读取标准输入
来源：http://tcj.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://kke.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ukc.yuanzhike.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://thy.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://tdp.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://nwx.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://emp.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://wba.cashguo.top

C#:   Console.ReadLine();
来源：http://znw.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://iwd.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://xba.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ogi.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://brc.svipenyu.cn

TS:   (3.14159).toFixed(2)
来源：http://uvy.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://ozr.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iba.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://rzp.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://jjf.cdnleiting.top

[A22] 获取字符串长度
来源：http://vfo.xuanzx.com

Py:   len(s)
来源：http://kpo.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://psf.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://doy.iojbl.cn

TS:   s.length
来源：http://wrz.ivvv.top

Java: s.length()
来源：http://ugp.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xoo.0kj1m.cn

Ruby: s.length
来源：http://zsq.zhaomingkeji.xyz

C#:   s.Length
来源：http://btm.shanyushiyangtech.top

[A23] 大小写转换
来源：http://pqd.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kpa.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://frf.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yxu.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mhe.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lkf.hnqzz.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vga.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vjp.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qke.shzxlz.cn

[A24] 去除首尾空白
来源：http://clb.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xdr.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aof.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vvk.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dfz.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ogj.epnwcf.com

Go:   strings.TrimSpace(s)
来源：http://mux.haohaochexian.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://esz.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hdn.bbcook.cn

[A25] 字符串比较
来源：http://kwi.yuanzhike.top

Py:   s1 == s2; s1 != s2
来源：http://thz.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lwr.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rkw.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://abx.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eir.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mci.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ogx.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aqg.jyoumei.cn

[A26] 类型转换总览
来源：http://vsy.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bhm.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rpk.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rqj.sufxvd.cn

TS:   Number() String() Boolean() x as number
来源：http://uxo.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ywg.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://brf.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jvk.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wqx.yfazqb.com

================================================================================
来源：http://pyi.zhaomingkeji.xyz

B. 流程控制
来源：http://sxu.jianghu66.top

================================================================================
来源：http://pmc.ehwqpu.com

[B01] 条件判断 if / else
来源：http://uad.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mos.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lhi.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lcx.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gil.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xpp.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tqq.redwolf501.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iud.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dsv.yuxming.cn

[B02] 多分支 else if / elif
来源：http://xrc.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xgq.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gaa.daxiang520.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqy.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppb.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tju.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pdp.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dag.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqv.shangyingyoupin.top

[B03] switch / match / case
来源：http://tzv.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nds.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xyv.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://stm.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zst.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ovj.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jxb.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://etu.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jfq.wangdashe.top

[B04] for 计数循环
来源：http://aid.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://zcp.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sge.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zuy.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zza.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eqg.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yvt.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://dce.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zzq.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://yhq.kuanghao11.cn

Py:   for item in arr: print(item)
来源：http://ank.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hsi.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cti.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mgh.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vdi.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xfp.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://rqs.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jos.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://nuc.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://plk.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gpr.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zyd.jinyuanbaomall.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://trg.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gid.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zbb.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fuw.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kej.ehwqpu.com

[B07] while 循环
来源：http://cen.uphjek.com

Py:   while i < 10: i += 1
来源：http://sxs.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://siv.cashguo.top

JS:   while (i < 10) { i++; }
来源：http://upb.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://mvr.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://eyo.ydjk.org.cn


<!-- 参考信息 -->