代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://sfr.jinqigufen.top

[A03] 常量定义
来源：http://rxm.hesvh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mom.xylfe.cn

PHP:  const PI = 3.14159;
来源：http://odh.shanyushiyangtech.top

JS:   const PI = 3.14159;
来源：http://rxz.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://xcz.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://ozl.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://xuk.fehbvm.com

Ruby: PI = 3.14159
来源：http://bqr.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://poh.wangshuangyany.cn

[A04] 判断变量类型
来源：http://teu.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vyd.jinqigufen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nmt.ywan-chungtsiang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wpz.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://wqo.ybcxt.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fav.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kkq.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://iel.epnwcf.com

C#:   x.GetType().Name; x is int
来源：http://nfz.epnwcf.com

[A05] 整数除法与取模
来源：http://yas.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zfx.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zwi.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bkk.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hhq.zhiwuduotai.top

Java: 7 / 2; 7 % 2
来源：http://ubg.fengsongda.top

Go:   7 / 2; 7 % 2
来源：http://ysi.haohaochexian.top

Ruby: 7 / 2; 7 % 2
来源：http://ypx.yangfankeji.com

C#:   7 / 2; 7 % 2
来源：http://xob.daxiang520.top

[A06] 字符串转数字
来源：http://kev.pycfn.com

Py:   int("42"); float("3.14")
来源：http://gvu.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gha.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lsq.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://ydl.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qsf.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xgj.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hkq.pycfn.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tne.guowangkeji.top

[A07] 数字转字符串
来源：http://uod.yj202588.top

Py:   str(42)
来源：http://bwy.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://ukd.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://kmn.ybcxt.top

TS:   String(42)
来源：http://pqk.feifeiyinyue.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zlc.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://sgh.hywenlv.cn

Ruby: 42.to_s
来源：http://ryp.ivvv.top

C#:   42.ToString()
来源：http://pig.chenlongwang.top

[A08] 取整与四舍五入
来源：http://nvh.nwbrower.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://awc.xylfe.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lpy.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lsx.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ccx.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uss.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mtr.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fhs.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bnr.svipenyu.cn

[A09] 绝对值与最大最小值
来源：http://gov.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oox.chenjidiqi.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iit.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://atv.cashguo.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://afb.chenjidiqi.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gti.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qxw.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mkb.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wpe.shangyingyoupin.top

[A10] 生成随机数
来源：http://dpl.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://pmy.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://pek.yfazqb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://alq.cdnleiting.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ydp.jinqigfzy.top

Java: new Random().nextInt(100) + 1
来源：http://qzy.hysaishi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bzq.jinqigufen.top

Ruby: rand(1..100)
来源：http://dlq.dashuyun.cn

C#:   new Random().Next(1, 101)
来源：http://fde.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://qqc.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://zvf.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ikl.wangdashe.top

JS:   x > 0 ? "yes" : "no"
来源：http://lhs.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://hcf.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://oac.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yiv.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://myh.kuanghao11.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cxr.ctjpmb.com

[A12] 字符串插值 / 格式化
来源：http://pck.ybcxt.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ieq.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fep.zhengqikj.top

JS:   `Hello, ${name}!`
来源：http://vnl.daxiang520.top

TS:   `Hello, ${name}!`
来源：http://czn.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://rqg.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fgz.hongshengwenyu.top

Ruby: "Hello, #{name}!"
来源：http://yhe.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://zmz.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vmh.vehdjk.com

Py:   "第一行\n第二行"
来源：http://qul.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://lcb.guannengcc.top

JS:   "第一行\n第二行"
来源：http://sxq.ydjk.org.cn

TS:   "第一行\n第二行"
来源：http://rtu.xziqi.cn

Java: "第一行\n第二行"
来源：http://ubc.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://ugo.shanyushiyangtech.top

Ruby: "第一行\n第二行"
来源：http://xma.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://can.ehwqpu.com

[A14] 注释写法
来源：http://jnj.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://edn.daxiang520.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://afw.xinyue.icu

JS:   // 单行；/* 多行 */
来源：http://nen.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://ejj.ybcxt.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uys.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://tdk.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://ioy.zhixingplan.top

C#:   // 单行；/* 多行 */
来源：http://htv.aibaodan.cn

[A15] 空值判断与默认值
来源：http://jic.cqqwz.cn

Py:   value = data or "默认值"
来源：http://mxr.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://fyb.chenjidiqi.icu

JS:   const value = data ?? "默认值";
来源：http://dvz.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://zcb.redwolf501.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://izp.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://klg.ppjwa.cn

Ruby: value = data || "默认值"
来源：http://sjo.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://dxo.daria6918.cn

[A16] 真假值判断规则
来源：http://hcd.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://suw.bjfxy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wdu.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fyq.bjfxy.top

