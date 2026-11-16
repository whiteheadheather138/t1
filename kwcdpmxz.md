代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://eph.ywan-chungtsiang.top

[A03] 常量定义
来源：http://omr.tian-w.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://svm.jiagoushi.top

PHP:  const PI = 3.14159;
来源：http://hor.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://fyh.shzxlz.cn

TS:   const PI: number = 3.14159;
来源：http://wmt.tianlin.xyz

Java: static final double PI = 3.14159;
来源：http://sqa.shanyushiyangkeji.top

Go:   const PI = 3.14159
来源：http://css.yongpay.top

Ruby: PI = 3.14159
来源：http://vmt.jinqigufen.top

C#:   const double PI = 3.14159;
来源：http://sho.shanyushiyangtech.top

[A04] 判断变量类型
来源：http://gga.chenlongwang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ifw.snrcjt.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xjq.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kfz.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://tns.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xqh.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kxt.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mde.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://kgg.dashuyun.cn

[A05] 整数除法与取模
来源：http://sve.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jqt.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://afm.ydjk.org.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tcv.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lna.ywan-chungtsiang.top

Java: 7 / 2; 7 % 2
来源：http://jlp.hammf.cn

Go:   7 / 2; 7 % 2
来源：http://kau.ppjwa.cn

Ruby: 7 / 2; 7 % 2
来源：http://nxv.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://trv.bjfxy.top

[A06] 字符串转数字
来源：http://zck.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://sjq.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jfw.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cpl.daria6918.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gxw.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zhr.ydjk.org.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bdo.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://atj.yj20258.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cnm.pengpengdd.cyou

[A07] 数字转字符串
来源：http://cbf.yueranfly.top

Py:   str(42)
来源：http://czy.epnwcf.com

PHP:  (string) 42; strval(42)
来源：http://pka.shuidangran.top

JS:   String(42); (42).toString()
来源：http://etz.yuxming.cn

TS:   String(42)
来源：http://qpb.gotoacloud.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dwa.tian-w.cn

Go:   strconv.Itoa(42)
来源：http://gfq.yvedp.cn

Ruby: 42.to_s
来源：http://ayk.sjlbkw.cn

C#:   42.ToString()
来源：http://bep.shzxlz.cn

[A08] 取整与四舍五入
来源：http://vst.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lao.zhixingplan.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fty.yuanzhike.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://egk.jianghu66.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ttt.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kyj.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qdg.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yjz.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rmb.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://gbj.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cve.epnwcf.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vsb.svipenyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wmm.zycfv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xhh.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iii.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hxa.chenlongwang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bbi.jinqigfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bju.zhijiandao.cn

[A10] 生成随机数
来源：http://icg.xuanzx.com

Py:   import random; random.randint(1, 100)
来源：http://yap.uphjek.com

PHP:  random_int(1, 100);
来源：http://akr.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lbr.zhoulong.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zvq.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://jmy.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gaq.andypj.xyz

Ruby: rand(1..100)
来源：http://aaw.nwbrower.top

C#:   new Random().Next(1, 101)
来源：http://nzf.yj20258.top

[A11] 条件表达式（三元）
来源：http://vut.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://wdw.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://teq.sxryk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jbv.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://eud.zhiwuduotai.top

Java: x > 0 ? "yes" : "no"
来源：http://gut.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://mqf.yvedp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mfo.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://sse.yangfankeji.com

[A12] 字符串插值 / 格式化
来源：http://viw.yj20258.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hxu.guowangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://amf.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://cym.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://hps.zhoulong.xyz

Java: "Hello, %s!".formatted(name)
来源：http://amw.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tqm.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://uxm.nanxinkj.top

C#:   $"Hello, {name}!"
来源：http://qel.ehwqpu.com

[A13] 多行字符串（练习 \n 转义）
来源：http://max.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://cop.c1oappe.top

PHP:  "第一行\n第二行"
来源：http://bxn.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://qex.xylfe.cn

TS:   "第一行\n第二行"
来源：http://kch.chenzaomai.com

Java: "第一行\n第二行"
来源：http://jin.redwolf501.top

Go:   "第一行\n第二行"
来源：http://qcv.fzhhl.top

Ruby: "第一行\n第二行"
来源：http://uqp.ctjpmb.com

C#:   "第一行\n第二行"
来源：http://ctm.hcnkem.com

[A14] 注释写法
来源：http://hed.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ntx.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://izc.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://tgo.nwbrower.top

TS:   // 单行；/* 多行 */
来源：http://cnk.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://php.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://uuq.dianchejie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ncd.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://xua.dianchejie.cn

[A15] 空值判断与默认值
来源：http://hha.ehwqpu.com

Py:   value = data or "默认值"
来源：http://gqf.iojbl.cn

PHP:  $value = $data ?? "默认值";
来源：http://ueq.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://zbk.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://tue.kuanghao11.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xck.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://pbx.jianghu66.top

Ruby: value = data || "默认值"
来源：http://ltq.zycfv.cn

C#:   var value = data ?? "默认值";
来源：http://lzu.gogol.net.cn

[A16] 真假值判断规则
来源：http://scw.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://afm.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tce.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hzw.snrcjt.cn

TS:   if (!x) {}
来源：http://mwg.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cjb.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iib.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://plf.daria6918.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lfu.smart0.xyz

