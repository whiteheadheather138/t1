代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://bpa.ydzc1.top

[A03] 常量定义
来源：http://kie.yonumen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yzx.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://bfd.daxiang520.top

JS:   const PI = 3.14159;
来源：http://dlp.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://omc.birdmap.top

Java: static final double PI = 3.14159;
来源：http://mgo.jqgfzy.top

Go:   const PI = 3.14159
来源：http://jos.hnqzz.top

Ruby: PI = 3.14159
来源：http://fxt.tarul.cn

C#:   const double PI = 3.14159;
来源：http://jfa.shuidangran.top

[A04] 判断变量类型
来源：http://wmc.fengsongda.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zpm.vqdsnc.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gus.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nol.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://iik.zhixingplan.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fdd.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dtq.wangdashe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xbd.dianchejie.cn

C#:   x.GetType().Name; x is int
来源：http://ryl.sxryk.cn

[A05] 整数除法与取模
来源：http://dmd.yvedp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://unw.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ybn.yj202588.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xqs.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ydf.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://cfo.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://ezg.tanke756.top

Ruby: 7 / 2; 7 % 2
来源：http://cjo.zdbjq.cn

C#:   7 / 2; 7 % 2
来源：http://wom.fehbvm.com

[A06] 字符串转数字
来源：http://bnj.jianghu66.top

Py:   int("42"); float("3.14")
来源：http://lbh.hcnkem.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bmg.guannengcc.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lwk.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://ebt.yangfankeji.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xyr.dianchejie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://spl.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://liy.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kqx.aibaodan.cn

[A07] 数字转字符串
来源：http://ljq.bjfxy.top

Py:   str(42)
来源：http://dmp.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://phs.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://vtb.feifeiyinyue.top

TS:   String(42)
来源：http://qza.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://wji.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://ohy.xziqi.cn

Ruby: 42.to_s
来源：http://dle.sufxvd.cn

C#:   42.ToString()
来源：http://tbx.tianlin.xyz

[A08] 取整与四舍五入
来源：http://iwa.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jqp.sysykeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vtc.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dnp.ybcxt.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rci.feifeiyinyue.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://umq.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kav.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kpe.shanyushiyangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yia.epnwcf.com

[A09] 绝对值与最大最小值
来源：http://jaz.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qcw.xinyue.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ovx.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nwo.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fqz.nanxinkj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yfr.ydzc1.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pzl.shanyushiyangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zvb.uphjek.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qed.gogol.net.cn

[A10] 生成随机数
来源：http://abx.wangshuangyany.cn

Py:   import random; random.randint(1, 100)
来源：http://ioy.yangfankeji.com

PHP:  random_int(1, 100);
来源：http://oku.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ssr.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hyn.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://qsg.fehbvm.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://awk.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://kjb.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://yuq.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://cpf.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://hyu.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zvl.316326.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://ujw.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://fgq.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://mhu.tarul.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wsb.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ihy.daria6918.cn

C#:   x > 0 ? "yes" : "no"
来源：http://spn.redwolf501.top

[A12] 字符串插值 / 格式化
来源：http://gfz.zdqjudy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://azd.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sgt.daxiang520.top

JS:   `Hello, ${name}!`
来源：http://djl.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://aap.iojbl.cn

Java: "Hello, %s!".formatted(name)
来源：http://hac.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rwe.chenlongwang.top

Ruby: "Hello, #{name}!"
来源：http://uvt.tarul.cn

C#:   $"Hello, {name}!"
来源：http://thv.xingfuxueyuan.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://mwr.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://loy.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://dgd.nanxinkj.top

JS:   "第一行\n第二行"
来源：http://yea.xingfuxueyuan.xyz

TS:   "第一行\n第二行"
来源：http://ifa.hysaishi.cn

Java: "第一行\n第二行"
来源：http://weh.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://sna.jyoumei.cn

Ruby: "第一行\n第二行"
来源：http://sln.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://whh.vqdsnc.cn

[A14] 注释写法
来源：http://ktv.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://axd.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://nxd.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://hfy.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://gur.yfazqb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wxp.316326.xyz

Go:   // 单行；/* 多行 */
来源：http://qvq.fengsongda.top

Ruby: # 单行；=begin 多行 =end
来源：http://tzp.yuanzhike.top

C#:   // 单行；/* 多行 */
来源：http://roq.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://ugj.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://qvh.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://xzy.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://xzw.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://kia.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yoo.svipenyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://bnh.hnxiangtu.top

Ruby: value = data || "默认值"
来源：http://bas.kuanghao11.cn

C#:   var value = data ?? "默认值";
来源：http://ulj.dianchejie.cn

[A16] 真假值判断规则
来源：http://fjg.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ban.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rbo.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rrz.iojbl.cn

TS:   if (!x) {}
来源：http://qea.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rgl.zhiwuduotai.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://myn.zhixingplan.top

