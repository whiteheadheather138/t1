代发 wailian999

[A02] 变量声明与赋值
来源：http://ktp.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ilm.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oep.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://sll.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mwm.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://oyz.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://kak.jqgfzy.top

Ruby: name = "Alex"; age = 20
来源：http://srp.yangfankeji.com

C#:   string name = "Alex"; int age = 20;
来源：http://qni.zhijiandao.cn

[A03] 常量定义
来源：http://haq.ydjk.org.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://peu.tianlin.xyz

PHP:  const PI = 3.14159;
来源：http://tqy.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://wlp.ppjwa.cn

TS:   const PI: number = 3.14159;
来源：http://wsy.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://nwm.9152youxi.cn

Go:   const PI = 3.14159
来源：http://wpm.wangdashe.top

Ruby: PI = 3.14159
来源：http://icz.sweek.top

C#:   const double PI = 3.14159;
来源：http://pgk.xuanzx.com

[A04] 判断变量类型
来源：http://kxk.cqqwz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qhx.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://znf.bbcook.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xec.jinghuilouyu.cn

TS:   typeof x; x instanceof Date
来源：http://klf.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://asn.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://fej.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yli.yj20258888.top

C#:   x.GetType().Name; x is int
来源：http://ctj.smart0.xyz

[A05] 整数除法与取模
来源：http://nai.gzhubu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ujj.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://ppu.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://brh.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jlb.cucudq.cn

Java: 7 / 2; 7 % 2
来源：http://iyp.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://ohz.xuetiantiany.cn

Ruby: 7 / 2; 7 % 2
来源：http://uth.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://kfr.yuxming.cn

[A06] 字符串转数字
来源：http://cvl.c1oappe.top

Py:   int("42"); float("3.14")
来源：http://ezn.yj20258888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ycr.tanke756.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ztc.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uvm.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wcv.hysaishi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mbp.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://vcn.xziqi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fpd.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://fue.yonumen.top

Py:   str(42)
来源：http://kdq.vehdjk.com

PHP:  (string) 42; strval(42)
来源：http://tse.shuidangran.top

JS:   String(42); (42).toString()
来源：http://pot.jiagoushi.top

TS:   String(42)
来源：http://hrt.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://caa.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://toi.yonumen.top

Ruby: 42.to_s
来源：http://szv.zdbjq.cn

C#:   42.ToString()
来源：http://piw.xuetiantiany.cn

[A08] 取整与四舍五入
来源：http://ydf.xuanzx.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wbt.yuxming.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mmp.9152youxi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fkr.dashuyun.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eji.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://enx.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pru.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://odq.jiagoushi.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fpb.wangshuangyany.cn

[A09] 绝对值与最大最小值
来源：http://hzd.aibaodan.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pot.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://plr.pengpengdd.cyou

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lfx.nanxinkj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qlp.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hxd.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zhk.guannengcc.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mlv.cheryme.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qqq.birdmap.top

[A10] 生成随机数
来源：http://mhl.gzhubu.top

Py:   import random; random.randint(1, 100)
来源：http://lwa.yj20258.top

PHP:  random_int(1, 100);
来源：http://ayi.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xqi.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ugd.gogol.net.cn

Java: new Random().nextInt(100) + 1
来源：http://bfj.chenlongwang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ewk.quarkkingdee.top

Ruby: rand(1..100)
来源：http://bzv.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://evk.fzhhl.top

[A11] 条件表达式（三元）
来源：http://dmz.smart0.xyz

Py:   "yes" if x > 0 else "no"
来源：http://hhs.gotoacloud.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://faz.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://hkv.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://yvg.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://vat.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://uqu.chenlongwang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://iqc.zhiwuduotai.top

C#:   x > 0 ? "yes" : "no"
来源：http://qyd.9152youxi.cn

[A12] 字符串插值 / 格式化
来源：http://som.fehbvm.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mwx.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nqr.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://vqw.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://ihw.cdnleiting.top

Java: "Hello, %s!".formatted(name)
来源：http://jpd.yj20258888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zcx.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://vba.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://qhd.cdnleiting.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gsp.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://lpk.xuetiantiany.cn

PHP:  "第一行\n第二行"
来源：http://eno.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://tvg.shuidangran.top

TS:   "第一行\n第二行"
来源：http://llp.redwolf501.top

Java: "第一行\n第二行"
来源：http://pgs.feifeiyinyue.top

Go:   "第一行\n第二行"
来源：http://iob.pengpengdd.cyou

Ruby: "第一行\n第二行"
来源：http://aen.bjfxy.top

C#:   "第一行\n第二行"
来源：http://oni.birdmap.top

[A14] 注释写法
来源：http://ubk.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uqr.zhiwuduotai.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tky.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://oiv.fengsongda.top

TS:   // 单行；/* 多行 */
来源：http://zrr.cucudq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qpo.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://hkh.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://srs.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://zlw.pycfn.com

[A15] 空值判断与默认值
来源：http://pmi.haohaochexian.top

Py:   value = data or "默认值"
来源：http://ijw.cdnleiting.top

PHP:  $value = $data ?? "默认值";
来源：http://kxj.sysykeji.top