[A17] 位运算
来源：http://rnu.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://etq.sysykeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gdr.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://whc.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xwm.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lpo.aizwys.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://noz.yonumen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rqb.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqq.gzhubu.top

[A18] 字符与 ASCII 码互转
来源：http://ebp.hysaishi.cn

Py:   ord("A"); chr(65)
来源：http://tnb.sufxvd.cn

PHP:  ord("A"); chr(65)
来源：http://bxi.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://smv.ehwqpu.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uyg.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://qrk.vehdjk.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pex.ivvv.top

Ruby: "A".ord; 65.chr
来源：http://otm.yongpay.top

C#:   (int)'A'; (char)65
来源：http://zot.yuanzhike.top

[A19] 交换两个变量
来源：http://goi.jinqigfzy.top

Py:   a, b = b, a
来源：http://lwi.sxryk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iqk.dashuyun.cn

JS:   [a, b] = [b, a];
来源：http://xez.zdqjudy.top

TS:   [a, b] = [b, a];
来源：http://pkv.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://oro.ppjwa.cn

Go:   a, b = b, a
来源：http://mac.gzhubu.top

Ruby: a, b = b, a
来源：http://jrf.daria6918.cn

C#:   (a, b) = (b, a);
来源：http://dcs.ydjk.org.cn

[A20] 读取标准输入
来源：http://brf.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://tov.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://yrl.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hjj.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://vpv.yangfankeji.com

Java: new Scanner(System.in).nextLine()
来源：http://dmj.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://srr.yvedp.cn

Ruby: gets.chomp
来源：http://xdv.c1oappe.top

C#:   Console.ReadLine();
来源：http://gni.epnwcf.com

[A21] 保留指定小数位输出
来源：http://mef.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://vti.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jik.shangyingyoupin.top

JS:   (3.14159).toFixed(2)
来源：http://ehl.chenzaomai.com

TS:   (3.14159).toFixed(2)
来源：http://hjc.jinqigufen.top

Java: String.format("%.2f", 3.14159)
来源：http://ocs.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dps.tanke756.top

Ruby: format("%.2f", 3.14159)
来源：http://vwv.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://ouu.xuetiantiany.cn

[A22] 获取字符串长度
来源：http://tas.52xcode.cn

Py:   len(s)
来源：http://knm.ctjpmb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gju.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://btn.zhijiandao.cn

TS:   s.length
来源：http://qzo.fehbvm.com

Java: s.length()
来源：http://qkp.sysykeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dds.jinqigufen.top

Ruby: s.length
来源：http://yqg.zdbjq.cn

C#:   s.Length
来源：http://nkr.haohaochexian.top

[A23] 大小写转换
来源：http://skm.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xzx.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xlq.yj20258.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://isl.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yld.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fbr.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ijr.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://exh.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dlx.iojbl.cn

[A24] 去除首尾空白
来源：http://rac.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mcf.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jxm.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqh.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yat.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pky.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://dvg.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bwb.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://izr.epnwcf.com

[A25] 字符串比较
来源：http://xgq.gaohongyu789.top

Py:   s1 == s2; s1 != s2
来源：http://sgf.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yzf.fanxiaobao.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qyw.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://klz.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://avp.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ymh.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://kaq.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ysx.jinqigufen.top

[A26] 类型转换总览
来源：http://ewz.gaohongyu789.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://twq.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://efs.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rdh.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://nwb.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kks.jiagoushi.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hzp.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rzw.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zbs.yj202588.top

================================================================================
来源：http://wsd.chenzaomai.com

B. 流程控制
来源：http://chc.ivvv.top

================================================================================
来源：http://mwg.chenzaomai.com

[B01] 条件判断 if / else
来源：http://hvs.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://abe.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bgd.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cmu.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://abe.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://mpn.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xub.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ztj.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nxd.jianghu66.top

[B02] 多分支 else if / elif
来源：http://sng.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://npt.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://anq.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yuw.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://suh.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvu.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pyx.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hfy.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rfi.hongshengwenyu.top

[B03] switch / match / case
来源：http://bdi.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xyu.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rve.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://axj.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ulf.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cbz.shanyushiyangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fco.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iik.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bcj.hywenlv.cn

[B04] for 计数循环
来源：http://uol.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://pdk.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://prs.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://glb.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lpq.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xqd.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iiw.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://avw.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vat.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://rve.jinghuilouyu.cn

Py:   for item in arr: print(item)
来源：http://ckj.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pqs.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kzj.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ifo.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://pel.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://unr.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://ouj.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://grl.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://vor.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wij.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eti.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oap.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://noz.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gkv.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kdq.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://szm.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ovn.hcnkem.com

[B07] while 循环
来源：http://hdu.yuxming.cn

Py:   while i < 10: i += 1
来源：http://lbf.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://agv.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://oli.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://jib.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://evv.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qvk.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://zad.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://ktp.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://ric.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ykb.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://gvq.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://phv.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://wxc.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://kzf.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ypy.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://zqp.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://agp.pycfn.com

[B09] break 与 continue
来源：http://nuq.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rgf.xziqi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bkc.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mii.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vfg.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmx.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://srm.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tin.haohaochexian.top


<!-- 参考信息 -->