TS:   if (!x) {}
来源：http://fom.fzhhl.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://idx.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bpx.bbcook.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kov.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uvh.dashuyun.cn

[A17] 位运算
来源：http://top.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blo.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ayb.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wiw.c1oappe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vzc.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qzg.tianlin.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jxx.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aou.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzi.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://sdn.yj20258888.top

Py:   ord("A"); chr(65)
来源：http://fxy.epnwcf.com

PHP:  ord("A"); chr(65)
来源：http://skh.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://obi.daxiang520.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qmg.kuanghao11.cn

Java: (int) 'A'; (char) 65
来源：http://qin.cheryme.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mnk.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://cpt.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://dwt.havefunace.top

[A19] 交换两个变量
来源：http://jsg.iojbl.cn

Py:   a, b = b, a
来源：http://wgv.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jpf.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://dhy.tanke756.top

TS:   [a, b] = [b, a];
来源：http://ykx.xingfuxueyuan.xyz

Java: int t = a; a = b; b = t;
来源：http://guz.gzhubu.top

Go:   a, b = b, a
来源：http://yrk.yongpay.top

Ruby: a, b = b, a
来源：http://lrb.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://jjd.shzxlz.cn

[A20] 读取标准输入
来源：http://zmb.xingfuxueyuan.xyz

Py:   name = input("请输入：")
来源：http://dem.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://auj.iojbl.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wue.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://jsa.xingfuxueyuan.xyz

Java: new Scanner(System.in).nextLine()
来源：http://cqu.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zyr.xylfe.cn

Ruby: gets.chomp
来源：http://rpb.jqgfzy.top

C#:   Console.ReadLine();
来源：http://wte.jinqigfzy.top

[A21] 保留指定小数位输出
来源：http://cpr.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://ush.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uex.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://jmt.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://wrw.ivvv.top

Java: String.format("%.2f", 3.14159)
来源：http://qse.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://puv.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://orb.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://rdy.havefunace.top

[A22] 获取字符串长度
来源：http://csl.52xcode.cn

Py:   len(s)
来源：http://kcx.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://foa.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aqu.hysaishi.cn

TS:   s.length
来源：http://tbo.nanxuanxn.top

Java: s.length()
来源：http://aoz.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lvv.ppjwa.cn

Ruby: s.length
来源：http://mzr.yongpay.top

C#:   s.Length
来源：http://lvx.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://dho.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ypt.ppjwa.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mon.meibo888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://erx.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nvw.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bge.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ggo.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://stf.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kor.yanxiufei.cn

[A24] 去除首尾空白
来源：http://aeb.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nai.snrcjt.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bis.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sxn.haohaochexian.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ank.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hzu.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://vms.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kiy.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qku.yonumen.top

[A25] 字符串比较
来源：http://txd.cucudq.cn

Py:   s1 == s2; s1 != s2
来源：http://xjq.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gcy.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lis.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bbw.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xrs.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ibq.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://tae.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nfk.tanke756.top

[A26] 类型转换总览
来源：http://rcn.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://igf.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://res.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jpi.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://aon.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ixa.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fdr.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kcz.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lhq.gogol.net.cn

================================================================================
来源：http://vdx.9152youxi.cn

B. 流程控制
来源：http://boc.fanxiaobao.xyz

================================================================================
来源：http://boj.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://dcu.zhijiandao.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zbc.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fud.cdnleiting.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nin.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ksk.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bgx.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yac.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bgg.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kvd.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://qjt.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tpa.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kib.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbg.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pcq.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ryv.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kda.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ijt.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pcn.chenzaomai.com

[B03] switch / match / case
来源：http://scu.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lna.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qcp.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://omy.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ohv.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ydj.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://brx.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ubu.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://flk.yanxiufei.cn

[B04] for 计数循环
来源：http://xkl.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://yeq.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://you.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://son.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dir.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rhs.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kau.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://cgs.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://syy.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://qrg.zycfv.cn

Py:   for item in arr: print(item)
来源：http://hcs.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ros.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://hzk.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gom.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://lol.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ept.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://wsr.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nup.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://xtf.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zlt.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mkc.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vod.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://otj.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ott.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ksg.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dod.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://khp.jianghu66.top

[B07] while 循环
来源：http://cpg.yuxming.cn

Py:   while i < 10: i += 1
来源：http://kvd.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://nfv.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://ets.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://pqm.epnwcf.com

Java: while (i < 10) { i++; }
来源：http://ova.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bhi.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://whb.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://mfu.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://hhu.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://ork.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bwy.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://naz.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://hkx.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://vgi.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wun.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://poa.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://odr.xuanzx.com

[B09] break 与 continue
来源：http://ifk.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sqi.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://riu.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggv.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkp.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwz.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gow.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ywd.haohaochexian.top


<!-- 参考信息 -->