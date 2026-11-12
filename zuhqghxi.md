代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://ana.hongshengwenyu.top

[A03] 常量定义
来源：http://ecq.yueranfly.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://deb.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://aum.sxryk.cn

JS:   const PI = 3.14159;
来源：http://vnm.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://uko.tarul.cn

Java: static final double PI = 3.14159;
来源：http://bcm.ydzc1.top

Go:   const PI = 3.14159
来源：http://asp.zhengqikj.top

Ruby: PI = 3.14159
来源：http://mgk.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://pil.nwbrower.top

[A04] 判断变量类型
来源：http://boa.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jeq.snrcjt.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jhb.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dfu.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://xoa.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ihr.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://bkb.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://urx.jinqigufen.top

C#:   x.GetType().Name; x is int
来源：http://vtl.cucudq.cn

[A05] 整数除法与取模
来源：http://qdk.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ico.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://yqj.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fif.andypj.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ley.chenjidiqi.icu

Java: 7 / 2; 7 % 2
来源：http://xbd.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://hqe.zhixingplan.top

Ruby: 7 / 2; 7 % 2
来源：http://dlm.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://paq.iojbl.cn

[A06] 字符串转数字
来源：http://hts.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://llf.yvedp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://for.gogol.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cap.nanxuanxn.top

TS:   parseInt("42", 10); Number("42")
来源：http://bho.xuetiantiany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vyp.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eks.yvedp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fwu.xinyue.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kqg.uphjek.com

[A07] 数字转字符串
来源：http://fjw.jianghu66.top

Py:   str(42)
来源：http://vfr.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://ojc.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://ciu.ppjwa.cn

TS:   String(42)
来源：http://zdc.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lab.jianghu66.top

Go:   strconv.Itoa(42)
来源：http://qki.jlsjyb.cn

Ruby: 42.to_s
来源：http://ezh.epnwcf.com

C#:   42.ToString()
来源：http://eky.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://jaf.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kkv.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pow.fehbvm.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fee.ydjk.org.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jxb.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cet.jyoumei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bbv.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wbe.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cjl.yfazqb.com

[A09] 绝对值与最大最小值
来源：http://gqz.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://szs.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qon.sjlbkw.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://czm.dianchejie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://plz.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fuw.fktsv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ndg.cashguo.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nss.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pgz.jinqigfzy.top

[A10] 生成随机数
来源：http://cic.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://vjc.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://gmp.zhiwuduotai.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://caq.sjlbkw.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ide.yangfankeji.com

Java: new Random().nextInt(100) + 1
来源：http://njl.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fqf.xziqi.cn

Ruby: rand(1..100)
来源：http://eeg.vehdjk.com

C#:   new Random().Next(1, 101)
来源：http://wjw.yonumen.top

[A11] 条件表达式（三元）
来源：http://qta.guannengcc.top

Py:   "yes" if x > 0 else "no"
来源：http://jdw.ivvv.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jcl.zhengqikj.top

JS:   x > 0 ? "yes" : "no"
来源：http://wnw.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zhb.nanxinkj.top

Java: x > 0 ? "yes" : "no"
来源：http://qeh.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://onb.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qsg.shanyushiyangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://pdy.daxiang520.top

[A12] 字符串插值 / 格式化
来源：http://bvc.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eyn.sxryk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cpy.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://nci.c1oappe.top

TS:   `Hello, ${name}!`
来源：http://ltg.andypj.xyz

Java: "Hello, %s!".formatted(name)
来源：http://lal.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://usb.cucudq.cn

Ruby: "Hello, #{name}!"
来源：http://ayu.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://lci.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://pxw.kuanghao11.cn

Py:   "第一行\n第二行"
来源：http://pue.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://ypp.ydjk.org.cn

JS:   "第一行\n第二行"
来源：http://bhl.cucudq.cn

TS:   "第一行\n第二行"
来源：http://anx.kuanghao11.cn

Java: "第一行\n第二行"
来源：http://uln.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://vht.xuetiantiany.cn

Ruby: "第一行\n第二行"
来源：http://tyy.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://ket.fzhhl.top

[A14] 注释写法
来源：http://dsn.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jxk.mhx1999.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://auf.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://dfo.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://rzp.jinyuanbaomall.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://htj.yuanzhike.top

Go:   // 单行；/* 多行 */
来源：http://ubz.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://qlr.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://mdo.yvedp.cn

[A15] 空值判断与默认值
来源：http://fvj.chenlongwang.top

Py:   value = data or "默认值"
来源：http://jlj.shanyushiyangtech.top

PHP:  $value = $data ?? "默认值";
来源：http://gxa.yuxming.cn

JS:   const value = data ?? "默认值";
来源：http://dke.daxiang520.top

TS:   const value = data ?? "默认值";
来源：http://jqc.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oyk.ydzc1.top

Go:   if data == "" { data = "默认值" }
来源：http://eph.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://zdo.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://eni.gogol.net.cn

[A16] 真假值判断规则
来源：http://xsk.iojbl.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hoi.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qhj.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mwo.daria6918.cn

