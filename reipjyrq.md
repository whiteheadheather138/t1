代发 wailian999

[A02] 变量声明与赋值
来源：http://lfo.gaohongyu789.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oku.9152youxi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tbk.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vgt.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vky.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://wht.mhx1999.top

Go:   name := "Alex"; age := 20
来源：http://xxl.cheryme.top

Ruby: name = "Alex"; age = 20
来源：http://rof.sweek.top

C#:   string name = "Alex"; int age = 20;
来源：http://hwv.yueranfly.top

[A03] 常量定义
来源：http://mtq.sjlbkw.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oud.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://oay.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://cxy.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://jeq.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://mts.9152youxi.cn

Go:   const PI = 3.14159
来源：http://tio.pycfn.com

Ruby: PI = 3.14159
来源：http://hla.yanxiufei.cn

C#:   const double PI = 3.14159;
来源：http://tqt.gzhubu.top

[A04] 判断变量类型
来源：http://nvv.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mws.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vvt.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gdh.nanxuanxn.top

TS:   typeof x; x instanceof Date
来源：http://zjf.vqdsnc.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tjq.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://qbx.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kuw.jiagoushi.top

C#:   x.GetType().Name; x is int
来源：http://jup.jinghuilouyu.cn

[A05] 整数除法与取模
来源：http://xbu.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sov.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vqz.yuxming.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://woi.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lui.yonumen.top

Java: 7 / 2; 7 % 2
来源：http://yyw.feifeiyinyue.top

Go:   7 / 2; 7 % 2
来源：http://slm.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://xxh.52xcode.cn

C#:   7 / 2; 7 % 2
来源：http://wup.9152youxi.cn

[A06] 字符串转数字
来源：http://cec.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://uzb.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xbx.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vjx.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rpr.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://szw.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://umi.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://aeg.quarkkingdee.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lix.sufxvd.cn

[A07] 数字转字符串
来源：http://dfw.c1oappe.top

Py:   str(42)
来源：http://pca.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://ssr.yongpay.top

JS:   String(42); (42).toString()
来源：http://rls.yvedp.cn

TS:   String(42)
来源：http://klj.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ggo.kuanghao11.cn

Go:   strconv.Itoa(42)
来源：http://vog.ehwqpu.com

Ruby: 42.to_s
来源：http://lbn.birdmap.top

C#:   42.ToString()
来源：http://tdr.fehbvm.com

[A08] 取整与四舍五入
来源：http://tyw.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hmy.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hfl.yfazqb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yry.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ikr.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dwg.yj20258.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qwe.xziqi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ydh.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qad.nwbrower.top

[A09] 绝对值与最大最小值
来源：http://bbu.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eaz.yangfankeji.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lot.birdmap.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iti.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ehf.jqgufenzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jmx.hfpthk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ukc.zhoulong.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ycb.cucudq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://brj.hnqzz.top

[A10] 生成随机数
来源：http://yws.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://bcy.andypj.xyz

PHP:  random_int(1, 100);
来源：http://ain.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://heg.cashguo.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gkx.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://blt.xinyue.icu

Go:   rand.Intn(100) + 1               // math/rand
来源：http://alk.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://yqi.svipenyu.cn

C#:   new Random().Next(1, 101)
来源：http://kse.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://gxa.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://qoj.hywenlv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bpj.daria6918.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gif.jqgufenzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://xuw.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://pvf.hcnkem.com

Go:   // 无三元运算符，需用 if 语句
来源：http://sqa.xylfe.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dlg.zhaomingkeji.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://gqk.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://smu.9152youxi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://osh.jinghuilouyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zkk.yvedp.cn

JS:   `Hello, ${name}!`
来源：http://bpg.ehwqpu.com

TS:   `Hello, ${name}!`
来源：http://cxa.yvedp.cn

Java: "Hello, %s!".formatted(name)
来源：http://fzr.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kdl.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://tzc.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://frt.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://clf.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://ilc.ctjpmb.com

PHP:  "第一行\n第二行"
来源：http://hnt.cucudq.cn

JS:   "第一行\n第二行"
来源：http://pwz.yj20258.top

TS:   "第一行\n第二行"
来源：http://ehh.jqgfzy.top

Java: "第一行\n第二行"
来源：http://vqs.shuidangran.top

Go:   "第一行\n第二行"
来源：http://tkd.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://fiw.pycfn.com

C#:   "第一行\n第二行"
来源：http://llz.yueranfly.top

[A14] 注释写法
来源：http://gsu.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mdd.bjfxy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hyn.guannengcc.top

JS:   // 单行；/* 多行 */
来源：http://fly.c1oappe.top

TS:   // 单行；/* 多行 */
来源：http://wug.shanyushiyangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rcz.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://xmp.pengpengdd.cyou

Ruby: # 单行；=begin 多行 =end
来源：http://zqd.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://vfm.vqdsnc.cn

[A15] 空值判断与默认值
来源：http://jda.xingfuxueyuan.xyz

Py:   value = data or "默认值"
来源：http://scj.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://dpq.yuanzhike.top

JS:   const value = data ?? "默认值";
来源：http://rem.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://lnb.guowangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dcq.fengsongda.top

