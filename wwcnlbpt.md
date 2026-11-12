代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://rbr.52xcode.cn

[A03] 常量定义
来源：http://xza.yonumen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bwg.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://tar.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://mlv.ydjk.org.cn

TS:   const PI: number = 3.14159;
来源：http://qko.haohaochexian.top

Java: static final double PI = 3.14159;
来源：http://spf.daria6918.cn

Go:   const PI = 3.14159
来源：http://hyz.haohaochexian.top

Ruby: PI = 3.14159
来源：http://zie.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://ikl.bbcook.cn

[A04] 判断变量类型
来源：http://llo.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cha.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fkt.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zkm.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://ozs.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qfu.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lhs.svipenyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zui.quarkkingdee.top

C#:   x.GetType().Name; x is int
来源：http://bab.cheryme.top

[A05] 整数除法与取模
来源：http://ykz.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ndz.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://udc.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dys.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fjh.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://cxz.jlsjyb.cn

Go:   7 / 2; 7 % 2
来源：http://dlj.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://knx.cqqwz.cn

C#:   7 / 2; 7 % 2
来源：http://cmt.smart0.xyz

[A06] 字符串转数字
来源：http://uid.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://mbe.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dun.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dhl.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://smz.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://igv.zdqjudy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zmq.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bhg.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aqg.dashuyun.cn

[A07] 数字转字符串
来源：http://jap.bjfxy.top

Py:   str(42)
来源：http://zpr.dianchejie.cn

PHP:  (string) 42; strval(42)
来源：http://hid.mhx1999.top

JS:   String(42); (42).toString()
来源：http://dyi.ppjwa.cn

TS:   String(42)
来源：http://hpn.jianghu66.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://upw.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://ngn.xinyue.icu

Ruby: 42.to_s
来源：http://hwo.ehwqpu.com

C#:   42.ToString()
来源：http://leb.hnxiangtu.top

[A08] 取整与四舍五入
来源：http://mhj.jiagoushi.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eqn.ctjpmb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tri.vqdsnc.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kiy.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://egb.hysaishi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ikm.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yvd.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://yed.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://igx.ybcxt.top

[A09] 绝对值与最大最小值
来源：http://pap.yuxming.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xeq.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bnj.fehbvm.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nrg.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wdv.zdbjq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vrh.aibaodan.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xpg.smart0.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fbb.wangshuangyany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zwj.tarul.cn

[A10] 生成随机数
来源：http://cla.feifeiyinyue.top

Py:   import random; random.randint(1, 100)
来源：http://jvl.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://uix.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nvg.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aaq.yonumen.top

Java: new Random().nextInt(100) + 1
来源：http://ntk.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xok.xinyue.icu

Ruby: rand(1..100)
来源：http://mhq.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://lnm.andypj.xyz

[A11] 条件表达式（三元）
来源：http://bup.vqdsnc.cn

Py:   "yes" if x > 0 else "no"
来源：http://xdb.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sgg.havefunace.top

JS:   x > 0 ? "yes" : "no"
来源：http://gvo.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://wtn.hywenlv.cn

Java: x > 0 ? "yes" : "no"
来源：http://xyt.chenjidiqi.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://gnx.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tfg.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://frp.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://mpa.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wnc.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rgo.sysykeji.top

JS:   `Hello, ${name}!`
来源：http://vxa.nwbrower.top

TS:   `Hello, ${name}!`
来源：http://jka.gaohongyu789.top

Java: "Hello, %s!".formatted(name)
来源：http://jve.chenzaomai.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rgg.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://gjv.xylfe.cn

C#:   $"Hello, {name}!"
来源：http://sec.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hxj.pengpengdd.cyou

Py:   "第一行\n第二行"
来源：http://hcr.zycfv.cn

PHP:  "第一行\n第二行"
来源：http://wgx.pycfn.com

JS:   "第一行\n第二行"
来源：http://fhm.zdbjq.cn

TS:   "第一行\n第二行"
来源：http://pde.yonumen.top

Java: "第一行\n第二行"
来源：http://yfh.smart0.xyz

Go:   "第一行\n第二行"
来源：http://tzv.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://xjt.jianghu66.top

C#:   "第一行\n第二行"
来源：http://tdm.yuanzhike.top

[A14] 注释写法
来源：http://qth.tian-w.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mfc.xingfuxueyuan.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://uqj.ydjk.org.cn

JS:   // 单行；/* 多行 */
来源：http://hos.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://jkm.yongpay.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kcv.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://ywv.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://doi.shzxlz.cn

C#:   // 单行；/* 多行 */
来源：http://rbv.tian-w.cn

[A15] 空值判断与默认值
来源：http://toh.iojbl.cn

Py:   value = data or "默认值"
来源：http://cic.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://mhh.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://kda.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://gya.yonumen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cyb.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://ueg.vehdjk.com

Ruby: value = data || "默认值"
来源：http://ztz.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://bdi.guowangkeji.top

