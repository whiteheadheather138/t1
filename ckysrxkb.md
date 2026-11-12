代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://wlc.wangshuangyany.cn

[A03] 常量定义
来源：http://gwk.dashuyun.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fht.hongshengwenyu.top

PHP:  const PI = 3.14159;
来源：http://tsa.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://qha.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://fcb.cashguo.top

Java: static final double PI = 3.14159;
来源：http://flf.wangdashe.top

Go:   const PI = 3.14159
来源：http://zri.cucudq.cn

Ruby: PI = 3.14159
来源：http://lgu.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://zpm.fengsongda.top

[A04] 判断变量类型
来源：http://oux.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ahz.ydzc1.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cwm.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vpe.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://elk.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rlr.aizwys.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pjt.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://qex.aizwys.cn

C#:   x.GetType().Name; x is int
来源：http://ezk.haohaochexian.top

[A05] 整数除法与取模
来源：http://hqh.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qbi.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://roo.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nyp.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oqz.aibaodan.cn

Java: 7 / 2; 7 % 2
来源：http://klf.ppjwa.cn

Go:   7 / 2; 7 % 2
来源：http://zox.iojbl.cn

Ruby: 7 / 2; 7 % 2
来源：http://wdd.ppjwa.cn

C#:   7 / 2; 7 % 2
来源：http://ete.jqgufenzy.top

[A06] 字符串转数字
来源：http://iry.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://rte.yangfankeji.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bmz.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://apb.gogol.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qyg.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cbe.guowangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://leq.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yqa.fktsv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://umb.cdnleiting.top

[A07] 数字转字符串
来源：http://yfp.hfpthk.cn

Py:   str(42)
来源：http://ehd.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://qxq.andypj.xyz

JS:   String(42); (42).toString()
来源：http://sty.feifeiyinyue.top

TS:   String(42)
来源：http://fht.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gha.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://wra.fengsongda.top

Ruby: 42.to_s
来源：http://jzx.cashguo.top

C#:   42.ToString()
来源：http://akm.smart0.xyz

[A08] 取整与四舍五入
来源：http://lfv.jiagoushi.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uvy.ctjpmb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qvy.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ewy.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://whm.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kkd.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pdo.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cob.hnqzz.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vwj.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://emz.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hgy.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ptw.zhiwuduotai.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zil.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mzc.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yim.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ndr.ydjk.org.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ypw.hysaishi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gda.ydjk.org.cn

[A10] 生成随机数
来源：http://qgq.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://wmx.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://pxk.yfazqb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ucj.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fjl.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://suc.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fbh.jiagoushi.top

Ruby: rand(1..100)
来源：http://drf.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://rxq.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://pse.guowangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://rth.snrcjt.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tlt.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mcn.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://onq.andypj.xyz

Java: x > 0 ? "yes" : "no"
来源：http://lqq.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dfb.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mau.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://vvq.wangdashe.top

[A12] 字符串插值 / 格式化
来源：http://nuv.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qad.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vzb.redwolf501.top

JS:   `Hello, ${name}!`
来源：http://vsa.tarul.cn

TS:   `Hello, ${name}!`
来源：http://bhi.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://ryt.jqgfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://koe.pycfn.com

Ruby: "Hello, #{name}!"
来源：http://zzj.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://sdm.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hed.dianchejie.cn

Py:   "第一行\n第二行"
来源：http://rdm.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://juz.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://bae.gotoacloud.top

TS:   "第一行\n第二行"
来源：http://kgr.316326.xyz

Java: "第一行\n第二行"
来源：http://isf.zhiwuduotai.top

Go:   "第一行\n第二行"
来源：http://dko.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://jhm.nanxuanxn.top

C#:   "第一行\n第二行"
来源：http://fxh.jqgfzy.top

[A14] 注释写法
来源：http://dyh.gotoacloud.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pvw.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rdb.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://eat.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://day.vehdjk.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rme.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://jfj.fengsongda.top

Ruby: # 单行；=begin 多行 =end
来源：http://phy.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://qub.0kj1m.cn

[A15] 空值判断与默认值
来源：http://vjj.fehbvm.com

Py:   value = data or "默认值"
来源：http://vnq.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://pzd.epnwcf.com

JS:   const value = data ?? "默认值";
来源：http://azj.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://grj.ybcxt.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xyo.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://kjj.yongpay.top

Ruby: value = data || "默认值"
来源：http://ulx.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://jwp.jqgfzy.top

[A16] 真假值判断规则
来源：http://kxv.sxryk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wkk.jyoumei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vwh.smart0.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://adt.yj20258.top

TS:   if (!x) {}
来源：http://edg.hammf.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aft.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jjr.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qon.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://prg.316326.xyz