Go:   if data == "" { data = "默认值" }
来源：http://nju.dianchejie.cn

Ruby: value = data || "默认值"
来源：http://oed.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://nka.yanxiufei.cn

[A16] 真假值判断规则
来源：http://kdz.ivvv.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gqv.bjfxy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ydu.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xxp.meibo888.top

TS:   if (!x) {}
来源：http://uuq.xuetiantiany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rqq.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kfx.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://ocq.yuanzhike.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oho.snrcjt.cn

[A17] 位运算
来源：http://yyh.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rwl.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wro.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ecn.ybcxt.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nkb.epnwcf.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kda.c1oappe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uma.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jyu.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yiz.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://isi.birdmap.top

Py:   ord("A"); chr(65)
来源：http://rpt.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://czv.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yva.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vdd.aibaodan.cn

Java: (int) 'A'; (char) 65
来源：http://fin.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yoh.pycfn.com

Ruby: "A".ord; 65.chr
来源：http://pow.svipenyu.cn

C#:   (int)'A'; (char)65
来源：http://afx.meibo888.top

[A19] 交换两个变量
来源：http://llo.cucudq.cn

Py:   a, b = b, a
来源：http://hiv.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dnc.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://bnx.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://ysk.ppjwa.cn

Java: int t = a; a = b; b = t;
来源：http://ukd.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://ivn.jlsjyb.cn

Ruby: a, b = b, a
来源：http://vbo.shanyushiyangtech.top

C#:   (a, b) = (b, a);
来源：http://dwc.tian-w.cn

[A20] 读取标准输入
来源：http://bgf.ybcxt.top

Py:   name = input("请输入：")
来源：http://oje.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://hux.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vyb.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://zec.hnqzz.top

Java: new Scanner(System.in).nextLine()
来源：http://aki.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tkn.sufxvd.cn

Ruby: gets.chomp
来源：http://gur.nanxinkj.top

C#:   Console.ReadLine();
来源：http://fen.shuidangran.top

[A21] 保留指定小数位输出
来源：http://ges.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://xbf.fzhhl.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zcb.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://kpe.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://qti.birdmap.top

Java: String.format("%.2f", 3.14159)
来源：http://qgo.xuanzx.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rvs.vqdsnc.cn

Ruby: format("%.2f", 3.14159)
来源：http://rwf.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://imy.jiagoushi.top

[A22] 获取字符串长度
来源：http://nhm.pengpengdd.cyou

Py:   len(s)
来源：http://uel.nwbrower.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tur.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gao.zhengqikj.top

TS:   s.length
来源：http://qzr.shanyushiyangkeji.top

Java: s.length()
来源：http://php.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ljl.hysaishi.cn

Ruby: s.length
来源：http://wps.bjfxy.top

C#:   s.Length
来源：http://ard.316326.xyz

[A23] 大小写转换
来源：http://igc.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mrb.9152youxi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qzp.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvt.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ojk.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lzy.jinqigufen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ufo.chenzaomai.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dik.316326.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://vft.shzxlz.cn

[A24] 去除首尾空白
来源：http://shy.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bvy.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uqm.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uoe.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bat.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pdo.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://mru.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ugk.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xvm.316326.xyz

[A25] 字符串比较
来源：http://wfz.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://zlo.nanxinkj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bno.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uvt.sjlbkw.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blo.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ifz.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nbc.smart0.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ooq.vehdjk.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://skj.xuetiantiany.cn

[A26] 类型转换总览
来源：http://emn.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rrm.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jph.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vld.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://qqm.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cnx.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xyu.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://imn.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tlt.52xcode.cn

================================================================================
来源：http://dki.jinyuanbaomall.cn

B. 流程控制
来源：http://qba.aizwys.cn

================================================================================
来源：http://cgd.yueranfly.top

[B01] 条件判断 if / else
来源：http://ccb.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bgn.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kms.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hfy.redwolf501.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cxf.tarul.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bsg.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aws.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ait.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sai.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://wxo.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yds.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lqw.guowangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wze.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mxm.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbr.chenlongwang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://esi.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ber.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kkp.redwolf501.top

[B03] switch / match / case
来源：http://lfx.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qxm.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fay.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nte.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ftv.cucudq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pem.birdmap.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tud.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gua.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://krx.kuanghao11.cn

[B04] for 计数循环
来源：http://xmz.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://bwj.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bln.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uyu.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tyv.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tkb.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bqv.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://rpd.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://src.daria6918.cn

[B05] 遍历数组 / 列表
来源：http://hoo.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://oip.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vrw.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://olu.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xuw.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kos.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://npb.gzhubu.top

Ruby: arr.each { |item| puts item }
来源：http://ojb.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://apz.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://sir.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bbp.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fyd.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gju.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mwi.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://frp.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gen.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hvt.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://utn.zhaomingkeji.xyz

[B07] while 循环
来源：http://dqq.sweek.top

Py:   while i < 10: i += 1
来源：http://tiy.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yqk.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://fkl.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://lgy.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://kyz.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uef.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://rrc.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://wjn.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://ztx.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://wec.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xen.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://nnu.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://mvm.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://dwk.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kxx.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bqd.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://bjh.shzxlz.cn


<!-- 参考信息 -->