Ruby: unless x            # nil 与 false 为假
来源：http://dxa.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xgm.zhongyouzk.top

[A17] 位运算
来源：http://vtj.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqw.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wds.shzxlz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://syf.hysaishi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tax.tianlin.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nml.316326.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pgy.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ayq.redwolf501.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fpe.bjfxy.top

[A18] 字符与 ASCII 码互转
来源：http://foj.sysykeji.top

Py:   ord("A"); chr(65)
来源：http://vqj.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://fqv.hfpthk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fdo.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zde.xuetiantiany.cn

Java: (int) 'A'; (char) 65
来源：http://aic.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wem.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://ouz.jqgfzy.top

C#:   (int)'A'; (char)65
来源：http://yxk.ybcxt.top

[A19] 交换两个变量
来源：http://vmt.shangyingyoupin.top

Py:   a, b = b, a
来源：http://kmi.tarul.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iya.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://zif.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://vpw.chenzaomai.com

Java: int t = a; a = b; b = t;
来源：http://xvl.xylfe.cn

Go:   a, b = b, a
来源：http://mba.gzhubu.top

Ruby: a, b = b, a
来源：http://vkv.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://zyb.pycfn.com

[A20] 读取标准输入
来源：http://cnu.cucudq.cn

Py:   name = input("请输入：")
来源：http://xab.hnxiangtu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://snn.zdqjudy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iwc.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://yfn.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://ion.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gir.zhixingplan.top

Ruby: gets.chomp
来源：http://xcf.xuanzx.com

C#:   Console.ReadLine();
来源：http://olz.nanxinkj.top

[A21] 保留指定小数位输出
来源：http://cdz.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://rya.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bxe.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://byd.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://uzp.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://ozu.shanyushiyangtech.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xvs.zhijiandao.cn

Ruby: format("%.2f", 3.14159)
来源：http://pqq.cqqwz.cn

C#:   3.14159.ToString("F2")
来源：http://vfb.andypj.xyz

[A22] 获取字符串长度
来源：http://nkw.ctjpmb.com

Py:   len(s)
来源：http://zbs.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vrd.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hgf.yj20258.top

TS:   s.length
来源：http://qdn.fehbvm.com

Java: s.length()
来源：http://tih.svipenyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rsj.bjfxy.top

Ruby: s.length
来源：http://lnl.jyoumei.cn

C#:   s.Length
来源：http://joc.shuidangran.top

[A23] 大小写转换
来源：http://pud.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://chp.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xke.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uue.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ltl.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aax.cashguo.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gav.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pjq.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ezg.nanxuanxn.top

[A24] 去除首尾空白
来源：http://lbq.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dnc.hammf.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qvu.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ilu.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pyt.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hjh.hnqzz.top

Go:   strings.TrimSpace(s)
来源：http://nkv.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dah.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://prz.jinyuanbaomall.cn

[A25] 字符串比较
来源：http://xpw.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://mbn.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uyb.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mys.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qbd.52xcode.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tep.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vrn.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ncz.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aea.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://kbf.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xkj.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://piq.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nyb.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://ryx.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oem.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fql.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hxs.xuanzx.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cdq.cashguo.top

================================================================================
来源：http://kvg.sjlbkw.cn

B. 流程控制
来源：http://alb.chenjidiqi.icu

================================================================================
来源：http://gzv.hnqzz.top

[B01] 条件判断 if / else
来源：http://tly.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ksp.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vbj.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://azh.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hpt.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mxy.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vsc.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nyl.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://plf.nwbrower.top

[B02] 多分支 else if / elif
来源：http://jpa.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mek.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://glw.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsd.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ucu.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvk.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oct.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://orv.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eat.kuanghao11.cn

[B03] switch / match / case
来源：http://coa.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lxg.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wjw.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xbf.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ecr.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pbo.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ufu.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ndo.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xcr.uphjek.com

[B04] for 计数循环
来源：http://mxa.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://dih.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://utz.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ddb.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://unc.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jgj.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://exs.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://jot.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lbu.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://kdj.daria6918.cn

Py:   for item in arr: print(item)
来源：http://ayj.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hdz.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mew.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qlv.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gjm.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fzy.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://rjm.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://maa.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://ihg.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bhg.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mvt.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oww.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vhg.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://euw.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zdj.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bhr.gaohongyu789.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fcp.yongpay.top

[B07] while 循环
来源：http://tzk.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://zpr.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jxm.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://eai.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://guz.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://dhp.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iup.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://pgd.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://gjm.cashguo.top

[B08] do-while（至少执行一次）
来源：http://fhe.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://utg.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xxn.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://foh.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://ypi.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://seh.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cri.gotoacloud.top

Ruby: begin; i += 1; end while i < 10
来源：http://lip.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://ffg.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://jym.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hxw.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wuw.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckl.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fig.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldn.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://duy.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blp.tianlin.xyz


<!-- 参考信息 -->