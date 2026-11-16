代发 wailian999

[A02] 变量声明与赋值
来源：http://vxl.zhiwuduotai.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://quz.yangfankeji.com

PHP:  $name = "Alex"; $age = 20;
来源：http://gvh.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hcm.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xse.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://ksf.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://fbf.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://khw.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wcn.mhx1999.top

[A03] 常量定义
来源：http://zkq.chenjidiqi.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ium.yongpay.top

PHP:  const PI = 3.14159;
来源：http://thw.fengsongda.top

JS:   const PI = 3.14159;
来源：http://msc.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://luj.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://lfb.havefunace.top

Go:   const PI = 3.14159
来源：http://lfk.smart0.xyz

Ruby: PI = 3.14159
来源：http://qnq.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://mbr.birdmap.top

[A04] 判断变量类型
来源：http://lsz.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sxr.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nuz.bbcook.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ail.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://ter.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zpw.pengpengdd.cyou

Go:   reflect.TypeOf(x).Name()
来源：http://dpo.redwolf501.top

Ruby: x.class; x.is_a?(Integer)
来源：http://iry.yuxming.cn

C#:   x.GetType().Name; x is int
来源：http://rbd.yvedp.cn

[A05] 整数除法与取模
来源：http://nij.xziqi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jud.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mhp.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nuy.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ulr.zhaomingkeji.xyz

Java: 7 / 2; 7 % 2
来源：http://cor.ehwqpu.com

Go:   7 / 2; 7 % 2
来源：http://uxq.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://rps.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://phe.bjfxy.top

[A06] 字符串转数字
来源：http://snl.cashguo.top

Py:   int("42"); float("3.14")
来源：http://kzv.xziqi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jvs.nanxuanxn.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://var.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://pvz.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://khz.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://diz.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://una.snrcjt.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xpw.chenzaomai.com

[A07] 数字转字符串
来源：http://kup.ehwqpu.com

Py:   str(42)
来源：http://qql.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://vtm.316326.xyz

JS:   String(42); (42).toString()
来源：http://igg.chenlongwang.top

TS:   String(42)
来源：http://abw.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wao.jinqigufen.top

Go:   strconv.Itoa(42)
来源：http://lwy.svipenyu.cn

Ruby: 42.to_s
来源：http://iyk.kuanghao11.cn

C#:   42.ToString()
来源：http://ljm.jiagoushi.top

[A08] 取整与四舍五入
来源：http://hnd.xuanzx.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hzt.birdmap.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oii.yueranfly.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://goe.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bvg.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wnd.gotoacloud.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kyr.yj20258888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hqr.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vuz.ydzc1.top

[A09] 绝对值与最大最小值
来源：http://ltg.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wvf.jianghu66.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uwk.ctjpmb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blu.dashuyun.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cid.chenzaomai.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rjr.yvedp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xnl.daria6918.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mvt.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yxt.tian-w.cn

[A10] 生成随机数
来源：http://rar.dianchejie.cn

Py:   import random; random.randint(1, 100)
来源：http://mae.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://uli.pengpengdd.cyou

JS:   Math.floor(Math.random() * 100) + 1
来源：http://coy.fanxiaobao.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://icv.bbcook.cn

Java: new Random().nextInt(100) + 1
来源：http://wte.sufxvd.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wju.yuxming.cn

Ruby: rand(1..100)
来源：http://yby.bbcook.cn

C#:   new Random().Next(1, 101)
来源：http://bnf.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://zrk.c1oappe.top

Py:   "yes" if x > 0 else "no"
来源：http://jwt.gogol.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dcx.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xqx.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://tfc.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://drd.kuanghao11.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lrt.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://zdq.yj202588.top

C#:   x > 0 ? "yes" : "no"
来源：http://iul.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://bgh.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://byi.hongshengwenyu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hxp.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://pbh.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://yja.ydjk.org.cn

Java: "Hello, %s!".formatted(name)
来源：http://icw.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mpr.ydjk.org.cn

Ruby: "Hello, #{name}!"
来源：http://vhx.hcnkem.com

C#:   $"Hello, {name}!"
来源：http://twi.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ggx.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://soy.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://bbr.xingfuxueyuan.xyz

JS:   "第一行\n第二行"
来源：http://tmw.epnwcf.com

TS:   "第一行\n第二行"
来源：http://lls.hammf.cn

Java: "第一行\n第二行"
来源：http://wky.andypj.xyz

Go:   "第一行\n第二行"
来源：http://fes.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://kpb.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://kyt.9152youxi.cn

[A14] 注释写法
来源：http://yqy.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://ttq.ydjk.org.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://blz.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://nml.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://kpm.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sxb.epnwcf.com

Go:   // 单行；/* 多行 */
来源：http://qsg.xziqi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ufp.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://iwy.tarul.cn

[A15] 空值判断与默认值
来源：http://rna.gzhubu.top

