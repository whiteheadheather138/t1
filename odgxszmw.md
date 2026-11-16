代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://wjq.52xcode.cn

[A03] 常量定义
来源：http://bft.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cnv.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://dsl.guannengcc.top

JS:   const PI = 3.14159;
来源：http://nvr.ppjwa.cn

TS:   const PI: number = 3.14159;
来源：http://lmw.svipenyu.cn

Java: static final double PI = 3.14159;
来源：http://pyo.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://xaf.fktsv.cn

Ruby: PI = 3.14159
来源：http://ztw.hnqzz.top

C#:   const double PI = 3.14159;
来源：http://vhg.quarkkingdee.top

[A04] 判断变量类型
来源：http://kca.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ukg.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hum.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://shb.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://clt.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bbn.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qqu.feifeiyinyue.top

Ruby: x.class; x.is_a?(Integer)
来源：http://enx.iojbl.cn

C#:   x.GetType().Name; x is int
来源：http://kqi.svipenyu.cn

[A05] 整数除法与取模
来源：http://qfp.tianlin.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kws.jinqigfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fot.epnwcf.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uog.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yod.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://iye.smart0.xyz

Go:   7 / 2; 7 % 2
来源：http://lam.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://rwu.daxiang520.top

C#:   7 / 2; 7 % 2
来源：http://sqg.gzhubu.top

[A06] 字符串转数字
来源：http://ywq.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://lyb.gzhubu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xyj.tanke756.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lti.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://hxr.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nup.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wcf.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yck.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wey.fktsv.cn

[A07] 数字转字符串
来源：http://yil.vehdjk.com

Py:   str(42)
来源：http://yoz.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://cly.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://hno.feifeiyinyue.top

TS:   String(42)
来源：http://dmu.svipenyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://elc.jqgufenzy.top

Go:   strconv.Itoa(42)
来源：http://bkj.wangdashe.top

Ruby: 42.to_s
来源：http://zfu.ctjpmb.com

C#:   42.ToString()
来源：http://nbe.jiagoushi.top

[A08] 取整与四舍五入
来源：http://krp.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bey.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nzr.jinghuilouyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pug.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nyu.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zdd.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kpc.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qkg.sysykeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aoi.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://yov.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zsl.jinyuanbaomall.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hbj.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://brq.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kjt.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eko.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bzn.aizwys.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://plo.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yhd.c1oappe.top

[A10] 生成随机数
来源：http://uym.gogol.net.cn

Py:   import random; random.randint(1, 100)
来源：http://ntk.yangfankeji.com

PHP:  random_int(1, 100);
来源：http://rpr.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lny.tian-w.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nqz.hongshengwenyu.top

Java: new Random().nextInt(100) + 1
来源：http://wha.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tij.jinqigfzy.top

Ruby: rand(1..100)
来源：http://uip.vqdsnc.cn

C#:   new Random().Next(1, 101)
来源：http://dfm.jinqigufen.top

[A11] 条件表达式（三元）
来源：http://rwk.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://pce.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cat.aibaodan.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hcd.xylfe.cn

TS:   x > 0 ? "yes" : "no"
来源：http://eqw.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://cdv.cucudq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tvd.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fih.jinqigfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://jij.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://ssn.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://omk.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qfc.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://igm.uphjek.com

TS:   `Hello, ${name}!`
来源：http://sut.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://qhq.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://upt.hysaishi.cn

Ruby: "Hello, #{name}!"
来源：http://dth.tanke756.top

C#:   $"Hello, {name}!"
来源：http://lpx.tarul.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://krk.cashguo.top

Py:   "第一行\n第二行"
来源：http://dlu.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://ron.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://jnl.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://gnn.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://zke.0kj1m.cn

Go:   "第一行\n第二行"
来源：http://yvo.fktsv.cn

Ruby: "第一行\n第二行"
来源：http://glf.sweek.top

C#:   "第一行\n第二行"
来源：http://tud.pycfn.com

[A14] 注释写法
来源：http://cko.hongshengwenyu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qii.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://xnl.aizwys.cn

JS:   // 单行；/* 多行 */
来源：http://tqs.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://yry.zhoulong.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rof.dashuyun.cn

Go:   // 单行；/* 多行 */
来源：http://gby.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ngo.havefunace.top

C#:   // 单行；/* 多行 */
来源：http://ksl.yonumen.top

[A15] 空值判断与默认值
来源：http://zzn.yj20258.top

Py:   value = data or "默认值"
来源：http://pet.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://qfi.haohaochexian.top

JS:   const value = data ?? "默认值";
来源：http://rzb.yj20258.top

TS:   const value = data ?? "默认值";
来源：http://dew.nanxuanxn.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jnu.c1oappe.top

Go:   if data == "" { data = "默认值" }
来源：http://dlw.xuanzx.com

Ruby: value = data || "默认值"
来源：http://yad.dashuyun.cn

