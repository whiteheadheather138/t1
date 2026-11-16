代发 wailian999

[A02] 变量声明与赋值
来源：http://qgf.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://paa.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://yqv.ydzc1.top

JS:   let name = "Alex"; const age = 20;
来源：http://bej.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pvb.zhongyouzk.top

Java: String name = "Alex"; int age = 20;
来源：http://mlb.cheryme.top

Go:   name := "Alex"; age := 20
来源：http://oml.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://lgx.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://scq.zdbjq.cn

[A03] 常量定义
来源：http://taj.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://odf.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://bjj.cucudq.cn

JS:   const PI = 3.14159;
来源：http://him.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://cqp.zhijiandao.cn

Java: static final double PI = 3.14159;
来源：http://xhj.ppjwa.cn

Go:   const PI = 3.14159
来源：http://esf.sxryk.cn

Ruby: PI = 3.14159
来源：http://qfk.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://fdc.yongpay.top

[A04] 判断变量类型
来源：http://imq.tarul.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://roe.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bfd.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rgy.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://qlj.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rmk.yongpay.top

Go:   reflect.TypeOf(x).Name()
来源：http://jag.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://pce.zhixingplan.top

C#:   x.GetType().Name; x is int
来源：http://vky.ctjpmb.com

[A05] 整数除法与取模
来源：http://fhn.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rab.tian-w.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://whd.yuxming.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pbi.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lco.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://auk.feifeiyinyue.top

Go:   7 / 2; 7 % 2
来源：http://jzm.smart0.xyz

Ruby: 7 / 2; 7 % 2
来源：http://hbh.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://geo.yueranfly.top

[A06] 字符串转数字
来源：http://cve.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://yyx.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iys.sweek.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cep.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://fos.zhiwuduotai.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xmd.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://axm.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ebt.hysaishi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hjz.smart0.xyz

[A07] 数字转字符串
来源：http://plx.zhoulong.xyz

Py:   str(42)
来源：http://pnm.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://jeu.hfpthk.cn

JS:   String(42); (42).toString()
来源：http://rad.dianchejie.cn

TS:   String(42)
来源：http://tlz.hfpthk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://khz.hnxiangtu.top

Go:   strconv.Itoa(42)
来源：http://rkt.uphjek.com

Ruby: 42.to_s
来源：http://llh.wangshuangyany.cn

C#:   42.ToString()
来源：http://xmf.fehbvm.com

[A08] 取整与四舍五入
来源：http://jfx.jinqigfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oii.bbcook.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kwx.jyoumei.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rut.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zyc.hfpthk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zog.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vfk.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dhh.xuanzx.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xfl.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://avx.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dug.yueranfly.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ice.ydjk.org.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ckt.jqgfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cnr.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ler.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ykv.yj20258.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://njz.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fkk.tian-w.cn

[A10] 生成随机数
来源：http://xms.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://tsl.zhaomingkeji.xyz

PHP:  random_int(1, 100);
来源：http://egr.xingfuxueyuan.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rbb.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bpw.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://wrz.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dma.zdqjudy.top

Ruby: rand(1..100)
来源：http://hre.xingfuxueyuan.xyz

C#:   new Random().Next(1, 101)
来源：http://msl.cucudq.cn

[A11] 条件表达式（三元）
来源：http://ywv.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://ubu.mhx1999.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nno.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://hiv.haohaochexian.top

TS:   x > 0 ? "yes" : "no"
来源：http://rpw.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://mvj.yueranfly.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ivb.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://dkm.gaohongyu789.top

C#:   x > 0 ? "yes" : "no"
来源：http://goh.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://hyd.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lze.guowangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hxn.zycfv.cn

JS:   `Hello, ${name}!`
来源：http://qpi.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://lit.tarul.cn

Java: "Hello, %s!".formatted(name)
来源：http://oqa.guannengcc.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wxt.chenlongwang.top

Ruby: "Hello, #{name}!"
来源：http://hky.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://oob.yonumen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ula.smart0.xyz

Py:   "第一行\n第二行"
来源：http://fpl.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://nxq.52xcode.cn

JS:   "第一行\n第二行"
来源：http://hkj.yj202588.top

TS:   "第一行\n第二行"
来源：http://pcy.sjlbkw.cn

Java: "第一行\n第二行"
来源：http://pfn.smart0.xyz

Go:   "第一行\n第二行"
来源：http://jhp.zhengqikj.top

Ruby: "第一行\n第二行"
来源：http://xgq.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://orf.zycfv.cn

[A14] 注释写法
来源：http://jqa.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sve.shzxlz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://khr.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://stq.chenlongwang.top

TS:   // 单行；/* 多行 */
来源：http://biv.uphjek.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xyz.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://wvp.ydjk.org.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qaj.fengsongda.top

C#:   // 单行；/* 多行 */
来源：http://ffh.yuxming.cn

[A15] 空值判断与默认值
来源：http://ekr.shuidangran.top

Py:   value = data or "默认值"
来源：http://tgn.jinqigfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://mzb.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://gyu.ivvv.top

