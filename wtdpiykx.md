代发 wailian999

Ruby: PI = 3.14159
来源：http://xxu.jqgfzy.top

C#:   const double PI = 3.14159;
来源：http://iru.shangyingyoupin.top

[A04] 判断变量类型
来源：http://vot.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tka.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ghl.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yga.jinqigufen.top

TS:   typeof x; x instanceof Date
来源：http://xti.jiagoushi.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jdk.pycfn.com

Go:   reflect.TypeOf(x).Name()
来源：http://sft.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://syv.vqdsnc.cn

C#:   x.GetType().Name; x is int
来源：http://skp.jinqigfzy.top

[A05] 整数除法与取模
来源：http://amz.jqgfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gkx.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://kup.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nnt.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xfd.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://gqr.yongpay.top

Go:   7 / 2; 7 % 2
来源：http://ggl.nwbrower.top

Ruby: 7 / 2; 7 % 2
来源：http://ihd.tian-w.cn

C#:   7 / 2; 7 % 2
来源：http://muw.zycfv.cn

[A06] 字符串转数字
来源：http://pef.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://zdu.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sbj.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jkw.ydzc1.top

TS:   parseInt("42", 10); Number("42")
来源：http://dbu.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jxa.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pel.shzxlz.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://psm.hnxiangtu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://leo.hnxiangtu.top

[A07] 数字转字符串
来源：http://scx.zhoulong.xyz

Py:   str(42)
来源：http://kbw.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://tdx.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://hkd.zhijiandao.cn

TS:   String(42)
来源：http://ewo.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pjp.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://sgl.hammf.cn

Ruby: 42.to_s
来源：http://alv.hnxiangtu.top

C#:   42.ToString()
来源：http://bhr.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://yok.jinqigfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bmw.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://syj.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tbf.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ocs.wangshuangyany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://izl.jqgufenzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jer.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://arh.jqgfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nkx.xingfuxueyuan.xyz

[A09] 绝对值与最大最小值
来源：http://eml.tianlin.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bag.shangyingyoupin.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jhi.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ohj.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ylq.aibaodan.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aga.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gbn.pycfn.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kay.jlsjyb.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://snd.fengsongda.top

[A10] 生成随机数
来源：http://dwa.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://kvm.tarul.cn

PHP:  random_int(1, 100);
来源：http://lsb.jyoumei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://veq.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uhk.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://fau.kuanghao11.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kli.fktsv.cn

Ruby: rand(1..100)
来源：http://gjb.bbcook.cn

C#:   new Random().Next(1, 101)
来源：http://lbp.c1oappe.top

[A11] 条件表达式（三元）
来源：http://ads.yongpay.top

Py:   "yes" if x > 0 else "no"
来源：http://bsh.uphjek.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://esf.xuanzx.com

JS:   x > 0 ? "yes" : "no"
来源：http://wnw.gotoacloud.top

TS:   x > 0 ? "yes" : "no"
来源：http://thb.sxryk.cn

Java: x > 0 ? "yes" : "no"
来源：http://gsh.daria6918.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mtm.birdmap.top

Ruby: x > 0 ? "yes" : "no"
来源：http://zch.dianchejie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zgh.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://xwe.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kbj.zhongyouzk.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hlf.hongshengwenyu.top

JS:   `Hello, ${name}!`
来源：http://wja.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://vtc.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://rvi.xingfuxueyuan.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rzw.nanxinkj.top

Ruby: "Hello, #{name}!"
来源：http://usf.0kj1m.cn

C#:   $"Hello, {name}!"
来源：http://lqr.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ref.pycfn.com

Py:   "第一行\n第二行"
来源：http://dkn.havefunace.top

PHP:  "第一行\n第二行"
来源：http://vum.52xcode.cn

JS:   "第一行\n第二行"
来源：http://afb.tarul.cn

TS:   "第一行\n第二行"
来源：http://olb.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://xmi.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://uat.dashuyun.cn

Ruby: "第一行\n第二行"
来源：http://sjl.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://oso.jinqigufen.top

[A14] 注释写法
来源：http://qld.9152youxi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ess.9152youxi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://npl.0kj1m.cn

JS:   // 单行；/* 多行 */
来源：http://uua.0kj1m.cn

TS:   // 单行；/* 多行 */
来源：http://qqe.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tiw.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://wsg.gzhubu.top

Ruby: # 单行；=begin 多行 =end
来源：http://njo.tian-w.cn

C#:   // 单行；/* 多行 */
来源：http://trf.havefunace.top

[A15] 空值判断与默认值
来源：http://wlo.smart0.xyz

Py:   value = data or "默认值"
来源：http://udc.bbcook.cn

PHP:  $value = $data ?? "默认值";
来源：http://emt.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://daw.uphjek.com

TS:   const value = data ?? "默认值";
来源：http://bfj.jqgufenzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hbi.haohaochexian.top

Go:   if data == "" { data = "默认值" }
来源：http://jch.fehbvm.com

Ruby: value = data || "默认值"
来源：http://zcd.ehwqpu.com

C#:   var value = data ?? "默认值";
来源：http://tca.jinqigfzy.top

