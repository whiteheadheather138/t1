代发 wailian999

[A02] 变量声明与赋值
来源：http://idw.shangyingyoupin.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dxp.tianlin.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://mnl.andypj.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://xro.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rnp.ybcxt.top

Java: String name = "Alex"; int age = 20;
来源：http://zar.zycfv.cn

Go:   name := "Alex"; age := 20
来源：http://xwu.zhiwuduotai.top

Ruby: name = "Alex"; age = 20
来源：http://oel.bbcook.cn

C#:   string name = "Alex"; int age = 20;
来源：http://awg.yj20258888.top

[A03] 常量定义
来源：http://jqr.shangyingyoupin.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qhu.pengpengdd.cyou

PHP:  const PI = 3.14159;
来源：http://mld.nwbrower.top

JS:   const PI = 3.14159;
来源：http://gdt.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://njg.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://ccl.ywan-chungtsiang.top

Go:   const PI = 3.14159
来源：http://mcq.cheryme.top

Ruby: PI = 3.14159
来源：http://avz.zdbjq.cn

C#:   const double PI = 3.14159;
来源：http://qmi.guannengcc.top

[A04] 判断变量类型
来源：http://vgz.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://qjc.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bfj.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mwo.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://flw.daxiang520.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kyl.kuanghao11.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jvb.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tli.c1oappe.top

C#:   x.GetType().Name; x is int
来源：http://bjd.haohaochexian.top

[A05] 整数除法与取模
来源：http://kty.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rwz.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ict.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nuw.uphjek.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xtv.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://jji.fengsongda.top

Go:   7 / 2; 7 % 2
来源：http://pjy.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://yjb.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://zjf.daria6918.cn

[A06] 字符串转数字
来源：http://gxp.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://wux.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qse.chenjidiqi.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://osg.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://luq.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pcy.tianlin.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xgi.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eex.0kj1m.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://asi.yangfankeji.com

[A07] 数字转字符串
来源：http://roi.chenzaomai.com

Py:   str(42)
来源：http://mhx.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://wxx.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://tsm.chenzaomai.com

TS:   String(42)
来源：http://niu.hywenlv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vwr.hammf.cn

Go:   strconv.Itoa(42)
来源：http://vnc.svipenyu.cn

Ruby: 42.to_s
来源：http://pde.chenjidiqi.icu

C#:   42.ToString()
来源：http://uiz.sxryk.cn

[A08] 取整与四舍五入
来源：http://png.andypj.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://feh.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mwu.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pwg.xingfuxueyuan.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uiw.shangyingyoupin.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tim.yueranfly.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tze.ehwqpu.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://gjh.316326.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mxc.birdmap.top

[A09] 绝对值与最大最小值
来源：http://ddc.xziqi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fzg.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://awk.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://aze.xuanzx.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://itg.shangyingyoupin.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yxt.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jsc.epnwcf.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wpw.zhiwuduotai.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oqh.0kj1m.cn

[A10] 生成随机数
来源：http://xib.jianghu66.top

Py:   import random; random.randint(1, 100)
来源：http://tgg.hammf.cn

PHP:  random_int(1, 100);
来源：http://liw.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vxy.c1oappe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ejx.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://jbr.zhengqikj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yft.svipenyu.cn

Ruby: rand(1..100)
来源：http://uia.zdqjudy.top

C#:   new Random().Next(1, 101)
来源：http://ppm.zdbjq.cn

[A11] 条件表达式（三元）
来源：http://iqe.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://piq.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uof.gaohongyu789.top

JS:   x > 0 ? "yes" : "no"
来源：http://car.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://clf.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://mei.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bmx.iojbl.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qng.fengsongda.top

C#:   x > 0 ? "yes" : "no"
来源：http://jvb.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://chg.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://whw.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bqj.sweek.top

JS:   `Hello, ${name}!`
来源：http://xla.chenjidiqi.icu

TS:   `Hello, ${name}!`
来源：http://arp.52xcode.cn

Java: "Hello, %s!".formatted(name)
来源：http://pox.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kmr.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://zgj.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://ozs.hongshengwenyu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lng.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://dav.guowangkeji.top

PHP:  "第一行\n第二行"
来源：http://swa.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://pbk.jianghu66.top

TS:   "第一行\n第二行"
来源：http://saa.hnqzz.top

Java: "第一行\n第二行"
来源：http://ylc.sxryk.cn

Go:   "第一行\n第二行"
来源：http://snv.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://htd.yj20258.top

C#:   "第一行\n第二行"
来源：http://dxw.aibaodan.cn

[A14] 注释写法
来源：http://xcx.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://brc.fktsv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yzz.fktsv.cn

JS:   // 单行；/* 多行 */
来源：http://pec.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://ufm.cdnleiting.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dnu.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://qjl.hesvh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mmc.yvedp.cn

C#:   // 单行；/* 多行 */
来源：http://mdo.meibo888.top

[A15] 空值判断与默认值
来源：http://jxa.daxiang520.top

Py:   value = data or "默认值"
来源：http://ifk.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://uhm.xylfe.cn

JS:   const value = data ?? "默认值";
来源：http://twz.jinyuanbaomall.cn