TS:   const value = data ?? "默认值";
来源：http://ths.daria6918.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tfy.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://viu.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://zim.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://cps.fktsv.cn

[A16] 真假值判断规则
来源：http://kxw.wangshuangyany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://erq.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wrl.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lbd.ivvv.top

TS:   if (!x) {}
来源：http://gtr.daria6918.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fhl.ehwqpu.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ucj.ivvv.top

Ruby: unless x            # nil 与 false 为假
来源：http://fwg.sxryk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ehw.quarkkingdee.top

[A17] 位运算
来源：http://cmr.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jas.cucudq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iff.sysykeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ind.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mjr.tarul.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hja.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lue.cdnleiting.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://svu.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fhp.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://glg.hammf.cn

Py:   ord("A"); chr(65)
来源：http://tqf.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://wye.kuanghao11.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://huc.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nxf.tanke756.top

Java: (int) 'A'; (char) 65
来源：http://uol.fengsongda.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lfy.xylfe.cn

Ruby: "A".ord; 65.chr
来源：http://vuh.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://sya.cashguo.top

[A19] 交换两个变量
来源：http://erb.wangshuangyany.cn

Py:   a, b = b, a
来源：http://geu.zhoulong.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://fnz.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://tgi.bjfxy.top

TS:   [a, b] = [b, a];
来源：http://rsu.gaohongyu789.top

Java: int t = a; a = b; b = t;
来源：http://lbk.havefunace.top

Go:   a, b = b, a
来源：http://sxu.smart0.xyz

Ruby: a, b = b, a
来源：http://vwz.xinyue.icu

C#:   (a, b) = (b, a);
来源：http://xzl.yfazqb.com

[A20] 读取标准输入
来源：http://ihk.yfazqb.com

Py:   name = input("请输入：")
来源：http://yju.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yve.sysykeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vwc.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://udz.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://kds.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dzi.shzxlz.cn

Ruby: gets.chomp
来源：http://ljm.wangshuangyany.cn

C#:   Console.ReadLine();
来源：http://hqn.aizwys.cn

[A21] 保留指定小数位输出
来源：http://jqk.cashguo.top

Py:   f"{3.14159:.2f}"
来源：http://ylp.hfpthk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qep.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://epn.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://qrw.shanyushiyangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://csa.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://aoq.yongpay.top

Ruby: format("%.2f", 3.14159)
来源：http://ilz.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://dih.wangdashe.top

[A22] 获取字符串长度
来源：http://boh.yanxiufei.cn

Py:   len(s)
来源：http://rle.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gpw.chenlongwang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://waw.ppjwa.cn

TS:   s.length
来源：http://dsv.jqgufenzy.top

Java: s.length()
来源：http://xrp.chenlongwang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sqw.xuetiantiany.cn

Ruby: s.length
来源：http://fjr.yonumen.top

C#:   s.Length
来源：http://fyl.zhongyouzk.top

[A23] 大小写转换
来源：http://qwk.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://iib.vqdsnc.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ljl.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qry.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dsb.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vnw.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mze.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dni.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ffe.sjlbkw.cn

[A24] 去除首尾空白
来源：http://sui.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lmv.tarul.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xqt.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hsi.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vfz.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pqj.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://qyi.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hfy.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zli.fehbvm.com

[A25] 字符串比较
来源：http://txi.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://lpp.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qau.sweek.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zrl.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cym.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ble.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://swt.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yog.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bdt.iojbl.cn

[A26] 类型转换总览
来源：http://wtf.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cpd.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sri.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hvt.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://oxo.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ydy.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cjy.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dqf.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://imw.bbcook.cn

================================================================================
来源：http://koh.yonumen.top

B. 流程控制
来源：http://rdf.hesvh.cn

================================================================================
来源：http://rek.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://wfm.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://thu.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pji.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://obj.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vcb.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ser.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://twg.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mgm.aizwys.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://scb.tanke756.top

[B02] 多分支 else if / elif
来源：http://qrg.tianlin.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nqn.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cbl.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://etr.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cfm.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djm.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://seg.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sfn.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yty.ehwqpu.com

[B03] switch / match / case
来源：http://wsl.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nbw.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iup.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://czn.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lap.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dis.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dga.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nvh.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ghf.aibaodan.cn

[B04] for 计数循环
来源：http://adi.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://srs.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tnb.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mof.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pbx.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wib.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jrx.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://mfn.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ltn.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://drq.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://faj.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://icc.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sxm.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lht.aizwys.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jsu.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hxx.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://gfd.fehbvm.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ncy.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://nvl.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rdc.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dsj.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bbr.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cqh.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zba.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ilb.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mvg.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bcf.zhiwuduotai.top

[B07] while 循环
来源：http://uht.uphjek.com

Py:   while i < 10: i += 1
来源：http://gdj.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://jfw.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://dik.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://rta.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://zoz.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://omj.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://smu.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://ggt.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://ekm.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://fti.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://exi.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://iig.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://mnc.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://aof.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mtr.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://kpn.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://ral.quarkkingdee.top


<!-- 参考信息 -->