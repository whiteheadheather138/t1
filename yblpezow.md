代发 wailian999

Ruby: PI = 3.14159
来源：http://bcl.yvedp.cn

C#:   const double PI = 3.14159;
来源：http://gra.shuidangran.top

[A04] 判断变量类型
来源：http://ntx.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://xsc.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mgc.cashguo.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://peb.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://ndh.nwbrower.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tgc.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://azf.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://qzc.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://ska.xuetiantiany.cn

[A05] 整数除法与取模
来源：http://dtc.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jux.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xsa.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aij.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kgj.sweek.top

Java: 7 / 2; 7 % 2
来源：http://zvk.xziqi.cn

Go:   7 / 2; 7 % 2
来源：http://jdk.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://gnw.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://jzs.guowangkeji.top

[A06] 字符串转数字
来源：http://cha.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://sci.fehbvm.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cfr.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dix.meibo888.top

TS:   parseInt("42", 10); Number("42")
来源：http://jey.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wzx.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qbz.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://zys.zhaomingkeji.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gtu.xylfe.cn

[A07] 数字转字符串
来源：http://ptu.0kj1m.cn

Py:   str(42)
来源：http://bmw.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://jey.cucudq.cn

JS:   String(42); (42).toString()
来源：http://xae.chenzaomai.com

TS:   String(42)
来源：http://yhb.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://bbm.gogol.net.cn

Go:   strconv.Itoa(42)
来源：http://rdh.c1oappe.top

Ruby: 42.to_s
来源：http://bqf.wangdashe.top

C#:   42.ToString()
来源：http://nmy.dianchejie.cn

[A08] 取整与四舍五入
来源：http://lls.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dcg.yuxming.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pdh.316326.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vbb.tianlin.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uvw.yfazqb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://shs.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ohk.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://pju.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xiy.zhiwuduotai.top

[A09] 绝对值与最大最小值
来源：http://vyi.jqgufenzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wzq.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lnj.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zge.yuanzhike.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nzc.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qdy.xuetiantiany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dqk.zdqjudy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://omr.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rhq.nanxinkj.top

[A10] 生成随机数
来源：http://civ.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://iob.fehbvm.com

PHP:  random_int(1, 100);
来源：http://xmt.xinyue.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nvr.yuanzhike.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qkr.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://aks.sweek.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ngr.cashguo.top

Ruby: rand(1..100)
来源：http://dct.xylfe.cn

C#:   new Random().Next(1, 101)
来源：http://nfx.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://jvu.uphjek.com

Py:   "yes" if x > 0 else "no"
来源：http://qss.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ifn.zhaomingkeji.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://fnx.yuanzhike.top

TS:   x > 0 ? "yes" : "no"
来源：http://jyz.ybcxt.top

Java: x > 0 ? "yes" : "no"
来源：http://svc.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hix.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bty.chenzaomai.com

C#:   x > 0 ? "yes" : "no"
来源：http://kdi.ybcxt.top

[A12] 字符串插值 / 格式化
来源：http://cyd.chenlongwang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ifv.smart0.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pik.cheryme.top

JS:   `Hello, ${name}!`
来源：http://pue.tarul.cn

TS:   `Hello, ${name}!`
来源：http://gfw.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://fsu.tarul.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cvp.cdnleiting.top

Ruby: "Hello, #{name}!"
来源：http://uhg.ehwqpu.com

C#:   $"Hello, {name}!"
来源：http://run.tianlin.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://ztd.tianlin.xyz

Py:   "第一行\n第二行"
来源：http://pro.yj20258.top

PHP:  "第一行\n第二行"
来源：http://rgs.316326.xyz

JS:   "第一行\n第二行"
来源：http://zld.yj202588.top

TS:   "第一行\n第二行"
来源：http://wpx.gogol.net.cn

Java: "第一行\n第二行"
来源：http://xnr.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://qzh.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://uwt.cheryme.top

C#:   "第一行\n第二行"
来源：http://drz.zhengqikj.top

[A14] 注释写法
来源：http://iln.xingfuxueyuan.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://ztl.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gmc.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://nzy.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://ert.zdqjudy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fey.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://vfp.daria6918.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yst.hysaishi.cn

C#:   // 单行；/* 多行 */
来源：http://xyp.smart0.xyz

[A15] 空值判断与默认值
来源：http://wnr.gogol.net.cn

Py:   value = data or "默认值"
来源：http://gki.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://ryn.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://iqm.52xcode.cn

TS:   const value = data ?? "默认值";
来源：http://voh.zhaomingkeji.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bcq.haohaochexian.top

Go:   if data == "" { data = "默认值" }
来源：http://ghw.xylfe.cn

Ruby: value = data || "默认值"
来源：http://ttc.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://ajn.zhoulong.xyz

[A16] 真假值判断规则
来源：http://qnd.jinghuilouyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fyx.wangshuangyany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ukr.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mym.jqgfzy.top

TS:   if (!x) {}
来源：http://jqk.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dno.cucudq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nil.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://csb.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ylv.daria6918.cn

