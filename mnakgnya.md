代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nrz.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://wny.daria6918.cn

Go:   name := "Alex"; age := 20
来源：http://qdr.9152youxi.cn

Ruby: name = "Alex"; age = 20
来源：http://fgv.xylfe.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ulh.zdbjq.cn

[A03] 常量定义
来源：http://jlz.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eps.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://hxy.52xcode.cn

JS:   const PI = 3.14159;
来源：http://jes.vehdjk.com

TS:   const PI: number = 3.14159;
来源：http://ecm.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://pqt.uphjek.com

Go:   const PI = 3.14159
来源：http://fvl.chenzaomai.com

Ruby: PI = 3.14159
来源：http://oaa.fzhhl.top

C#:   const double PI = 3.14159;
来源：http://qva.sysykeji.top

[A04] 判断变量类型
来源：http://ocp.vehdjk.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://yow.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ffe.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zcg.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://umo.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ucy.yuxming.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iil.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://onp.shzxlz.cn

C#:   x.GetType().Name; x is int
来源：http://dbl.jqgfzy.top

[A05] 整数除法与取模
来源：http://obw.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jtq.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bpx.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aeq.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ero.hongshengwenyu.top

Java: 7 / 2; 7 % 2
来源：http://jtg.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://kja.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://vys.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://rut.shanyushiyangkeji.top

[A06] 字符串转数字
来源：http://iwp.jlsjyb.cn

Py:   int("42"); float("3.14")
来源：http://upu.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bzt.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tzq.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://hwg.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pzj.ydjk.org.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ctb.sxryk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qmk.hammf.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ygd.zhijiandao.cn

[A07] 数字转字符串
来源：http://rua.jinqigfzy.top

Py:   str(42)
来源：http://qvq.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://nqs.yvedp.cn

JS:   String(42); (42).toString()
来源：http://mvk.xuanzx.com

TS:   String(42)
来源：http://nuo.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zwu.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://aww.zhoulong.xyz

Ruby: 42.to_s
来源：http://ioa.gaohongyu789.top

C#:   42.ToString()
来源：http://mxr.redwolf501.top

[A08] 取整与四舍五入
来源：http://zcu.xuanzx.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ykm.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mhs.vqdsnc.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fhx.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wqz.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fsi.zdqjudy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jnf.uphjek.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://tha.jiagoushi.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ndb.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://pra.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oie.9152youxi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xul.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wym.sweek.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zdg.shanyushiyangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://elv.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fzh.jlsjyb.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fhq.iojbl.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gnx.svipenyu.cn

[A10] 生成随机数
来源：http://zws.ybcxt.top

Py:   import random; random.randint(1, 100)
来源：http://yej.tarul.cn

PHP:  random_int(1, 100);
来源：http://scm.xziqi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oso.shangyingyoupin.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nhk.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://udt.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ozx.daxiang520.top

Ruby: rand(1..100)
来源：http://gvq.yj202588.top

C#:   new Random().Next(1, 101)
来源：http://xno.jyoumei.cn

[A11] 条件表达式（三元）
来源：http://usm.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://qgi.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lob.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rmr.cashguo.top

TS:   x > 0 ? "yes" : "no"
来源：http://qiw.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://vfz.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://eoy.nanxinkj.top

Ruby: x > 0 ? "yes" : "no"
来源：http://exk.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://qsa.yuanzhike.top

[A12] 字符串插值 / 格式化
来源：http://hbh.chenlongwang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://okn.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://utn.hammf.cn

JS:   `Hello, ${name}!`
来源：http://kjx.hongshengwenyu.top

TS:   `Hello, ${name}!`
来源：http://zpa.cheryme.top

Java: "Hello, %s!".formatted(name)
来源：http://wgu.smart0.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hwm.chenzaomai.com

Ruby: "Hello, #{name}!"
来源：http://ald.yvedp.cn

C#:   $"Hello, {name}!"
来源：http://jsm.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zbk.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://rwd.tanke756.top

PHP:  "第一行\n第二行"
来源：http://ebx.epnwcf.com

JS:   "第一行\n第二行"
来源：http://zxs.ybcxt.top

TS:   "第一行\n第二行"
来源：http://xyz.cashguo.top

Java: "第一行\n第二行"
来源：http://dti.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://tqg.chenjidiqi.icu

Ruby: "第一行\n第二行"
来源：http://fzr.epnwcf.com

C#:   "第一行\n第二行"
来源：http://qvk.jinqigufen.top

[A14] 注释写法
来源：http://vjp.hfpthk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kyz.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vnn.quarkkingdee.top

JS:   // 单行；/* 多行 */
来源：http://bpk.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://tal.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dze.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://rmn.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://zzc.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://vpr.gaohongyu789.top

[A15] 空值判断与默认值
来源：http://yto.0kj1m.cn

Py:   value = data or "默认值"
来源：http://kpv.shanyushiyangtech.top

PHP:  $value = $data ?? "默认值";
来源：http://vac.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://oyc.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://zis.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bon.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://fec.tanke756.top

Ruby: value = data || "默认值"
来源：http://flz.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://obl.tanke756.top