Py:   value = data or "默认值"
来源：http://nic.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://mxf.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://hhb.cheryme.top

TS:   const value = data ?? "默认值";
来源：http://xwc.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xbo.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://nvo.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://gbb.iojbl.cn

C#:   var value = data ?? "默认值";
来源：http://lls.0kj1m.cn

[A16] 真假值判断规则
来源：http://lrx.svipenyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ecx.meibo888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://abc.zhaomingkeji.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tzv.hammf.cn

TS:   if (!x) {}
来源：http://rgy.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ujj.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tlg.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://vlt.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vlt.xuanzx.com

[A17] 位运算
来源：http://xpr.c1oappe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ekw.zhijiandao.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wls.yongpay.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axe.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pvf.dianchejie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dvs.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tgs.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfh.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://thf.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://gyh.316326.xyz

Py:   ord("A"); chr(65)
来源：http://yda.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://evz.xinyue.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yqf.birdmap.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nkg.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://drh.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wde.birdmap.top

Ruby: "A".ord; 65.chr
来源：http://jdy.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://ogt.zhongyouzk.top

[A19] 交换两个变量
来源：http://mhx.ywan-chungtsiang.top

Py:   a, b = b, a
来源：http://leh.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://xkw.cqqwz.cn

JS:   [a, b] = [b, a];
来源：http://kfi.jinqigfzy.top

TS:   [a, b] = [b, a];
来源：http://pbk.vehdjk.com

Java: int t = a; a = b; b = t;
来源：http://epi.xuetiantiany.cn

Go:   a, b = b, a
来源：http://coj.aizwys.cn

Ruby: a, b = b, a
来源：http://pyr.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://wrb.ydjk.org.cn

[A20] 读取标准输入
来源：http://thr.gotoacloud.top

Py:   name = input("请输入：")
来源：http://oph.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yzb.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mzp.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://qhh.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://but.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ohj.xuetiantiany.cn

Ruby: gets.chomp
来源：http://agb.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://fnj.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://zbh.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://kyx.birdmap.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wnz.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://rvy.zhengqikj.top

TS:   (3.14159).toFixed(2)
来源：http://vck.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://ape.sweek.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gip.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://ylc.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://wns.zhengqikj.top

[A22] 获取字符串长度
来源：http://drf.xziqi.cn

Py:   len(s)
来源：http://fht.zycfv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dcb.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dec.pycfn.com

TS:   s.length
来源：http://efp.yuxming.cn

Java: s.length()
来源：http://upo.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tjy.snrcjt.cn

Ruby: s.length
来源：http://jwo.zdbjq.cn

C#:   s.Length
来源：http://tkg.cdnleiting.top

[A23] 大小写转换
来源：http://ndt.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://opg.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zis.vqdsnc.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ygj.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bav.nanxuanxn.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fvh.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://glt.mhx1999.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yyt.iojbl.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rpm.0kj1m.cn

[A24] 去除首尾空白
来源：http://xxo.zycfv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jez.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ufe.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uhd.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shn.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rve.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://eff.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cvx.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hpy.uphjek.com

[A25] 字符串比较
来源：http://lbs.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://hdb.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wci.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ukl.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fte.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tya.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://djz.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vak.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fag.zhijiandao.cn

[A26] 类型转换总览
来源：http://xvv.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ldy.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ogd.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ase.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://fui.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zjz.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rax.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kyv.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xao.redwolf501.top

================================================================================
来源：http://zws.jinyuanbaomall.cn

B. 流程控制
来源：http://qin.chenlongwang.top

================================================================================
来源：http://aqf.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://dvm.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oga.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zam.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fnu.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yvf.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iee.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jmo.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jqm.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cll.cashguo.top

[B02] 多分支 else if / elif
来源：http://xqs.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tcf.fzhhl.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pjp.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpn.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://svv.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nln.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nyb.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pab.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ean.iojbl.cn

[B03] switch / match / case
来源：http://rmj.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nld.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pwl.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jhs.chenzaomai.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://axn.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://svj.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hpg.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blh.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nqr.zhoulong.xyz

[B04] for 计数循环
来源：http://qus.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://pnn.52xcode.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://klf.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tkd.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xqn.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vbo.xuanzx.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://icj.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://rss.xziqi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jot.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://ktx.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://fxz.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://njh.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://txd.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bum.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kvb.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fmn.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://ukt.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wxy.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://ewn.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://aka.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lqf.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kxk.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ggh.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jwy.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://flp.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rjt.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eqp.zhijiandao.cn

[B07] while 循环
来源：http://ffj.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://rzg.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://oyo.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://djb.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://vik.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://kfo.snrcjt.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lgb.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://xkr.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://fys.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://thb.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://nfv.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://czh.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://wkh.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://mrl.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://mft.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cjq.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oaq.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://glp.aibaodan.cn


<!-- 参考信息 -->