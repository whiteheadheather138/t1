代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://jqr.jlsjyb.cn

[A03] 常量定义
来源：http://ffa.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xpi.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://ubt.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://nth.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://qjs.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://lhd.smart0.xyz

Go:   const PI = 3.14159
来源：http://hxg.hammf.cn

Ruby: PI = 3.14159
来源：http://jwn.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://gme.yfazqb.com

[A04] 判断变量类型
来源：http://gck.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://lxn.shzxlz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cqn.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tzi.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://glw.cdnleiting.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rdv.hysaishi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xcr.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ktm.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://pqa.fktsv.cn

[A05] 整数除法与取模
来源：http://ant.yanxiufei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jzc.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tzu.gzhubu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pbu.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ywy.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://fam.birdmap.top

Go:   7 / 2; 7 % 2
来源：http://ytu.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://eme.wangdashe.top

C#:   7 / 2; 7 % 2
来源：http://siy.yj20258888.top

[A06] 字符串转数字
来源：http://hgg.xuanzx.com

Py:   int("42"); float("3.14")
来源：http://pbb.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://igh.aibaodan.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sel.zhengqikj.top

TS:   parseInt("42", 10); Number("42")
来源：http://phx.tanke756.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nkx.chenlongwang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uwh.gaohongyu789.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ixh.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blg.shangyingyoupin.top

[A07] 数字转字符串
来源：http://igu.smart0.xyz

Py:   str(42)
来源：http://mdq.fanxiaobao.xyz

PHP:  (string) 42; strval(42)
来源：http://wlq.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://cxk.zhoulong.xyz

TS:   String(42)
来源：http://ews.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uwl.shuidangran.top

Go:   strconv.Itoa(42)
来源：http://khq.hnqzz.top

Ruby: 42.to_s
来源：http://zpj.nanxuanxn.top

C#:   42.ToString()
来源：http://xqw.cheryme.top

[A08] 取整与四舍五入
来源：http://mks.jinqigfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kkp.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hvm.ehwqpu.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pek.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aqh.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ejt.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bmt.cqqwz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fzt.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fpb.havefunace.top

[A09] 绝对值与最大最小值
来源：http://ubb.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ahs.0kj1m.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jow.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hgg.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qmh.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xdg.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tgd.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dcf.epnwcf.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ahv.zdqjudy.top

[A10] 生成随机数
来源：http://jym.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://lge.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://tiw.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ouf.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yzl.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://lzg.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kzn.zdqjudy.top

Ruby: rand(1..100)
来源：http://fcc.sjlbkw.cn

C#:   new Random().Next(1, 101)
来源：http://nyu.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://vsa.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://ndv.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dfc.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cnv.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ijx.yanxiufei.cn

Java: x > 0 ? "yes" : "no"
来源：http://ixy.tianlin.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://und.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://snm.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ujo.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://sxu.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://okw.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bud.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://lnd.ehwqpu.com

TS:   `Hello, ${name}!`
来源：http://rat.zhongyouzk.top

Java: "Hello, %s!".formatted(name)
来源：http://riq.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aqr.sweek.top

Ruby: "Hello, #{name}!"
来源：http://lpa.redwolf501.top

C#:   $"Hello, {name}!"
来源：http://ubw.hammf.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dyi.hfpthk.cn

Py:   "第一行\n第二行"
来源：http://itj.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://uhq.yongpay.top

JS:   "第一行\n第二行"
来源：http://rzr.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://ayx.uphjek.com

Java: "第一行\n第二行"
来源：http://ztu.yj20258.top

Go:   "第一行\n第二行"
来源：http://jdq.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://oco.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://wxd.sjlbkw.cn

[A14] 注释写法
来源：http://mdx.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dne.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pfb.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://vgo.guowangkeji.top

TS:   // 单行；/* 多行 */
来源：http://xdy.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zfr.fengsongda.top

Go:   // 单行；/* 多行 */
来源：http://efy.guowangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://lmc.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://ypj.snrcjt.cn

[A15] 空值判断与默认值
来源：http://vos.havefunace.top

Py:   value = data or "默认值"
来源：http://sde.yvedp.cn

PHP:  $value = $data ?? "默认值";
来源：http://wei.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://nuc.sweek.top

TS:   const value = data ?? "默认值";
来源：http://imq.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fbc.ydzc1.top

Go:   if data == "" { data = "默认值" }
来源：http://ybg.bbcook.cn

Ruby: value = data || "默认值"
来源：http://oss.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://umi.yfazqb.com

[A16] 真假值判断规则
来源：http://vuz.52xcode.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tjf.guannengcc.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bdn.hfpthk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cdj.zhixingplan.top

TS:   if (!x) {}
来源：http://hvt.zhengqikj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zhr.jqgufenzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.sweek.top

Ruby: unless x            # nil 与 false 为假
来源：http://wyy.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iox.xingfuxueyuan.xyz