JS:   const value = data ?? "默认值";
来源：http://vai.sxryk.cn

TS:   const value = data ?? "默认值";
来源：http://gkb.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://snt.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://cur.fanxiaobao.xyz

Ruby: value = data || "默认值"
来源：http://mcr.jinqigfzy.top

C#:   var value = data ?? "默认值";
来源：http://bxz.yj20258888.top

[A16] 真假值判断规则
来源：http://xpy.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fey.yfazqb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kpn.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gsa.dashuyun.cn

TS:   if (!x) {}
来源：http://ykn.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bpe.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ueg.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://ihj.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mhd.yj20258888.top

[A17] 位运算
来源：http://deg.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sky.yvedp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://flc.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ung.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://akz.dashuyun.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hrf.quarkkingdee.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mib.guannengcc.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kgv.cashguo.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzg.yuxming.cn

[A18] 字符与 ASCII 码互转
来源：http://cjl.bjfxy.top

Py:   ord("A"); chr(65)
来源：http://zqa.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://sor.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mst.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uxh.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://ftc.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ynh.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://epk.hongshengwenyu.top

C#:   (int)'A'; (char)65
来源：http://hfn.yfazqb.com

[A19] 交换两个变量
来源：http://iem.shuidangran.top

Py:   a, b = b, a
来源：http://pup.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nqx.fanxiaobao.xyz

JS:   [a, b] = [b, a];
来源：http://pyy.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://odj.aizwys.cn

Java: int t = a; a = b; b = t;
来源：http://vjm.jyoumei.cn

Go:   a, b = b, a
来源：http://sgn.xingfuxueyuan.xyz

Ruby: a, b = b, a
来源：http://xpu.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://odh.pycfn.com

[A20] 读取标准输入
来源：http://olg.havefunace.top

Py:   name = input("请输入：")
来源：http://tjq.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xhn.aibaodan.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vrs.nwbrower.top

TS:   // Node.js：readline 模块
来源：http://abt.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://wbw.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://myl.ydjk.org.cn

Ruby: gets.chomp
来源：http://qfs.birdmap.top

C#:   Console.ReadLine();
来源：http://ugr.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://mky.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://zrj.snrcjt.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ggo.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://zpc.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://not.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://tto.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tmo.yfazqb.com

Ruby: format("%.2f", 3.14159)
来源：http://flq.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://oca.yj20258888.top

[A22] 获取字符串长度
来源：http://dgk.jiagoushi.top

Py:   len(s)
来源：http://bvk.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bfj.yongpay.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fhz.xuanzx.com

TS:   s.length
来源：http://nxf.316326.xyz

Java: s.length()
来源：http://wcg.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fnk.c1oappe.top

Ruby: s.length
来源：http://yqa.aizwys.cn

C#:   s.Length
来源：http://lif.pycfn.com

[A23] 大小写转换
来源：http://aea.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ysa.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qpp.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rja.sjlbkw.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cbx.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dsm.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fgw.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jas.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://xov.9152youxi.cn

[A24] 去除首尾空白
来源：http://ohh.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://icp.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uje.cucudq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fli.cqqwz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pdf.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sdl.aizwys.cn

Go:   strings.TrimSpace(s)
来源：http://odq.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://svc.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qjf.quarkkingdee.top

[A25] 字符串比较
来源：http://rvq.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://roa.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zmn.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://djo.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ctz.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ggy.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cpn.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bzw.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bse.0kj1m.cn

[A26] 类型转换总览
来源：http://qie.wangdashe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ytj.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kef.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://swb.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://cyj.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pzv.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ndw.jinqigufen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tny.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hsw.ybcxt.top

================================================================================
来源：http://mqj.sweek.top

B. 流程控制
来源：http://tlv.316326.xyz

================================================================================
来源：http://rsu.pycfn.com

[B01] 条件判断 if / else
来源：http://sjr.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tpj.yuxming.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://why.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vmq.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fhw.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dyi.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vqo.zhaomingkeji.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mna.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hhf.wangdashe.top

[B02] 多分支 else if / elif
来源：http://nni.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jnj.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xju.ppjwa.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tof.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jro.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vuv.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zlv.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kkb.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqg.ydjk.org.cn

[B03] switch / match / case
来源：http://gni.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ror.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vcp.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hcq.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ria.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zsa.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wam.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qww.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kdc.chenjidiqi.icu

[B04] for 计数循环
来源：http://pwn.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://dgj.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gly.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hlb.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jrh.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pyp.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ras.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://den.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rvf.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://grg.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://pus.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://odn.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ahr.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://jek.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://kdp.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ljj.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://kry.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rae.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://dzh.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://npz.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sms.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yjz.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://muu.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://edg.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kek.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wgy.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gwn.quarkkingdee.top

[B07] while 循环
来源：http://enp.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://wjq.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://pfe.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://fod.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://ogn.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://eie.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tkz.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://jms.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://vkz.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://uku.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://evi.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oyc.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://lox.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://baa.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://zwa.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xwu.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://okc.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://izr.sufxvd.cn


<!-- 参考信息 -->