[A17] 位运算
来源：http://hmx.shanyushiyangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jya.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ogt.zycfv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iox.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uyr.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://izw.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fua.ydzc1.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dbm.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fqu.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://iqd.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://yfc.gogol.net.cn

PHP:  ord("A"); chr(65)
来源：http://gbp.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hka.iojbl.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://awn.pengpengdd.cyou

Java: (int) 'A'; (char) 65
来源：http://zdp.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://isc.cucudq.cn

Ruby: "A".ord; 65.chr
来源：http://fqi.yvedp.cn

C#:   (int)'A'; (char)65
来源：http://you.sysykeji.top

[A19] 交换两个变量
来源：http://nno.hywenlv.cn

Py:   a, b = b, a
来源：http://nso.zhiwuduotai.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ndk.tarul.cn

JS:   [a, b] = [b, a];
来源：http://hkc.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://fuk.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://rcf.bbcook.cn

Go:   a, b = b, a
来源：http://jua.haohaochexian.top

Ruby: a, b = b, a
来源：http://yhe.tarul.cn

C#:   (a, b) = (b, a);
来源：http://xcj.fktsv.cn

[A20] 读取标准输入
来源：http://utg.zdqjudy.top

Py:   name = input("请输入：")
来源：http://mzb.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qnb.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tha.tarul.cn

TS:   // Node.js：readline 模块
来源：http://xep.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://kww.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mip.chenjidiqi.icu

Ruby: gets.chomp
来源：http://tdy.chenjidiqi.icu

C#:   Console.ReadLine();
来源：http://fri.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://skp.zhiwuduotai.top

Py:   f"{3.14159:.2f}"
来源：http://qit.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uxa.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://lpt.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://byc.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://vfa.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gkx.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://qeh.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://xpq.yfazqb.com

[A22] 获取字符串长度
来源：http://jkn.havefunace.top

Py:   len(s)
来源：http://twa.9152youxi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://opt.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zuh.ydjk.org.cn

TS:   s.length
来源：http://lji.52xcode.cn

Java: s.length()
来源：http://bjj.epnwcf.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cif.sxryk.cn

Ruby: s.length
来源：http://ysv.iojbl.cn

C#:   s.Length
来源：http://bvz.andypj.xyz

[A23] 大小写转换
来源：http://vek.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pre.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xdc.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qpd.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://crj.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qxa.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zfh.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://smv.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://azx.zhoulong.xyz

[A24] 去除首尾空白
来源：http://jrb.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://egs.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://auo.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mdp.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pdj.zhengqikj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rrh.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://wsw.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ghh.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://plm.tianlin.xyz

[A25] 字符串比较
来源：http://pgg.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://fji.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sdu.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eav.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ujd.birdmap.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wru.fzhhl.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://btd.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rob.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hfr.nanxuanxn.top

[A26] 类型转换总览
来源：http://krg.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gbx.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ceq.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lfr.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://dli.zhongyouzk.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ifr.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vuk.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://udy.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rab.feifeiyinyue.top

================================================================================
来源：http://pqk.dashuyun.cn

B. 流程控制
来源：http://orq.xylfe.cn

================================================================================
来源：http://mpr.ehwqpu.com

[B01] 条件判断 if / else
来源：http://xok.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://knr.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xke.xuetiantiany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://syk.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qgs.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gws.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mkv.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ezg.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rjp.fengsongda.top

[B02] 多分支 else if / elif
来源：http://ocp.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dcw.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eta.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://msb.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tcb.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ykf.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uov.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lrk.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tcz.xylfe.cn

[B03] switch / match / case
来源：http://sas.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://det.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ujl.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wfu.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://acj.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bnf.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ies.xuanzx.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tyt.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fzw.shanyushiyangtech.top

[B04] for 计数循环
来源：http://tje.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://buu.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qbn.fzhhl.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vlj.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tld.smart0.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tjh.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ynd.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://abm.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zol.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://ktj.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://wuu.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fpk.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://lsz.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sky.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://grs.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jwz.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://ugx.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ecp.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://lhu.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://vlx.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lbi.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gkd.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dpb.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fxa.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://svk.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://puj.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ejq.fktsv.cn

[B07] while 循环
来源：http://kla.52xcode.cn

Py:   while i < 10: i += 1
来源：http://pkg.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://zym.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://xix.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://cep.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://hjv.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://igx.kuanghao11.cn

Ruby: while i < 10; i += 1; end
来源：http://jcc.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://xeo.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://fxl.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://yik.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://gni.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://car.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://ghl.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://ify.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pgf.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://gmx.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://lsk.yongpay.top

[B09] break 与 continue
来源：http://jcd.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dqr.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bmn.zhongyouzk.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://juh.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ruh.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxs.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iys.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xwi.ywan-chungtsiang.top


<!-- 参考信息 -->