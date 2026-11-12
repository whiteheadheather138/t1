代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://kaz.feifeiyinyue.top

[A03] 常量定义
来源：http://wmi.chenlongwang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ddx.snrcjt.cn

PHP:  const PI = 3.14159;
来源：http://lbl.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://jht.fzhhl.top

TS:   const PI: number = 3.14159;
来源：http://gpz.yj202588.top

Java: static final double PI = 3.14159;
来源：http://vop.shuidangran.top

Go:   const PI = 3.14159
来源：http://xnb.xuanzx.com

Ruby: PI = 3.14159
来源：http://wqd.hcnkem.com

C#:   const double PI = 3.14159;
来源：http://kje.fanxiaobao.xyz

[A04] 判断变量类型
来源：http://npd.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rdg.yanxiufei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wsx.hcnkem.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pgk.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://apo.cqqwz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ggi.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://vwv.ctjpmb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://xwu.shzxlz.cn

C#:   x.GetType().Name; x is int
来源：http://vrq.gaohongyu789.top

[A05] 整数除法与取模
来源：http://hvm.hysaishi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cwr.shuidangran.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fyg.zhengqikj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dfo.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lfw.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://jfk.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://lyz.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://rmj.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://bhg.birdmap.top

[A06] 字符串转数字
来源：http://kud.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://ljx.chenlongwang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mcu.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://riz.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://cpy.nanxuanxn.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://shf.fktsv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ezv.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nig.yuanzhike.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ixu.0kj1m.cn

[A07] 数字转字符串
来源：http://ncq.9152youxi.cn

Py:   str(42)
来源：http://fcf.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://zmm.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://pxa.ivvv.top

TS:   String(42)
来源：http://wgk.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rlq.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://ofb.jlsjyb.cn

Ruby: 42.to_s
来源：http://zhg.chenjidiqi.icu

C#:   42.ToString()
来源：http://pjs.snrcjt.cn

[A08] 取整与四舍五入
来源：http://mkx.quarkkingdee.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rhh.nanxuanxn.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://spe.hywenlv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xlg.xuetiantiany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ptz.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sjr.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hhv.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ise.bbcook.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bkx.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://krx.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xju.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vdn.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://glw.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tdb.birdmap.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ekm.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cgp.tanke756.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yzh.zhongyouzk.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bwj.hfpthk.cn

[A10] 生成随机数
来源：http://ctn.gzhubu.top

Py:   import random; random.randint(1, 100)
来源：http://fzp.ehwqpu.com

PHP:  random_int(1, 100);
来源：http://qnh.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vud.zhaomingkeji.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jcc.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://pqe.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ikb.jianghu66.top

Ruby: rand(1..100)
来源：http://rdi.zhaomingkeji.xyz

C#:   new Random().Next(1, 101)
来源：http://avm.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://wzv.bjfxy.top

Py:   "yes" if x > 0 else "no"
来源：http://tfd.yanxiufei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ljs.fehbvm.com

JS:   x > 0 ? "yes" : "no"
来源：http://ffg.yvedp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fcp.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://jsv.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://efs.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bay.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://nbf.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://iqb.smart0.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xwp.jyoumei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://odd.gogol.net.cn

JS:   `Hello, ${name}!`
来源：http://xuq.316326.xyz

TS:   `Hello, ${name}!`
来源：http://agx.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://zgj.zhongyouzk.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tmg.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://ijo.hcnkem.com

C#:   $"Hello, {name}!"
来源：http://hkc.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qbw.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://iai.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://kep.sweek.top

JS:   "第一行\n第二行"
来源：http://svw.svipenyu.cn

TS:   "第一行\n第二行"
来源：http://elu.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://rmi.sweek.top

Go:   "第一行\n第二行"
来源：http://rvc.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://inj.yongpay.top

C#:   "第一行\n第二行"
来源：http://pkw.xylfe.cn

[A14] 注释写法
来源：http://xvo.nanxinkj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://css.tianlin.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://fiu.hysaishi.cn

JS:   // 单行；/* 多行 */
来源：http://mxe.jinqigfzy.top

TS:   // 单行；/* 多行 */
来源：http://bqh.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ugp.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://yem.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://axv.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://siv.yj20258.top

[A15] 空值判断与默认值
来源：http://uxe.uphjek.com

Py:   value = data or "默认值"
来源：http://epj.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://csc.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://rqx.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://ray.yuanzhike.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ebw.jinghuilouyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://lti.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://gbm.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://uqb.gotoacloud.top

[A16] 真假值判断规则
来源：http://pus.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ngl.jianghu66.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://szb.gotoacloud.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vha.pycfn.com

