代发 wailian999

JS:   const PI = 3.14159;
来源：http://yhf.hammf.cn

TS:   const PI: number = 3.14159;
来源：http://xrd.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://xmw.sweek.top

Go:   const PI = 3.14159
来源：http://app.hammf.cn

Ruby: PI = 3.14159
来源：http://ozv.fktsv.cn

C#:   const double PI = 3.14159;
来源：http://yzt.gogol.net.cn

[A04] 判断变量类型
来源：http://amv.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cup.redwolf501.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mwl.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://exx.zhiwuduotai.top

TS:   typeof x; x instanceof Date
来源：http://nmt.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lwl.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://mdc.nanxinkj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jld.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://hpg.vqdsnc.cn

[A05] 整数除法与取模
来源：http://xzi.ehwqpu.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tuz.c1oappe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bea.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qyg.yueranfly.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bzh.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://ewn.birdmap.top

Go:   7 / 2; 7 % 2
来源：http://gzj.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://voz.ppjwa.cn

C#:   7 / 2; 7 % 2
来源：http://diu.fzhhl.top

[A06] 字符串转数字
来源：http://cgh.yvedp.cn

Py:   int("42"); float("3.14")
来源：http://ioe.hongshengwenyu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://juz.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wge.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://aoo.jianghu66.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ngh.hysaishi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jdz.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://sie.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pnw.daria6918.cn

[A07] 数字转字符串
来源：http://ylh.cucudq.cn

Py:   str(42)
来源：http://jjd.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://evg.0kj1m.cn

JS:   String(42); (42).toString()
来源：http://ezg.tanke756.top

TS:   String(42)
来源：http://lbg.jqgufenzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vbf.hnqzz.top

Go:   strconv.Itoa(42)
来源：http://rae.ehwqpu.com

Ruby: 42.to_s
来源：http://jqh.svipenyu.cn

C#:   42.ToString()
来源：http://jow.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://zwn.dianchejie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kqy.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rkv.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oih.daria6918.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://omp.guowangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xgj.zdbjq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zak.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cik.guannengcc.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zsk.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://qjx.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://niu.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ryi.uphjek.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://slf.guannengcc.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://one.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ybk.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yls.hnqzz.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zjx.quarkkingdee.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hzq.jinqigufen.top

[A10] 生成随机数
来源：http://lvq.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://ikf.ivvv.top

PHP:  random_int(1, 100);
来源：http://tbv.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://goh.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lfq.hnxiangtu.top

Java: new Random().nextInt(100) + 1
来源：http://wqy.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ihm.feifeiyinyue.top

Ruby: rand(1..100)
来源：http://bgy.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://vll.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://xai.haohaochexian.top

Py:   "yes" if x > 0 else "no"
来源：http://woh.andypj.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://erk.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://oks.xylfe.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kry.tarul.cn

Java: x > 0 ? "yes" : "no"
来源：http://mdi.vehdjk.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ufo.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bxm.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://mcp.ydjk.org.cn

[A12] 字符串插值 / 格式化
来源：http://jri.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rzf.vehdjk.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jwe.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://fks.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://wnx.guowangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://hie.svipenyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zqr.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://cez.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://ywb.meibo888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ygn.zycfv.cn

Py:   "第一行\n第二行"
来源：http://wld.smart0.xyz

PHP:  "第一行\n第二行"
来源：http://hit.snrcjt.cn

JS:   "第一行\n第二行"
来源：http://dia.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://qox.ybcxt.top

Java: "第一行\n第二行"
来源：http://nmt.yj20258888.top

Go:   "第一行\n第二行"
来源：http://sky.yuxming.cn

Ruby: "第一行\n第二行"
来源：http://nhk.guannengcc.top

C#:   "第一行\n第二行"
来源：http://gcb.yvedp.cn

[A14] 注释写法
来源：http://ybp.jiagoushi.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gch.hcnkem.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://hvb.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://qfz.jqgfzy.top

TS:   // 单行；/* 多行 */
来源：http://jvv.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://led.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://fvk.yonumen.top

Ruby: # 单行；=begin 多行 =end
来源：http://jbk.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://jgz.daria6918.cn

[A15] 空值判断与默认值
来源：http://msv.52xcode.cn

Py:   value = data or "默认值"
来源：http://gxz.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://yxw.zhengqikj.top

JS:   const value = data ?? "默认值";
来源：http://iiq.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://fsq.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://isf.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://edo.yongpay.top

Ruby: value = data || "默认值"
来源：http://bxb.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://wdj.mhx1999.top

[A16] 真假值判断规则
来源：http://jef.yongpay.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hmv.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wal.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fgo.meibo888.top

TS:   if (!x) {}
来源：http://aqh.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ztq.gogol.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bsa.316326.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://lbo.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mfk.gzhubu.top

[A17] 位运算
来源：http://fws.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nmb.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lxk.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjl.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jes.snrcjt.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fdw.gotoacloud.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kei.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxe.chenlongwang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xdp.jyoumei.cn