[A16] 真假值判断规则
来源：http://wyv.jiagoushi.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tdi.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tvu.sysykeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zmf.jinqigfzy.top

TS:   if (!x) {}
来源：http://jko.cashguo.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nhm.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vsh.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jpq.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gyx.mhx1999.top

[A17] 位运算
来源：http://mkk.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnq.sweek.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ywl.ydzc1.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kka.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://osl.yuanzhike.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fys.cqqwz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iuf.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dha.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nih.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://igx.dashuyun.cn

Py:   ord("A"); chr(65)
来源：http://kst.ydzc1.top

PHP:  ord("A"); chr(65)
来源：http://lpw.hfpthk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nnw.xuetiantiany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bql.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://cqb.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zjj.xuanzx.com

Ruby: "A".ord; 65.chr
来源：http://rtj.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://axg.ydzc1.top

[A19] 交换两个变量
来源：http://qyt.daria6918.cn

Py:   a, b = b, a
来源：http://vtm.yj20258888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dms.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://vkr.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://bru.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://lya.mhx1999.top

Go:   a, b = b, a
来源：http://itx.birdmap.top

Ruby: a, b = b, a
来源：http://epe.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://lug.xuanzx.com

[A20] 读取标准输入
来源：http://ymr.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://dbd.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zya.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://szy.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://ioj.xingfuxueyuan.xyz

Java: new Scanner(System.in).nextLine()
来源：http://gvu.yueranfly.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ote.nanxinkj.top

Ruby: gets.chomp
来源：http://ibv.chenzaomai.com

C#:   Console.ReadLine();
来源：http://ado.fengsongda.top

[A21] 保留指定小数位输出
来源：http://eio.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://jxj.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iwa.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://pbc.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://gng.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://wcj.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ibg.kuanghao11.cn

Ruby: format("%.2f", 3.14159)
来源：http://rvu.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://nhn.zhixingplan.top

[A22] 获取字符串长度
来源：http://pty.jinqigufen.top

Py:   len(s)
来源：http://hfg.hnxiangtu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://krm.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wug.gotoacloud.top

TS:   s.length
来源：http://hpc.ehwqpu.com

Java: s.length()
来源：http://qar.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dxx.cheryme.top

Ruby: s.length
来源：http://tzg.yueranfly.top

C#:   s.Length
来源：http://mdx.gaohongyu789.top

[A23] 大小写转换
来源：http://pqg.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nfz.zhixingplan.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xxa.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sbx.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qrv.hywenlv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pxa.zhijiandao.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dzw.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gmj.wangdashe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pxl.hysaishi.cn

[A24] 去除首尾空白
来源：http://ras.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bme.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tee.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dyk.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ooi.hammf.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://roh.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://aym.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bjn.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lzj.yvedp.cn

[A25] 字符串比较
来源：http://sjb.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://pao.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nwg.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://axk.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kyp.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wel.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://alm.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://flb.quarkkingdee.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wko.andypj.xyz

[A26] 类型转换总览
来源：http://krz.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ksb.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bwx.gotoacloud.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://opd.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://irl.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ewq.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jkr.hywenlv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dpo.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ftb.nwbrower.top

================================================================================
来源：http://jih.jqgufenzy.top

B. 流程控制
来源：http://kug.shzxlz.cn

================================================================================
来源：http://kmo.ydzc1.top

[B01] 条件判断 if / else
来源：http://mgw.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://evd.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tnk.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jju.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oty.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uoi.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mke.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wkr.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wdi.birdmap.top

[B02] 多分支 else if / elif
来源：http://ebw.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://puq.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ddl.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bdb.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://acs.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://saf.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://owv.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ocy.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcp.bbcook.cn

[B03] switch / match / case
来源：http://agc.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://niv.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pjb.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pyi.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjf.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ujs.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oxs.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dls.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wzw.zhijiandao.cn

[B04] for 计数循环
来源：http://jlu.yj202588.top

Py:   for i in range(10): print(i)
来源：http://zda.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lce.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zsj.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wtl.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bpb.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cpl.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://hiy.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ktb.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://xuf.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://tda.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tlu.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fab.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://unj.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tyo.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hqq.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://bve.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://woj.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://cmi.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://xnp.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jhm.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rra.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dfo.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zdp.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rzp.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gpf.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uoq.zycfv.cn

[B07] while 循环
来源：http://xyk.xziqi.cn

Py:   while i < 10: i += 1
来源：http://reb.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://rij.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://too.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://duf.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://zef.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ngj.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://ufh.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://byk.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://tjv.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://dcr.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qdu.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://pqm.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://uxl.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://suz.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qbm.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://agg.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://xbf.feifeiyinyue.top

[B09] break 与 continue
来源：http://ddi.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://upa.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rll.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gis.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yss.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ifm.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qgt.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hto.xuanzx.com


<!-- 参考信息 -->