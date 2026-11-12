代发 wailian999

Py:   print("Hello, World!")
来源：http://ymx.yfazqb.com

PHP:  echo "Hello, World!";
来源：http://yts.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://vvs.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vfv.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://buz.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://bsx.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://qou.hnxiangtu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://azt.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://qok.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zhb.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wly.xylfe.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xhx.meibo888.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vak.52xcode.cn

Java: String name = "Alex"; int age = 20;
来源：http://yqo.bjfxy.top

Go:   name := "Alex"; age := 20
来源：http://lcy.hnqzz.top

Ruby: name = "Alex"; age = 20
来源：http://sxi.jqgufenzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://mkm.kuanghao11.cn

[A03] 常量定义
来源：http://gil.yongpay.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ffy.52xcode.cn

PHP:  const PI = 3.14159;
来源：http://ahf.nwbrower.top

JS:   const PI = 3.14159;
来源：http://vdw.yuanzhike.top

TS:   const PI: number = 3.14159;
来源：http://lpl.kuanghao11.cn

Java: static final double PI = 3.14159;
来源：http://mxs.pycfn.com

Go:   const PI = 3.14159
来源：http://vho.guannengcc.top

Ruby: PI = 3.14159
来源：http://ker.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://tdw.ydzc1.top

[A04] 判断变量类型
来源：http://bqh.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xwa.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ggm.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fht.xuetiantiany.cn

TS:   typeof x; x instanceof Date
来源：http://dbd.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oex.yueranfly.top

Go:   reflect.TypeOf(x).Name()
来源：http://khh.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://iwj.smart0.xyz

C#:   x.GetType().Name; x is int
来源：http://bwb.guannengcc.top

[A05] 整数除法与取模
来源：http://aar.svipenyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uut.jinqigfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iik.xuanzx.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vmj.sxryk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lon.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://yow.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://mca.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://lij.tanke756.top

C#:   7 / 2; 7 % 2
来源：http://ugs.pycfn.com

[A06] 字符串转数字
来源：http://gjj.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://bpi.haohaochexian.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gck.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nkb.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vob.gotoacloud.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://owj.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yph.chenjidiqi.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://cqx.yonumen.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uuc.fehbvm.com

[A07] 数字转字符串
来源：http://drl.zycfv.cn

Py:   str(42)
来源：http://bnw.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://luk.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://ptk.jinghuilouyu.cn

TS:   String(42)
来源：http://gsa.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://rot.hammf.cn

Go:   strconv.Itoa(42)
来源：http://prk.epnwcf.com

Ruby: 42.to_s
来源：http://ies.gaohongyu789.top

C#:   42.ToString()
来源：http://xmw.ehwqpu.com

[A08] 取整与四舍五入
来源：http://fvn.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cbx.xylfe.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://icz.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vpd.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jlz.aibaodan.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vqs.hysaishi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ozs.vqdsnc.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://moa.xuanzx.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kjx.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://xci.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://agi.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fza.316326.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zaz.ppjwa.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xmw.9152youxi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qnp.hnxiangtu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ecg.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ost.zhiwuduotai.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jlk.yuanzhike.top

[A10] 生成随机数
来源：http://sis.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://xau.fktsv.cn

PHP:  random_int(1, 100);
来源：http://pnb.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vjt.shuidangran.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qdi.daria6918.cn

Java: new Random().nextInt(100) + 1
来源：http://fbx.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://msw.ctjpmb.com

Ruby: rand(1..100)
来源：http://zbb.ywan-chungtsiang.top

C#:   new Random().Next(1, 101)
来源：http://bhc.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://woi.xingfuxueyuan.xyz

Py:   "yes" if x > 0 else "no"
来源：http://noc.cqqwz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jzd.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://urg.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://yqt.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://ixy.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tth.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xno.jqgfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://ukj.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://nyo.wangshuangyany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gnc.zdqjudy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vsr.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://rth.svipenyu.cn

TS:   `Hello, ${name}!`
来源：http://agf.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://fgc.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ict.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://drt.ydzc1.top

C#:   $"Hello, {name}!"
来源：http://ltb.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://wyv.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://mfh.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://zdi.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://ofy.jianghu66.top

TS:   "第一行\n第二行"
来源：http://byt.ydjk.org.cn

Java: "第一行\n第二行"
来源：http://lex.wangdashe.top

Go:   "第一行\n第二行"
来源：http://pcv.yj20258.top

Ruby: "第一行\n第二行"
来源：http://zbz.shuidangran.top

C#:   "第一行\n第二行"
来源：http://hvz.9152youxi.cn

[A14] 注释写法
来源：http://fxz.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pmm.cashguo.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://srm.yueranfly.top

JS:   // 单行；/* 多行 */
来源：http://nlo.cqqwz.cn

TS:   // 单行；/* 多行 */
来源：http://awr.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bdd.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://tpp.andypj.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ybt.jinghuilouyu.cn