TS:   if (!x) {}
来源：http://fwc.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jee.aibaodan.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cyj.hfpthk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://abd.cdnleiting.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://adz.sysykeji.top

[A17] 位运算
来源：http://wui.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zuh.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pvy.shanyushiyangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zrs.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qcd.bjfxy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aos.xingfuxueyuan.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ptw.yj20258888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://anh.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zum.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://tum.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://zbg.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://uci.fktsv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cgt.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jil.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://mqz.sjlbkw.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fys.fengsongda.top

Ruby: "A".ord; 65.chr
来源：http://cgu.aibaodan.cn

C#:   (int)'A'; (char)65
来源：http://imn.ppjwa.cn

[A19] 交换两个变量
来源：http://din.shzxlz.cn

Py:   a, b = b, a
来源：http://opj.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qcs.tian-w.cn

JS:   [a, b] = [b, a];
来源：http://gsl.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://hki.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://jci.sweek.top

Go:   a, b = b, a
来源：http://wnk.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://qlx.bbcook.cn

C#:   (a, b) = (b, a);
来源：http://bqd.xingfuxueyuan.xyz

[A20] 读取标准输入
来源：http://gns.yongpay.top

Py:   name = input("请输入：")
来源：http://lmo.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://fdg.svipenyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bgr.cashguo.top

TS:   // Node.js：readline 模块
来源：http://yhj.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://eqt.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dtc.zhongyouzk.top

Ruby: gets.chomp
来源：http://gsq.pycfn.com

C#:   Console.ReadLine();
来源：http://hpp.andypj.xyz

[A21] 保留指定小数位输出
来源：http://cml.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://wnm.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nvc.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://onc.gogol.net.cn

TS:   (3.14159).toFixed(2)
来源：http://ueq.redwolf501.top

Java: String.format("%.2f", 3.14159)
来源：http://rxj.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xlk.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://njt.jyoumei.cn

C#:   3.14159.ToString("F2")
来源：http://yon.fengsongda.top

[A22] 获取字符串长度
来源：http://lzm.daxiang520.top

Py:   len(s)
来源：http://ugd.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://snf.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zhe.fanxiaobao.xyz

TS:   s.length
来源：http://kln.hammf.cn

Java: s.length()
来源：http://ssf.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tje.xuetiantiany.cn

Ruby: s.length
来源：http://xbx.wangdashe.top

C#:   s.Length
来源：http://ead.bbcook.cn

[A23] 大小写转换
来源：http://fjx.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://paz.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://umj.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qxr.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pkc.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cuv.hesvh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qyq.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uxj.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://yix.nwbrower.top

[A24] 去除首尾空白
来源：http://wjq.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dnz.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ldc.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aks.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tic.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jim.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://fub.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hlj.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fpv.quarkkingdee.top

[A25] 字符串比较
来源：http://sxy.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://uql.vehdjk.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uue.fanxiaobao.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ajx.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gdp.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://djy.xingfuxueyuan.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dfj.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dop.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jzl.tarul.cn

[A26] 类型转换总览
来源：http://wzx.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xcd.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iur.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dnc.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://cnd.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://agx.52xcode.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sya.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://rji.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cww.hongshengwenyu.top

================================================================================
来源：http://zhd.ppjwa.cn

B. 流程控制
来源：http://vng.cheryme.top

================================================================================
来源：http://pnw.c1oappe.top

[B01] 条件判断 if / else
来源：http://dlj.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tot.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://atq.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dli.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zyy.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mjj.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cjk.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ksl.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rld.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://cqc.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cau.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://clo.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwu.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://etk.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fiy.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://opt.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://opn.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wsf.zhiwuduotai.top

[B03] switch / match / case
来源：http://byb.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://evl.nanxinkj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xtj.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xfz.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zmj.zhongyouzk.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://reo.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bpt.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sft.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fyh.aibaodan.cn

[B04] for 计数循环
来源：http://rxv.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://ogo.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dpd.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wwb.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jwt.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wvs.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yux.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://bmp.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sxv.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://zgy.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://pap.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rds.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gpy.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zwj.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qkr.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gqr.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://gnb.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uyn.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://mlb.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bty.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gug.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wuz.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vvo.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xsb.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqg.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gpm.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aym.ywan-chungtsiang.top

[B07] while 循环
来源：http://msr.sysykeji.top

Py:   while i < 10: i += 1
来源：http://jli.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://fpq.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://puu.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://czb.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://hxx.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zgc.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://war.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://uks.pycfn.com

[B08] do-while（至少执行一次）
来源：http://ibj.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://zbq.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xzk.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://hhj.zhiwuduotai.top

TS:   do { i++; } while (i < 10);
来源：http://kfk.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://ffz.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bfj.jinghuilouyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eyq.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://bhv.meibo888.top

[B09] break 与 continue
来源：http://hvu.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yvn.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tvc.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://arx.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yok.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ntz.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://osi.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gqa.cucudq.cn


<!-- 参考信息 -->