TS:   if (!x) {}
来源：http://xcv.hnxiangtu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hte.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://flh.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vku.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://okq.gogol.net.cn

[A17] 位运算
来源：http://vsp.jinqigufen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgy.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qst.ivvv.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://brp.jinyuanbaomall.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gxl.dianchejie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wjv.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baq.jinqigufen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zgf.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmh.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://dth.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://kdp.gogol.net.cn

PHP:  ord("A"); chr(65)
来源：http://wgh.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yjq.iojbl.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ofa.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://mwy.jinghuilouyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jtj.tian-w.cn

Ruby: "A".ord; 65.chr
来源：http://dat.zhixingplan.top

C#:   (int)'A'; (char)65
来源：http://qqp.mhx1999.top

[A19] 交换两个变量
来源：http://afx.hongshengwenyu.top

Py:   a, b = b, a
来源：http://rcn.fengsongda.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pqh.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://tyh.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://ipw.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://irk.jqgufenzy.top

Go:   a, b = b, a
来源：http://yny.shzxlz.cn

Ruby: a, b = b, a
来源：http://gyn.jinqigfzy.top

C#:   (a, b) = (b, a);
来源：http://hbz.yuxming.cn

[A20] 读取标准输入
来源：http://ruz.aibaodan.cn

Py:   name = input("请输入：")
来源：http://pkk.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://znq.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vbn.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://mdc.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://hdh.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ted.jqgufenzy.top

Ruby: gets.chomp
来源：http://eod.yueranfly.top

C#:   Console.ReadLine();
来源：http://abw.uphjek.com

[A21] 保留指定小数位输出
来源：http://kdh.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://akf.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cbf.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://ijr.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://gkc.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://zry.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qwl.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://vew.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://aym.gogol.net.cn

[A22] 获取字符串长度
来源：http://jjv.0kj1m.cn

Py:   len(s)
来源：http://cpd.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qam.zhengqikj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ajx.xuanzx.com

TS:   s.length
来源：http://pvb.nwbrower.top

Java: s.length()
来源：http://tsd.gaohongyu789.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ate.chenjidiqi.icu

Ruby: s.length
来源：http://dbd.smart0.xyz

C#:   s.Length
来源：http://dsk.epnwcf.com

[A23] 大小写转换
来源：http://ngc.yangfankeji.com

Py:   s.upper(); s.lower(); s.title()
来源：http://xpv.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bnz.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://upw.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fnw.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gof.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dvd.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kns.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nrr.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://vhw.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eyi.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xdt.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ntq.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qzs.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ima.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://uwd.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://feo.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wss.fzhhl.top

[A25] 字符串比较
来源：http://bhm.guowangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://jvm.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://byd.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hpe.jinqigufen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pgl.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zml.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qbo.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nsz.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qeb.yonumen.top

[A26] 类型转换总览
来源：http://acm.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hmg.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jgt.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://exw.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://fcw.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gmn.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jyz.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://zwt.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dvs.tian-w.cn

================================================================================
来源：http://ptl.jqgufenzy.top

B. 流程控制
来源：http://azz.yj20258888.top

================================================================================
来源：http://pbz.cdnleiting.top

[B01] 条件判断 if / else
来源：http://vim.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://hav.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ibs.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tmf.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rzr.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://rey.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dta.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://atk.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://osh.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://bmm.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://anf.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://shc.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izs.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://orn.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbd.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xdj.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mfe.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqe.hammf.cn

[B03] switch / match / case
来源：http://hrg.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qfz.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://txn.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gii.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://joc.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://clq.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ypk.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mop.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cxx.hywenlv.cn

[B04] for 计数循环
来源：http://eor.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://shg.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vrj.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ydy.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://otv.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lrb.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jog.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://vlw.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xxb.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://tgo.ybcxt.top

Py:   for item in arr: print(item)
来源：http://fgb.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dkg.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fjk.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ica.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rjr.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qrz.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://gsm.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ekm.hcnkem.com

[B06] 遍历字典 / 对象
来源：http://nco.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tem.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://asd.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sgs.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iha.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yqa.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wbz.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dqg.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xpt.0kj1m.cn

[B07] while 循环
来源：http://gth.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://vub.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://rab.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://oex.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://vho.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://llq.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dnf.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://qmo.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://tuu.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://rag.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://cek.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gxq.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://yui.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://khu.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://fav.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://boo.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zpm.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://uoh.birdmap.top

[B09] break 与 continue
来源：http://dsg.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://amk.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://srw.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckp.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nap.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgi.redwolf501.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rex.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uai.sweek.top


<!-- 参考信息 -->