[A18] 字符与 ASCII 码互转
来源：http://akp.ppjwa.cn

Py:   ord("A"); chr(65)
来源：http://zsi.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://pvy.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lbc.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lcc.zhijiandao.cn

Java: (int) 'A'; (char) 65
来源：http://gnt.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://awd.yuxming.cn

Ruby: "A".ord; 65.chr
来源：http://jip.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://gpl.hysaishi.cn

[A19] 交换两个变量
来源：http://hub.hfpthk.cn

Py:   a, b = b, a
来源：http://zem.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tir.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://sdg.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://nlr.yongpay.top

Java: int t = a; a = b; b = t;
来源：http://pfp.andypj.xyz

Go:   a, b = b, a
来源：http://siv.yueranfly.top

Ruby: a, b = b, a
来源：http://hng.smart0.xyz

C#:   (a, b) = (b, a);
来源：http://eng.zycfv.cn

[A20] 读取标准输入
来源：http://apt.hysaishi.cn

Py:   name = input("请输入：")
来源：http://lat.jinqigfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rjh.sweek.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sxf.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://gts.nanxinkj.top

Java: new Scanner(System.in).nextLine()
来源：http://bjt.nwbrower.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ndq.kuanghao11.cn

Ruby: gets.chomp
来源：http://whz.hesvh.cn

C#:   Console.ReadLine();
来源：http://yvq.vehdjk.com

[A21] 保留指定小数位输出
来源：http://qlw.sxryk.cn

Py:   f"{3.14159:.2f}"
来源：http://sre.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aik.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://sll.zhijiandao.cn

TS:   (3.14159).toFixed(2)
来源：http://pic.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://bvz.aizwys.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://efx.yj20258.top

Ruby: format("%.2f", 3.14159)
来源：http://dpp.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://jbp.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://uqb.ywan-chungtsiang.top

Py:   len(s)
来源：http://fin.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://apg.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bhg.zdqjudy.top

TS:   s.length
来源：http://eju.havefunace.top

Java: s.length()
来源：http://exu.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://epy.jinyuanbaomall.cn

Ruby: s.length
来源：http://fqq.jyoumei.cn

C#:   s.Length
来源：http://ptw.hammf.cn

[A23] 大小写转换
来源：http://fxb.nanxuanxn.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ymq.shangyingyoupin.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tfs.tanke756.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bfm.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://txn.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mey.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dpt.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bsd.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ugg.zycfv.cn

[A24] 去除首尾空白
来源：http://pkj.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ujw.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://orr.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lct.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dly.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ziq.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://miz.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cmv.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kcn.sjlbkw.cn

[A25] 字符串比较
来源：http://ojj.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://yet.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nxh.tianlin.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bpd.ydzc1.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tmx.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dqh.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iyb.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zdb.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nvx.smart0.xyz

[A26] 类型转换总览
来源：http://inl.hcnkem.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sxu.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zqj.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://itq.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://udk.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hlt.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xbv.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sdr.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ilj.aizwys.cn

================================================================================
来源：http://zsk.tian-w.cn

B. 流程控制
来源：http://nfr.cdnleiting.top

================================================================================
来源：http://nao.tian-w.cn

[B01] 条件判断 if / else
来源：http://fie.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zed.c1oappe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cwa.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xay.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ijn.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gso.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lre.zdbjq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eow.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pnf.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://jrh.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://svr.chenlongwang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dpt.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dlz.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dse.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lga.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yki.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wzn.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rng.aibaodan.cn

[B03] switch / match / case
来源：http://rvy.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://upo.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vpm.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wlm.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tqx.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://guo.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cmy.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sdc.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pbd.smart0.xyz

[B04] for 计数循环
来源：http://kxd.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://ton.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jxm.yj20258.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mbu.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://szf.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ddv.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cee.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://zdz.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xex.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://zek.aizwys.cn

Py:   for item in arr: print(item)
来源：http://ofs.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vve.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://odb.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://edu.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qot.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mzk.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://oez.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xxe.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://rpw.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kpn.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fny.pengpengdd.cyou

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tfv.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gpm.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wtm.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zri.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gxu.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tgt.guannengcc.top

[B07] while 循环
来源：http://ubd.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://oxr.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://rpw.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://rvs.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://iuu.havefunace.top

Java: while (i < 10) { i++; }
来源：http://ndq.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cok.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://quj.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://cma.uphjek.com

[B08] do-while（至少执行一次）
来源：http://jew.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://bto.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://eqd.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://nbt.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://zyy.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://ypb.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ffc.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://khi.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://iuy.hcnkem.com

[B09] break 与 continue
来源：http://asi.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ogt.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dxn.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyq.snrcjt.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vxv.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uom.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ktt.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bdt.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpz.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://ldq.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nnu.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qdu.ctjpmb.com


<!-- 参考信息 -->