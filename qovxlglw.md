代发 wailian999

Ruby: PI = 3.14159
来源：http://dhg.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://gjc.jinghuilouyu.cn

[A04] 判断变量类型
来源：http://kvv.cqqwz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yqi.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vqu.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ygr.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://vdi.nanxinkj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xfd.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://jty.hammf.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mwt.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://evn.aibaodan.cn

[A05] 整数除法与取模
来源：http://vba.jinqigufen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nsg.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://owg.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zvx.pengpengdd.cyou

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sbo.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://qpe.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://mbo.shanyushiyangtech.top

Ruby: 7 / 2; 7 % 2
来源：http://jcn.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://hhf.gzhubu.top

[A06] 字符串转数字
来源：http://dvf.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://mbu.vehdjk.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eeq.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cqs.smart0.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://vuo.yj20258.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hpo.shuidangran.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oci.jinghuilouyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nwm.vehdjk.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mub.yfazqb.com

[A07] 数字转字符串
来源：http://dcw.zdqjudy.top

Py:   str(42)
来源：http://cth.cheryme.top

PHP:  (string) 42; strval(42)
来源：http://xeq.ivvv.top

JS:   String(42); (42).toString()
来源：http://qrq.tanke756.top

TS:   String(42)
来源：http://zdn.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dcs.hesvh.cn

Go:   strconv.Itoa(42)
来源：http://lpv.ivvv.top

Ruby: 42.to_s
来源：http://omz.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://siu.pycfn.com

[A08] 取整与四舍五入
来源：http://ajk.yj20258888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pfk.tianlin.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fqq.zhaomingkeji.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://joy.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lvy.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fmb.xuetiantiany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jxp.havefunace.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qvf.smart0.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ida.sweek.top

[A09] 绝对值与最大最小值
来源：http://nna.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tdz.tanke756.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fki.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pyd.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wde.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lmr.dashuyun.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lka.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qft.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bxz.epnwcf.com

[A10] 生成随机数
来源：http://mdm.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://dqe.hnxiangtu.top

PHP:  random_int(1, 100);
来源：http://weq.zhaomingkeji.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cbk.iojbl.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bsv.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://ptt.fzhhl.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tis.cdnleiting.top

Ruby: rand(1..100)
来源：http://gsm.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://xyo.zhijiandao.cn

[A11] 条件表达式（三元）
来源：http://jvf.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://qrf.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tef.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://vhp.hongshengwenyu.top

TS:   x > 0 ? "yes" : "no"
来源：http://ehp.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://uqb.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hio.jlsjyb.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ukj.fehbvm.com

C#:   x > 0 ? "yes" : "no"
来源：http://xnr.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://gpw.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nrb.hnqzz.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ico.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://epi.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://opa.52xcode.cn

Java: "Hello, %s!".formatted(name)
来源：http://mta.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://owg.hcnkem.com

Ruby: "Hello, #{name}!"
来源：http://ybt.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://itu.yvedp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ixa.xinyue.icu

Py:   "第一行\n第二行"
来源：http://xft.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://kgz.zycfv.cn

JS:   "第一行\n第二行"
来源：http://vac.fengsongda.top

TS:   "第一行\n第二行"
来源：http://phe.yfazqb.com

Java: "第一行\n第二行"
来源：http://qze.vqdsnc.cn

Go:   "第一行\n第二行"
来源：http://cus.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://nod.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://mhs.xylfe.cn

[A14] 注释写法
来源：http://mpe.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://utc.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xwe.sxryk.cn

JS:   // 单行；/* 多行 */
来源：http://rbg.0kj1m.cn

TS:   // 单行；/* 多行 */
来源：http://yqt.tarul.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fde.uphjek.com

Go:   // 单行；/* 多行 */
来源：http://yid.sufxvd.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qtl.kuanghao11.cn

C#:   // 单行；/* 多行 */
来源：http://idj.svipenyu.cn

[A15] 空值判断与默认值
来源：http://ifp.jlsjyb.cn

Py:   value = data or "默认值"
来源：http://zzf.tian-w.cn

PHP:  $value = $data ?? "默认值";
来源：http://lrg.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://xsv.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://wsr.bbcook.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zjp.yanxiufei.cn

Go:   if data == "" { data = "默认值" }
来源：http://gkr.birdmap.top

Ruby: value = data || "默认值"
来源：http://byu.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://zwf.birdmap.top

[A16] 真假值判断规则
来源：http://khx.jlsjyb.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://csd.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nlx.zhaomingkeji.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ngd.yonumen.top

TS:   if (!x) {}
来源：http://ewp.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qjx.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yil.hywenlv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ypq.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dcr.yongpay.top