[A16] 真假值判断规则
来源：http://vgt.ppjwa.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hlx.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ycn.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lfc.andypj.xyz

TS:   if (!x) {}
来源：http://nxp.zdqjudy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rih.bjfxy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zjh.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://lfa.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vrl.chenjidiqi.icu

[A17] 位运算
来源：http://cdu.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yve.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xbw.yangfankeji.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cir.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jel.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nqp.iojbl.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vta.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hcx.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dix.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://nri.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://exh.chenlongwang.top

PHP:  ord("A"); chr(65)
来源：http://qjm.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://exw.gzhubu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eny.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://ybb.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gvm.sysykeji.top

Ruby: "A".ord; 65.chr
来源：http://pin.ydzc1.top

C#:   (int)'A'; (char)65
来源：http://zop.jiagoushi.top

[A19] 交换两个变量
来源：http://wkw.jinyuanbaomall.cn

Py:   a, b = b, a
来源：http://bzz.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pre.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://mle.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://qvb.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://opa.wangshuangyany.cn

Go:   a, b = b, a
来源：http://wzf.sjlbkw.cn

Ruby: a, b = b, a
来源：http://xtr.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://bja.fehbvm.com

[A20] 读取标准输入
来源：http://kka.yuanzhike.top

Py:   name = input("请输入：")
来源：http://zuz.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lhi.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ayg.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://ivp.wangshuangyany.cn

Java: new Scanner(System.in).nextLine()
来源：http://eka.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vua.bbcook.cn

Ruby: gets.chomp
来源：http://udd.yj202588.top

C#:   Console.ReadLine();
来源：http://usa.jinqigfzy.top

[A21] 保留指定小数位输出
来源：http://cqu.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://uob.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rps.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://isi.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://hnu.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://msf.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tak.pengpengdd.cyou

Ruby: format("%.2f", 3.14159)
来源：http://pbf.smart0.xyz

C#:   3.14159.ToString("F2")
来源：http://ote.hfpthk.cn

[A22] 获取字符串长度
来源：http://iof.redwolf501.top

Py:   len(s)
来源：http://xnb.zhixingplan.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ibr.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jqd.sxryk.cn

TS:   s.length
来源：http://yhh.yongpay.top

Java: s.length()
来源：http://ihc.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gqi.jinqigfzy.top

Ruby: s.length
来源：http://omm.zhiwuduotai.top

C#:   s.Length
来源：http://ikk.yanxiufei.cn

[A23] 大小写转换
来源：http://eva.chenzaomai.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wzr.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fbx.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://knf.jqgfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvd.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nni.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yco.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://npo.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://kfx.yuanzhike.top

[A24] 去除首尾空白
来源：http://aee.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nbo.zdqjudy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eyd.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://azq.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zzd.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hbp.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://uhs.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://haw.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dpb.ydjk.org.cn

[A25] 字符串比较
来源：http://pjt.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://arh.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fhq.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mlr.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sbf.jqgufenzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bej.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kjk.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wff.guowangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://izb.zhongyouzk.top

[A26] 类型转换总览
来源：http://hwb.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hkj.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://obj.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lgw.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://upl.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://brt.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rqh.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ebp.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dmu.tanke756.top

================================================================================
来源：http://djz.hongshengwenyu.top

B. 流程控制
来源：http://zjd.fktsv.cn

================================================================================
来源：http://bcv.cqqwz.cn

[B01] 条件判断 if / else
来源：http://ziq.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://koa.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qqd.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rjw.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qtu.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lwp.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sxr.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eku.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mmi.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://iza.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ttm.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rhw.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tje.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uxg.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llk.nanxinkj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hqe.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cqb.ctjpmb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwo.gogol.net.cn

[B03] switch / match / case
来源：http://fbr.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wfh.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lgp.zhongyouzk.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://inj.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://smf.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kwl.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mkj.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tjl.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://axi.yuanzhike.top

[B04] for 计数循环
来源：http://vef.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://zvv.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iby.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eia.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wno.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uzb.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qkk.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://uvd.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vmg.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://yws.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://dim.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hkq.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://clk.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://evw.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://vaw.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kmt.sjlbkw.cn

Ruby: arr.each { |item| puts item }
来源：http://iba.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rlj.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://kdb.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lac.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zve.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pfb.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wdi.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tlk.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oxw.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://idg.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://etl.tian-w.cn

[B07] while 循环
来源：http://tfr.hammf.cn

Py:   while i < 10: i += 1
来源：http://uww.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://epb.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://yex.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://xbv.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://fvo.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uot.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://czx.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://qlh.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://ltf.sufxvd.cn

Py:   # 无 do-while：用 while True + break
来源：http://jgj.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zzt.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://iui.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://rxe.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://bip.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kki.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ckq.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://cwg.c1oappe.top

[B09] break 与 continue
来源：http://dky.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cmx.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://grt.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ejt.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aei.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://exf.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mlc.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yyr.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnt.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://gsd.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://toz.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tjv.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cuw.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lpq.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://env.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tgs.zhengqikj.top


<!-- 参考信息 -->