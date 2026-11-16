代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://rkg.dashuyun.cn

Go:   fmt.Println("Hello, World!")
来源：http://mek.hfpthk.cn

Ruby: puts "Hello, World!"
来源：http://ajg.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fhd.ydjk.org.cn

[A02] 变量声明与赋值
来源：http://fmt.zhijiandao.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xsg.cqqwz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aoo.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vrh.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xul.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://jms.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://rpg.gzhubu.top

Ruby: name = "Alex"; age = 20
来源：http://lsj.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://psb.daxiang520.top

[A03] 常量定义
来源：http://lqo.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yyo.yongpay.top

PHP:  const PI = 3.14159;
来源：http://smq.shanyushiyangtech.top

JS:   const PI = 3.14159;
来源：http://dqo.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://qlu.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://rfa.zycfv.cn

Go:   const PI = 3.14159
来源：http://mff.hcnkem.com

Ruby: PI = 3.14159
来源：http://yas.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://hjk.tarul.cn

[A04] 判断变量类型
来源：http://nwy.feifeiyinyue.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kki.gotoacloud.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fgf.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jyl.ivvv.top

TS:   typeof x; x instanceof Date
来源：http://gol.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bgt.sxryk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ypm.nanxinkj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gpj.ehwqpu.com

C#:   x.GetType().Name; x is int
来源：http://rxq.jyoumei.cn

[A05] 整数除法与取模
来源：http://yhj.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qyz.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wmm.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dgt.sxryk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qul.tian-w.cn

Java: 7 / 2; 7 % 2
来源：http://aev.zhengqikj.top

Go:   7 / 2; 7 % 2
来源：http://lqy.zycfv.cn

Ruby: 7 / 2; 7 % 2
来源：http://fby.aizwys.cn

C#:   7 / 2; 7 % 2
来源：http://pbu.jqgufenzy.top

[A06] 字符串转数字
来源：http://bje.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://pyd.yangfankeji.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nhb.tian-w.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://enx.shzxlz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ywp.ydzc1.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jef.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://txc.andypj.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://ocg.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ehv.xylfe.cn

[A07] 数字转字符串
来源：http://ezb.52xcode.cn

Py:   str(42)
来源：http://rob.cqqwz.cn

PHP:  (string) 42; strval(42)
来源：http://usm.jiagoushi.top

JS:   String(42); (42).toString()
来源：http://hge.uphjek.com

TS:   String(42)
来源：http://puh.yj20258888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uel.wangdashe.top

Go:   strconv.Itoa(42)
来源：http://yor.zdqjudy.top

Ruby: 42.to_s
来源：http://fqn.zhixingplan.top

C#:   42.ToString()
来源：http://gyc.yfazqb.com

[A08] 取整与四舍五入
来源：http://wrn.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uhf.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ahg.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://acl.hesvh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jgf.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ouk.jqgufenzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qwk.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://let.ywan-chungtsiang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://weg.yvedp.cn

[A09] 绝对值与最大最小值
来源：http://los.9152youxi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://onl.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ksu.jiagoushi.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sms.yj20258.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tla.smart0.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tuj.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hng.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yif.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vvq.andypj.xyz

[A10] 生成随机数
来源：http://uan.zhijiandao.cn

Py:   import random; random.randint(1, 100)
来源：http://qgr.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://snn.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jtk.meibo888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kmw.zhengqikj.top

Java: new Random().nextInt(100) + 1
来源：http://bvt.hcnkem.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lqv.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://brm.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://fzr.zhaomingkeji.xyz

[A11] 条件表达式（三元）
来源：http://nna.daxiang520.top

Py:   "yes" if x > 0 else "no"
来源：http://blw.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gfb.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vvf.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://ycp.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://ohy.hnxiangtu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xwy.tian-w.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jqd.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ywd.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://axi.ivvv.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://smy.cqqwz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qis.hongshengwenyu.top

JS:   `Hello, ${name}!`
来源：http://ovx.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://swd.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://hym.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kdb.ywan-chungtsiang.top

Ruby: "Hello, #{name}!"
来源：http://pxn.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://gie.jiagoushi.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gfr.hfpthk.cn

Py:   "第一行\n第二行"
来源：http://aey.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://ugw.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://ebt.hywenlv.cn

TS:   "第一行\n第二行"
来源：http://jrh.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://qeo.pycfn.com

Go:   "第一行\n第二行"
来源：http://xlh.yj20258888.top

Ruby: "第一行\n第二行"
来源：http://veg.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://ldx.meibo888.top

[A14] 注释写法
来源：http://bvr.wangdashe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://sqg.bbcook.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xqc.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://tak.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://abj.nwbrower.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rll.zhengqikj.top

Go:   // 单行；/* 多行 */
来源：http://vyv.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mrf.tian-w.cn

C#:   // 单行；/* 多行 */
来源：http://wdk.chenlongwang.top

[A15] 空值判断与默认值
来源：http://hjx.jinqigufen.top

Py:   value = data or "默认值"
来源：http://nsk.mhx1999.top

PHP:  $value = $data ?? "默认值";
来源：http://aac.yj20258.top