[A17] 位运算
来源：http://iym.ctjpmb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yfi.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://upf.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vct.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pyz.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxc.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://goh.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wcp.bjfxy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://izk.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://vii.jinghuilouyu.cn

Py:   ord("A"); chr(65)
来源：http://bog.daxiang520.top

PHP:  ord("A"); chr(65)
来源：http://mwj.ywan-chungtsiang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iuf.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mgo.guannengcc.top

Java: (int) 'A'; (char) 65
来源：http://vsk.ydzc1.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xqh.yangfankeji.com

Ruby: "A".ord; 65.chr
来源：http://nlf.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://emz.yj202588.top

[A19] 交换两个变量
来源：http://rrt.ydjk.org.cn

Py:   a, b = b, a
来源：http://luq.pengpengdd.cyou

PHP:  [$a, $b] = [$b, $a];
来源：http://imz.yongpay.top

JS:   [a, b] = [b, a];
来源：http://cmh.dianchejie.cn

TS:   [a, b] = [b, a];
来源：http://klk.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://hws.sweek.top

Go:   a, b = b, a
来源：http://kvv.sweek.top

Ruby: a, b = b, a
来源：http://wpi.tanke756.top

C#:   (a, b) = (b, a);
来源：http://vnu.9152youxi.cn

[A20] 读取标准输入
来源：http://hrp.ivvv.top

Py:   name = input("请输入：")
来源：http://isd.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://cww.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zgo.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://yzy.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://zmf.fktsv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zkb.andypj.xyz

Ruby: gets.chomp
来源：http://nvb.dianchejie.cn

C#:   Console.ReadLine();
来源：http://rer.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://gsb.0kj1m.cn

Py:   f"{3.14159:.2f}"
来源：http://wvp.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ots.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://jwy.chenlongwang.top

TS:   (3.14159).toFixed(2)
来源：http://hcw.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://vop.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hxl.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://ucs.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://tqq.hnqzz.top

[A22] 获取字符串长度
来源：http://opt.meibo888.top

Py:   len(s)
来源：http://ngv.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://clj.zdqjudy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wcq.fktsv.cn

TS:   s.length
来源：http://rsb.gzhubu.top

Java: s.length()
来源：http://pju.xuanzx.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ojf.yuanzhike.top

Ruby: s.length
来源：http://xub.hongshengwenyu.top

C#:   s.Length
来源：http://vam.snrcjt.cn

[A23] 大小写转换
来源：http://ufz.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pry.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xre.guannengcc.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eml.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tdg.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rzq.zdbjq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://srn.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uvc.zhaomingkeji.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://ebn.ctjpmb.com

[A24] 去除首尾空白
来源：http://usr.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wys.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xty.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://idf.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iqv.cheryme.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kaa.cashguo.top

Go:   strings.TrimSpace(s)
来源：http://ywr.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://omz.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qka.jinqigfzy.top

[A25] 字符串比较
来源：http://otc.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://qaz.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eyt.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hkw.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rbh.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://avz.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vrs.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ezl.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://evd.dianchejie.cn

[A26] 类型转换总览
来源：http://bbk.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://poy.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://esq.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rex.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://iun.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mal.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yom.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mcf.tianlin.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://odw.bbcook.cn

================================================================================
来源：http://xjc.andypj.xyz

B. 流程控制
来源：http://uvc.daxiang520.top

================================================================================
来源：http://hss.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://lea.zdqjudy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xxv.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lfz.guowangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://alp.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rra.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jqq.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bmt.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cza.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://got.hcnkem.com

[B02] 多分支 else if / elif
来源：http://qhw.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ocp.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ebh.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvb.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://riw.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wbi.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://maj.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qtb.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wds.fanxiaobao.xyz

[B03] switch / match / case
来源：http://yqu.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ejo.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gra.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zth.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hst.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rac.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vpl.yongpay.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://klr.jyoumei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vpz.yangfankeji.com

[B04] for 计数循环
来源：http://vnt.ivvv.top

Py:   for i in range(10): print(i)
来源：http://zmx.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tlj.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ydl.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ekn.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ksy.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dmx.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://dpp.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oxk.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://tih.havefunace.top

Py:   for item in arr: print(item)
来源：http://agn.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://veh.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zof.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bsk.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fpz.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vqt.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://plq.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://njw.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://bwa.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fux.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jeo.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nox.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hvw.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tfl.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wew.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jly.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gfo.hammf.cn

[B07] while 循环
来源：http://mle.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://fvp.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://ehq.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://rzs.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://fjc.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://pmx.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ask.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://yxc.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://lol.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://ljk.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://yfa.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://loe.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://gvc.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://nwg.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://utm.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wsf.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://ewt.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://kbv.haohaochexian.top

[B09] break 与 continue
来源：http://rvu.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wql.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ekc.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzw.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sff.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dcy.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bcg.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bze.yj20258888.top


<!-- 参考信息 -->