TS:   const value = data ?? "默认值";
来源：http://yow.gogol.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jdk.chenzaomai.com

Go:   if data == "" { data = "默认值" }
来源：http://ukq.yj202588.top

Ruby: value = data || "默认值"
来源：http://efm.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://mqn.smart0.xyz

[A16] 真假值判断规则
来源：http://kzr.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vhl.jianghu66.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yqu.fehbvm.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hit.zhaomingkeji.xyz

TS:   if (!x) {}
来源：http://bzp.pengpengdd.cyou

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://akh.sjlbkw.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://meu.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://lex.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://erv.daxiang520.top

[A17] 位运算
来源：http://dfk.zycfv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wyk.ppjwa.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wwr.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwd.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zsm.yvedp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tdq.andypj.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iuw.sysykeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vqi.zdqjudy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jbn.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://ehi.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://ytg.ivvv.top

PHP:  ord("A"); chr(65)
来源：http://qve.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lqp.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tuz.tian-w.cn

Java: (int) 'A'; (char) 65
来源：http://zkn.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://upa.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://nke.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://sts.xinyue.icu

[A19] 交换两个变量
来源：http://ghf.yueranfly.top

Py:   a, b = b, a
来源：http://idk.zhixingplan.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sgh.birdmap.top

JS:   [a, b] = [b, a];
来源：http://unc.vehdjk.com

TS:   [a, b] = [b, a];
来源：http://lns.dashuyun.cn

Java: int t = a; a = b; b = t;
来源：http://xiz.feifeiyinyue.top

Go:   a, b = b, a
来源：http://wek.cashguo.top

Ruby: a, b = b, a
来源：http://dnf.jqgufenzy.top

C#:   (a, b) = (b, a);
来源：http://dkl.bbcook.cn

[A20] 读取标准输入
来源：http://kkc.svipenyu.cn

Py:   name = input("请输入：")
来源：http://csl.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zmy.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://apd.hnxiangtu.top

TS:   // Node.js：readline 模块
来源：http://lpv.jinqigfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://xkp.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tlk.cucudq.cn

Ruby: gets.chomp
来源：http://rrm.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://pkm.zhongyouzk.top

[A21] 保留指定小数位输出
来源：http://kfu.52xcode.cn

Py:   f"{3.14159:.2f}"
来源：http://vix.xuanzx.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ofv.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://sso.zhiwuduotai.top

TS:   (3.14159).toFixed(2)
来源：http://dfs.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://ijz.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qfu.yj20258.top

Ruby: format("%.2f", 3.14159)
来源：http://ohm.zhongyouzk.top

C#:   3.14159.ToString("F2")
来源：http://woq.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://ztd.yfazqb.com

Py:   len(s)
来源：http://vvn.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cgv.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://crr.ydzc1.top

TS:   s.length
来源：http://hvu.fzhhl.top

Java: s.length()
来源：http://xaa.epnwcf.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jxx.dianchejie.cn

Ruby: s.length
来源：http://ppr.meibo888.top

C#:   s.Length
来源：http://oon.zhijiandao.cn

[A23] 大小写转换
来源：http://qnm.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://phi.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ofz.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oet.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jgn.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ndv.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aoi.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rsk.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jvk.epnwcf.com

[A24] 去除首尾空白
来源：http://usd.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://csp.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lpa.zhongyouzk.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dkt.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hsc.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nqv.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://xiz.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nfw.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zoj.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://amr.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://feb.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ysr.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mwt.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lnr.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bzx.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cgz.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vfg.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://loi.gzhubu.top

[A26] 类型转换总览
来源：http://yjy.kuanghao11.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ksk.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ose.c1oappe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://isn.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://ljq.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oxc.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ray.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bzw.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wfc.jyoumei.cn

================================================================================
来源：http://bqj.zhengqikj.top

B. 流程控制
来源：http://iqs.yuxming.cn

================================================================================
来源：http://vgl.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://oih.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cuz.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aym.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wjr.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://asv.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zqm.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uuj.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xld.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nrr.hnqzz.top

[B02] 多分支 else if / elif
来源：http://wde.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://odw.kuanghao11.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dbl.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvy.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xaa.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbv.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://elk.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://avi.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://age.yongpay.top

[B03] switch / match / case
来源：http://jxd.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dzm.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dlb.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fcj.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nfe.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mwg.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kjq.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qxz.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hwz.bbcook.cn

[B04] for 计数循环
来源：http://nhc.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://tin.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://osk.bbcook.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ajl.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oku.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rgn.0kj1m.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hbe.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://lju.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pwe.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://loy.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://hco.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vrl.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://his.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dfc.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fbo.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ees.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://rol.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bul.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://mcd.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://isc.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rpd.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zim.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wjo.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ugz.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ljr.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ndl.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bxn.andypj.xyz

[B07] while 循环
来源：http://ona.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://vyq.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://phc.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://itq.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://vlg.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://mdv.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wvd.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://hfq.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://wkb.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://zyy.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://itb.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://udx.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://ubf.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://upf.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://gbx.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jcc.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://axt.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://xvz.yueranfly.top


<!-- 参考信息 -->