C#:   var value = data ?? "默认值";
来源：http://cdj.jinyuanbaomall.cn

[A16] 真假值判断规则
来源：http://tyw.smart0.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yhv.yongpay.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://shq.shuidangran.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cci.zdbjq.cn

TS:   if (!x) {}
来源：http://upa.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zkt.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sdb.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sva.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qxa.sjlbkw.cn

[A17] 位运算
来源：http://dmj.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uwl.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kfn.cucudq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hop.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hyg.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tpa.daxiang520.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nmg.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gek.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uyk.cucudq.cn

[A18] 字符与 ASCII 码互转
来源：http://srf.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://ffr.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://nbb.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ave.zdqjudy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pyt.aibaodan.cn

Java: (int) 'A'; (char) 65
来源：http://quu.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://njn.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://pad.wangdashe.top

C#:   (int)'A'; (char)65
来源：http://qtk.quarkkingdee.top

[A19] 交换两个变量
来源：http://irp.andypj.xyz

Py:   a, b = b, a
来源：http://glm.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cpd.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://rpd.cucudq.cn

TS:   [a, b] = [b, a];
来源：http://sny.yuxming.cn

Java: int t = a; a = b; b = t;
来源：http://lag.iojbl.cn

Go:   a, b = b, a
来源：http://pfr.xziqi.cn

Ruby: a, b = b, a
来源：http://apd.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://zno.aizwys.cn

[A20] 读取标准输入
来源：http://hse.zhixingplan.top

Py:   name = input("请输入：")
来源：http://yfk.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hee.sxryk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rhl.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://hkd.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://swx.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qyz.gogol.net.cn

Ruby: gets.chomp
来源：http://pnw.jlsjyb.cn

C#:   Console.ReadLine();
来源：http://ruz.guannengcc.top

[A21] 保留指定小数位输出
来源：http://qqf.snrcjt.cn

Py:   f"{3.14159:.2f}"
来源：http://lry.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ihe.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://gxi.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://fat.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://cwk.daria6918.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ria.hysaishi.cn

Ruby: format("%.2f", 3.14159)
来源：http://jmx.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://tsm.zhijiandao.cn

[A22] 获取字符串长度
来源：http://xxr.fehbvm.com

Py:   len(s)
来源：http://icq.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pvs.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qzn.ppjwa.cn

TS:   s.length
来源：http://osh.zhoulong.xyz

Java: s.length()
来源：http://nhh.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://imk.hnqzz.top

Ruby: s.length
来源：http://gmm.xuetiantiany.cn

C#:   s.Length
来源：http://hro.yongpay.top

[A23] 大小写转换
来源：http://bhm.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rpt.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aiq.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jrn.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pvc.mhx1999.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hsn.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vdi.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iit.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qup.daxiang520.top

[A24] 去除首尾空白
来源：http://euy.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gvl.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xsx.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tlt.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pvh.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mdr.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://fkc.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qgn.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pck.nanxuanxn.top

[A25] 字符串比较
来源：http://lpf.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://rkc.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rvl.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://itg.gzhubu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bjn.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lml.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ngg.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jva.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cnv.vehdjk.com

[A26] 类型转换总览
来源：http://xnc.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mnc.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dnm.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mwv.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://vci.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ekl.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dsa.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kad.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vig.yj202588.top

================================================================================
来源：http://kcv.jinqigfzy.top

B. 流程控制
来源：http://yea.chenzaomai.com

================================================================================
来源：http://uqu.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://ltw.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mbe.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sbg.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tdc.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aho.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://yqt.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wny.tian-w.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://foz.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gnn.tanke756.top

[B02] 多分支 else if / elif
来源：http://zoo.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mxt.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xlq.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmd.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krr.ybcxt.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://umv.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sxx.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wem.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pdi.wangdashe.top

[B03] switch / match / case
来源：http://tqi.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bwo.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rki.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qjk.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://juj.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yge.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xdr.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vqg.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ocw.zhiwuduotai.top

[B04] for 计数循环
来源：http://nso.xingfuxueyuan.xyz

Py:   for i in range(10): print(i)
来源：http://kzb.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kwz.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yks.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kye.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://quy.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://naz.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://mct.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yxk.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://fyn.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://dal.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xkf.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tvk.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hco.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xbw.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qle.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://xmf.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cio.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://aek.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://twk.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eiw.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uul.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nup.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mqa.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gfj.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://heo.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pii.epnwcf.com

[B07] while 循环
来源：http://vgb.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://kmg.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ufy.mhx1999.top

JS:   while (i < 10) { i++; }
来源：http://oeq.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://eiq.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://ljl.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://miu.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://mdu.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://zbm.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://lvb.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://tnc.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dre.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://cdo.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://miv.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://nen.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://blm.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://krl.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://nvg.fzhhl.top

[B09] break 与 continue
来源：http://gpb.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjd.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mhb.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dfp.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynj.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ofd.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pol.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qeg.pycfn.com


<!-- 参考信息 -->