[A17] 位运算
来源：http://kfc.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rvm.andypj.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://owe.daxiang520.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://stg.nanxuanxn.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dsb.quarkkingdee.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://weg.cashguo.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://seo.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxr.cheryme.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gki.andypj.xyz

[A18] 字符与 ASCII 码互转
来源：http://jbj.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://uzn.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://hbr.yfazqb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jze.wangshuangyany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gdl.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://knx.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://akg.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://bnz.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://bkv.gzhubu.top

[A19] 交换两个变量
来源：http://cmr.yongpay.top

Py:   a, b = b, a
来源：http://lad.zycfv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tus.sweek.top

JS:   [a, b] = [b, a];
来源：http://ddh.yonumen.top

TS:   [a, b] = [b, a];
来源：http://col.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://bcd.ydzc1.top

Go:   a, b = b, a
来源：http://moe.hywenlv.cn

Ruby: a, b = b, a
来源：http://tez.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://yao.fehbvm.com

[A20] 读取标准输入
来源：http://jtn.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://ude.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ori.jlsjyb.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cqj.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://wlu.jyoumei.cn

Java: new Scanner(System.in).nextLine()
来源：http://obp.hfpthk.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yds.sweek.top

Ruby: gets.chomp
来源：http://mgi.pengpengdd.cyou

C#:   Console.ReadLine();
来源：http://eob.zycfv.cn

[A21] 保留指定小数位输出
来源：http://itz.aizwys.cn

Py:   f"{3.14159:.2f}"
来源：http://jhr.jqgufenzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ysy.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://dcs.yueranfly.top

TS:   (3.14159).toFixed(2)
来源：http://wao.feifeiyinyue.top

Java: String.format("%.2f", 3.14159)
来源：http://emx.cashguo.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://udw.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://bbh.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://wrz.gogol.net.cn

[A22] 获取字符串长度
来源：http://lpe.yj202588.top

Py:   len(s)
来源：http://xcq.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kgd.chenlongwang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dun.smart0.xyz

TS:   s.length
来源：http://ant.ivvv.top

Java: s.length()
来源：http://ogx.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ows.haohaochexian.top

Ruby: s.length
来源：http://wsw.cdnleiting.top

C#:   s.Length
来源：http://bzx.tianlin.xyz

[A23] 大小写转换
来源：http://cwg.havefunace.top

Py:   s.upper(); s.lower(); s.title()
来源：http://uub.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://moy.yj20258.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://stk.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nia.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lru.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hfo.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vkc.hammf.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gil.9152youxi.cn

[A24] 去除首尾空白
来源：http://byr.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ajn.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://owj.cdnleiting.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cac.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zld.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qev.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://iso.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ksa.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tgw.mhx1999.top

[A25] 字符串比较
来源：http://lqk.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://gus.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yzw.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://knh.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aez.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gzj.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ioz.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wgc.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kgm.xuetiantiany.cn

[A26] 类型转换总览
来源：http://sqr.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hjd.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://csa.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://olk.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://njm.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qzj.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ndk.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://plt.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hii.jqgufenzy.top

================================================================================
来源：http://vmq.ydjk.org.cn

B. 流程控制
来源：http://rfb.sysykeji.top

================================================================================
来源：http://tnb.smart0.xyz

[B01] 条件判断 if / else
来源：http://odx.shangyingyoupin.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wmg.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wjy.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://liv.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jjz.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jge.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lig.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mun.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rha.zycfv.cn

[B02] 多分支 else if / elif
来源：http://pou.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zox.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rph.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqn.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sax.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fdp.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cop.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cct.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjq.haohaochexian.top

[B03] switch / match / case
来源：http://cka.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aej.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hlo.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jsd.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hvt.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jzc.ctjpmb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ksh.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oyx.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wzl.9152youxi.cn

[B04] for 计数循环
来源：http://qwg.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://zbj.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bjm.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gqd.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qzm.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yvc.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fsq.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://xwb.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rbh.yj202588.top

[B05] 遍历数组 / 列表
来源：http://zcm.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://xny.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vsl.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://ike.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://wws.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mgb.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qmg.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://qeq.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qit.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://hlj.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xvm.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ouq.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qax.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kbu.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ayz.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://twu.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cgz.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uhf.fehbvm.com

[B07] while 循环
来源：http://yzb.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://ixc.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ljs.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://ixc.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://jta.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://wjo.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ody.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://lwm.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://pgg.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://aqs.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://jmk.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://brv.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://ncc.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://von.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://tli.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ksl.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://ewy.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://vgv.bjfxy.top

[B09] break 与 continue
来源：http://duk.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iea.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mgw.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dro.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzx.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddo.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xte.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xob.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqd.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://bvn.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wod.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sqc.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mtm.yuanzhike.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ynh.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tgf.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ejy.nanxinkj.top


<!-- 参考信息 -->