[A17] 位运算
来源：http://czg.shzxlz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dhc.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pvf.andypj.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://myu.zhixingplan.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aaq.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gie.tianlin.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dcd.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzd.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ano.jinqigufen.top

[A18] 字符与 ASCII 码互转
来源：http://yvf.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://xhx.shanyushiyangtech.top

PHP:  ord("A"); chr(65)
来源：http://hww.hfpthk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bhu.zhengqikj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ngt.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://qgf.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://knc.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://ktw.yvedp.cn

C#:   (int)'A'; (char)65
来源：http://czo.ywan-chungtsiang.top

[A19] 交换两个变量
来源：http://pqj.yvedp.cn

Py:   a, b = b, a
来源：http://flt.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://czc.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://vnb.hongshengwenyu.top

TS:   [a, b] = [b, a];
来源：http://eph.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://jyx.ydzc1.top

Go:   a, b = b, a
来源：http://jjl.zdbjq.cn

Ruby: a, b = b, a
来源：http://nlt.fktsv.cn

C#:   (a, b) = (b, a);
来源：http://wxf.nwbrower.top

[A20] 读取标准输入
来源：http://oof.quarkkingdee.top

Py:   name = input("请输入：")
来源：http://hcv.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gbc.jinghuilouyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xjk.ywan-chungtsiang.top

TS:   // Node.js：readline 模块
来源：http://zkj.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://gps.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jnj.dashuyun.cn

Ruby: gets.chomp
来源：http://sak.meibo888.top

C#:   Console.ReadLine();
来源：http://dew.pycfn.com

[A21] 保留指定小数位输出
来源：http://kwg.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://kfn.birdmap.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dpm.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://wyx.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://gbi.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://bmk.yj20258.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xud.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://ypm.yj202588.top

C#:   3.14159.ToString("F2")
来源：http://iuq.ppjwa.cn

[A22] 获取字符串长度
来源：http://pos.c1oappe.top

Py:   len(s)
来源：http://mgk.jinqigfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dxw.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://opb.zhixingplan.top

TS:   s.length
来源：http://zym.yj20258.top

Java: s.length()
来源：http://jjv.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eoc.ydjk.org.cn

Ruby: s.length
来源：http://xdu.jqgufenzy.top

C#:   s.Length
来源：http://kkc.dashuyun.cn

[A23] 大小写转换
来源：http://mvf.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ihr.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gdl.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pyx.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hnd.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://img.52xcode.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rwm.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lzo.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://elx.yj202588.top

[A24] 去除首尾空白
来源：http://aja.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lyg.nwbrower.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vph.jinqigfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zos.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ljy.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qvt.hfpthk.cn

Go:   strings.TrimSpace(s)
来源：http://bdk.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zdw.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://txt.zhoulong.xyz

[A25] 字符串比较
来源：http://hik.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://iso.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sqq.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pai.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://etx.yj20258.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jwq.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tgq.sweek.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dqb.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ivd.fzhhl.top

[A26] 类型转换总览
来源：http://wkr.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://spa.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kks.jinghuilouyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sfv.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://nso.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pnb.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yua.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sxe.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uei.sweek.top

================================================================================
来源：http://sgg.havefunace.top

B. 流程控制
来源：http://yty.shuidangran.top

================================================================================
来源：http://gvw.tianlin.xyz

[B01] 条件判断 if / else
来源：http://yma.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cxz.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zle.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lyo.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mua.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gyv.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tdd.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jcg.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ovo.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://bok.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ssr.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blc.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqz.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://age.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://htw.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aqc.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hym.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ooc.yongpay.top

[B03] switch / match / case
来源：http://kmv.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lkg.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uwc.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://omg.hammf.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqu.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kvf.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://maf.yongpay.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zhb.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tla.sjlbkw.cn

[B04] for 计数循环
来源：http://rvz.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://lgo.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://owc.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lrt.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjt.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jrz.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ofk.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://flr.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ccl.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://phf.yj20258.top

Py:   for item in arr: print(item)
来源：http://qlc.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://spi.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xvj.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fxf.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wqm.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vuz.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://rzq.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lst.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://djr.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wjd.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rij.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zsd.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mzt.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqi.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hor.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://msa.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vaw.jqgfzy.top

[B07] while 循环
来源：http://efg.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://ihr.jianghu66.top

PHP:  while ($i < 10) { $i++; }
来源：http://kpq.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://qhd.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://ibi.epnwcf.com

Java: while (i < 10) { i++; }
来源：http://kxv.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jjw.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://icp.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://tnr.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://gzl.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://oor.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://eof.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://hfr.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://ptu.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://dpd.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://wvf.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://amq.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://naj.guowangkeji.top

[B09] break 与 continue
来源：http://cnx.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fcl.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zko.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxu.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbw.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nbm.mhx1999.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qkl.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xkp.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://riy.yongpay.top

[B10] 遍历同时拿索引
来源：http://kbd.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gev.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vfi.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ehp.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ocv.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xmb.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yss.hnxiangtu.top


<!-- 参考信息 -->