JS:   const value = data ?? "默认值";
来源：http://rwu.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://sgd.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tof.cheryme.top

Go:   if data == "" { data = "默认值" }
来源：http://hak.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://oxk.snrcjt.cn

C#:   var value = data ?? "默认值";
来源：http://xjc.fktsv.cn

[A16] 真假值判断规则
来源：http://pad.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mfu.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mzc.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mtm.xinyue.icu

TS:   if (!x) {}
来源：http://aat.pengpengdd.cyou

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ebg.yj202588.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://faw.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://csy.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aov.hysaishi.cn

[A17] 位运算
来源：http://jja.havefunace.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://abo.nanxuanxn.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rff.gogol.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aeo.guannengcc.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uhb.jqgfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zgl.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kkj.cdnleiting.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ruw.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dgu.quarkkingdee.top

[A18] 字符与 ASCII 码互转
来源：http://mul.sysykeji.top

Py:   ord("A"); chr(65)
来源：http://aeu.hesvh.cn

PHP:  ord("A"); chr(65)
来源：http://xcf.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ohn.ybcxt.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ebq.hnxiangtu.top

Java: (int) 'A'; (char) 65
来源：http://diz.sysykeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://urf.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://osh.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://vkq.jiagoushi.top

[A19] 交换两个变量
来源：http://ues.gzhubu.top

Py:   a, b = b, a
来源：http://euh.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://yej.ivvv.top

JS:   [a, b] = [b, a];
来源：http://cxk.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://skz.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://fwj.cashguo.top

Go:   a, b = b, a
来源：http://big.xziqi.cn

Ruby: a, b = b, a
来源：http://nyw.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://csm.gogol.net.cn

[A20] 读取标准输入
来源：http://cfc.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://dps.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vzh.bjfxy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fdo.shzxlz.cn

TS:   // Node.js：readline 模块
来源：http://omb.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://wdk.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kau.hfpthk.cn

Ruby: gets.chomp
来源：http://cwp.gogol.net.cn

C#:   Console.ReadLine();
来源：http://fjr.xinyue.icu

[A21] 保留指定小数位输出
来源：http://iku.xingfuxueyuan.xyz

Py:   f"{3.14159:.2f}"
来源：http://nxw.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jqf.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://hrs.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://oev.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://hwx.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zfo.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://axo.sweek.top

C#:   3.14159.ToString("F2")
来源：http://ikz.dashuyun.cn

[A22] 获取字符串长度
来源：http://eyh.zdqjudy.top

Py:   len(s)
来源：http://lbr.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oxr.hysaishi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tbp.ydjk.org.cn

TS:   s.length
来源：http://umy.epnwcf.com

Java: s.length()
来源：http://kei.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tsv.nanxuanxn.top

Ruby: s.length
来源：http://mne.cdnleiting.top

C#:   s.Length
来源：http://bda.yuxming.cn

[A23] 大小写转换
来源：http://tkc.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://boo.vqdsnc.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vxj.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zkb.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ksm.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bnc.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hpv.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://geq.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://cuo.gogol.net.cn

[A24] 去除首尾空白
来源：http://dpm.yueranfly.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jwq.ppjwa.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://moi.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qgs.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gkk.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xio.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://giw.hcnkem.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ysc.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hro.hesvh.cn

[A25] 字符串比较
来源：http://zzf.gotoacloud.top

Py:   s1 == s2; s1 != s2
来源：http://hnm.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sgp.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jmw.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwu.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kkv.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uer.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://juy.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://les.nanxuanxn.top

[A26] 类型转换总览
来源：http://kol.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://whu.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kna.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ead.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://zpp.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hst.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mnw.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ezn.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://afj.ivvv.top

================================================================================
来源：http://yhu.svipenyu.cn

B. 流程控制
来源：http://jud.hnqzz.top

================================================================================
来源：http://snz.ppjwa.cn

[B01] 条件判断 if / else
来源：http://lml.fktsv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://coq.zdbjq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lim.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cem.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fbe.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kft.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xly.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qwj.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://com.fengsongda.top

[B02] 多分支 else if / elif
来源：http://bjp.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wbh.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pgk.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppv.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cay.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyn.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lgj.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://avy.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqs.ppjwa.cn

[B03] switch / match / case
来源：http://spw.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bsl.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dwx.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ykk.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lmf.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ece.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://las.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ads.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pfb.ydjk.org.cn

[B04] for 计数循环
来源：http://bxb.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://kqi.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kdu.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rxl.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jkf.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://egh.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ura.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://oes.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iwd.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://xyq.yj202588.top

Py:   for item in arr: print(item)
来源：http://yry.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://opb.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pez.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nuf.aizwys.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vry.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tan.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://bus.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oys.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://xyy.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yzq.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hzg.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hhm.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ciw.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://moc.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cvw.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rmi.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dzb.vehdjk.com

[B07] while 循环
来源：http://rvp.yj202588.top

Py:   while i < 10: i += 1
来源：http://caq.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://psu.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://nzm.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://ajl.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://wtj.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dle.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://pkk.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://kwy.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://csu.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://bja.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zel.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://zzg.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://ylj.sjlbkw.cn


<!-- 参考信息 -->