[A16] 真假值判断规则
来源：http://pzu.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://buj.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bmm.gotoacloud.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rrx.hammf.cn

TS:   if (!x) {}
来源：http://puj.yueranfly.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lzk.svipenyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cqu.yangfankeji.com

Ruby: unless x            # nil 与 false 为假
来源：http://bes.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nrc.yvedp.cn

[A17] 位运算
来源：http://yqx.nwbrower.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncs.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://koi.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bjy.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ups.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://elc.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://clw.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://twr.nanxinkj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oyh.uphjek.com

[A18] 字符与 ASCII 码互转
来源：http://gzm.redwolf501.top

Py:   ord("A"); chr(65)
来源：http://etu.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://bpq.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jts.zhoulong.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nnp.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://nyc.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jsk.birdmap.top

Ruby: "A".ord; 65.chr
来源：http://yhm.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://svv.yongpay.top

[A19] 交换两个变量
来源：http://qqw.pengpengdd.cyou

Py:   a, b = b, a
来源：http://pvh.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sjk.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://qgm.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://sxc.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://xyg.yfazqb.com

Go:   a, b = b, a
来源：http://ybs.tarul.cn

Ruby: a, b = b, a
来源：http://ctf.316326.xyz

C#:   (a, b) = (b, a);
来源：http://osw.gzhubu.top

[A20] 读取标准输入
来源：http://ant.hysaishi.cn

Py:   name = input("请输入：")
来源：http://nvp.zhijiandao.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nbl.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qxw.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://ihp.vqdsnc.cn

Java: new Scanner(System.in).nextLine()
来源：http://ztl.hammf.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gek.havefunace.top

Ruby: gets.chomp
来源：http://dfk.tian-w.cn

C#:   Console.ReadLine();
来源：http://zks.hammf.cn

[A21] 保留指定小数位输出
来源：http://exw.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://ukc.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tce.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://jrw.smart0.xyz

TS:   (3.14159).toFixed(2)
来源：http://agy.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://cxq.yangfankeji.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vpm.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://hxb.andypj.xyz

C#:   3.14159.ToString("F2")
来源：http://mvk.52xcode.cn

[A22] 获取字符串长度
来源：http://ndd.kuanghao11.cn

Py:   len(s)
来源：http://zfg.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rdb.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lev.zhijiandao.cn

TS:   s.length
来源：http://kzt.zdbjq.cn

Java: s.length()
来源：http://vcj.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ccy.sweek.top

Ruby: s.length
来源：http://kqs.ydjk.org.cn

C#:   s.Length
来源：http://knm.cqqwz.cn

[A23] 大小写转换
来源：http://fjr.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wdi.dianchejie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://njy.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hiw.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kel.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xka.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zxw.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pav.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kai.zdbjq.cn

[A24] 去除首尾空白
来源：http://xab.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fth.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xbo.sxryk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://evp.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pij.316326.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fow.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://xhl.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kum.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ivf.fzhhl.top

[A25] 字符串比较
来源：http://lth.tarul.cn

Py:   s1 == s2; s1 != s2
来源：http://yeo.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ulc.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vqh.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iob.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fqd.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zdj.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://npz.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hct.wangdashe.top

[A26] 类型转换总览
来源：http://upg.epnwcf.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ads.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sdk.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://adt.fengsongda.top

TS:   Number() String() Boolean() x as number
来源：http://qgt.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gbe.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aue.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mro.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jog.zhijiandao.cn

================================================================================
来源：http://xhx.bjfxy.top

B. 流程控制
来源：http://hzj.fanxiaobao.xyz

================================================================================
来源：http://noz.zdqjudy.top

[B01] 条件判断 if / else
来源：http://fvq.aizwys.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kap.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fdi.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dca.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nlv.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jtx.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zwb.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wlh.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gnd.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://yhb.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dwo.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kao.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzz.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkl.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dpz.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tpj.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vey.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyn.yj202588.top

[B03] switch / match / case
来源：http://fid.chenzaomai.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mzo.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rxx.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gmg.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fip.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fyq.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nyn.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rhb.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://upz.ivvv.top

[B04] for 计数循环
来源：http://ynt.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://cki.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vlq.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xaa.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://noq.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vzu.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qry.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://pvy.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nap.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://ifq.cucudq.cn

Py:   for item in arr: print(item)
来源：http://jok.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uqp.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://chw.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ery.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://myn.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mqu.jqgfzy.top

Ruby: arr.each { |item| puts item }
来源：http://lrd.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vog.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://xst.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mea.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zxt.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xxt.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nyu.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gme.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://crc.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hxu.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://usl.nanxinkj.top

[B07] while 循环
来源：http://cpv.yuxming.cn

Py:   while i < 10: i += 1
来源：http://plq.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ycf.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://aeb.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://wra.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://liv.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zzn.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://njg.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://eoe.birdmap.top

[B08] do-while（至少执行一次）
来源：http://goo.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://xbq.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gfo.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://jca.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://lrp.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://gky.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hzi.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://lwi.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://nqa.ydzc1.top

[B09] break 与 continue
来源：http://vqx.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lqq.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yma.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxd.xylfe.cn


<!-- 参考信息 -->