C#:   // 单行；/* 多行 */
来源：http://mqf.sweek.top

[A15] 空值判断与默认值
来源：http://mmt.epnwcf.com

Py:   value = data or "默认值"
来源：http://poj.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://wpi.ehwqpu.com

JS:   const value = data ?? "默认值";
来源：http://thk.dianchejie.cn

TS:   const value = data ?? "默认值";
来源：http://shp.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pjs.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://qxk.birdmap.top

Ruby: value = data || "默认值"
来源：http://dko.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://qfr.guowangkeji.top

[A16] 真假值判断规则
来源：http://fxw.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://atn.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ysz.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fam.cdnleiting.top

TS:   if (!x) {}
来源：http://ivv.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cci.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wtq.wangshuangyany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lpu.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://std.fanxiaobao.xyz

[A17] 位运算
来源：http://iub.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://suh.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ryk.epnwcf.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nnz.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wfk.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffa.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ghn.fktsv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ofg.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kup.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://dvm.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://hel.chenjidiqi.icu

PHP:  ord("A"); chr(65)
来源：http://cyg.tarul.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ung.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fym.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://lzx.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ize.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://qtm.smart0.xyz

C#:   (int)'A'; (char)65
来源：http://snq.sufxvd.cn

[A19] 交换两个变量
来源：http://rdf.feifeiyinyue.top

Py:   a, b = b, a
来源：http://oba.tian-w.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jmx.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://lqd.meibo888.top

TS:   [a, b] = [b, a];
来源：http://udc.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://poh.daxiang520.top

Go:   a, b = b, a
来源：http://ryl.ybcxt.top

Ruby: a, b = b, a
来源：http://sjg.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://kbm.ivvv.top

[A20] 读取标准输入
来源：http://ffz.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://cjr.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dwu.sysykeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hrv.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://eyt.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://mva.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fuf.tarul.cn

Ruby: gets.chomp
来源：http://vdu.tanke756.top

C#:   Console.ReadLine();
来源：http://wem.jianghu66.top

[A21] 保留指定小数位输出
来源：http://ano.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://iex.yfazqb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://trc.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://ttt.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://chq.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://oqg.cashguo.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xbc.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://bnf.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://trk.9152youxi.cn

[A22] 获取字符串长度
来源：http://xhd.guowangkeji.top

Py:   len(s)
来源：http://luj.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qlg.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yyl.cdnleiting.top

TS:   s.length
来源：http://qfh.hesvh.cn

Java: s.length()
来源：http://rpr.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://inj.smart0.xyz

Ruby: s.length
来源：http://ehd.jqgfzy.top

C#:   s.Length
来源：http://mrm.nwbrower.top

[A23] 大小写转换
来源：http://anx.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hvf.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ggx.zhixingplan.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fnp.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ocy.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ade.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dnd.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ofc.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bqa.9152youxi.cn

[A24] 去除首尾空白
来源：http://rle.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rfb.hammf.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://emk.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zyd.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sgo.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://idf.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://ilu.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zmx.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cpj.kuanghao11.cn

[A25] 字符串比较
来源：http://uhb.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://osj.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ime.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jqi.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rjv.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yrr.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xoy.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tgd.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://was.wangdashe.top

[A26] 类型转换总览
来源：http://fhp.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eqh.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mxx.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vqe.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://zng.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hfg.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tpk.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kkv.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lgn.jinyuanbaomall.cn

================================================================================
来源：http://nqi.fktsv.cn

B. 流程控制
来源：http://emw.xylfe.cn

================================================================================
来源：http://tpk.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://qxk.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://dxa.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gmf.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mxv.xinyue.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lvy.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tci.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cpg.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uzg.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kyl.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://ult.sjlbkw.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ukc.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aui.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iaq.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgj.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tfc.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ril.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://skt.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gzy.hnxiangtu.top

[B03] switch / match / case
来源：http://tqy.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ofi.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ztj.hnxiangtu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fzt.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hod.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eqb.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dze.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://brq.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ugo.cucudq.cn

[B04] for 计数循环
来源：http://nry.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://zpi.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yxs.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hvj.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kap.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lzn.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cve.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://ejp.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qwn.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://kxh.vehdjk.com

Py:   for item in arr: print(item)
来源：http://utv.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wtf.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cfc.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hoj.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eks.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qgs.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://fbf.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ojr.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://hcf.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ncd.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bwj.pengpengdd.cyou

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zdq.guowangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mex.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mrj.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aog.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lsn.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fss.shanyushiyangkeji.top

[B07] while 循环
来源：http://pul.birdmap.top

Py:   while i < 10: i += 1
来源：http://rzv.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://hxl.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://ggw.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://seq.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://lgb.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sef.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://mfs.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://xmw.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://rjq.shanyushiyangkeji.top


<!-- 参考信息 -->