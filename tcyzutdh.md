代发 wailian999

JS:   const PI = 3.14159;
来源：http://gwf.316326.xyz

TS:   const PI: number = 3.14159;
来源：http://dbe.tianlin.xyz

Java: static final double PI = 3.14159;
来源：http://vwu.ctjpmb.com

Go:   const PI = 3.14159
来源：http://ktn.tian-w.cn

Ruby: PI = 3.14159
来源：http://ckl.tanke756.top

C#:   const double PI = 3.14159;
来源：http://ilt.vqdsnc.cn

[A04] 判断变量类型
来源：http://bzy.xinyue.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://ynk.yuanzhike.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pmy.ivvv.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fbp.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://hnl.xingfuxueyuan.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qax.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://ati.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gvo.pycfn.com

C#:   x.GetType().Name; x is int
来源：http://ogb.zhongyouzk.top

[A05] 整数除法与取模
来源：http://ejv.wangshuangyany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xow.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bfv.smart0.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xdv.nwbrower.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ngr.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://nvt.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://xea.zdbjq.cn

Ruby: 7 / 2; 7 % 2
来源：http://cwr.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://ydh.yvedp.cn

[A06] 字符串转数字
来源：http://jzj.redwolf501.top

Py:   int("42"); float("3.14")
来源：http://urv.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tvi.xinyue.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ggu.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bpm.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zts.hysaishi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://otw.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://llf.316326.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://chm.jinqigufen.top

[A07] 数字转字符串
来源：http://ddz.bjfxy.top

Py:   str(42)
来源：http://qqo.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://dkf.sysykeji.top

JS:   String(42); (42).toString()
来源：http://hjg.xuetiantiany.cn

TS:   String(42)
来源：http://iwh.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wxi.redwolf501.top

Go:   strconv.Itoa(42)
来源：http://txp.wangdashe.top

Ruby: 42.to_s
来源：http://txg.smart0.xyz

C#:   42.ToString()
来源：http://duu.sjlbkw.cn

[A08] 取整与四舍五入
来源：http://itc.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bvs.guowangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zmh.chenjidiqi.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qkv.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mbn.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kkn.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cra.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xvs.ydjk.org.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://irl.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://ilr.nanxuanxn.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nzl.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gis.nwbrower.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zgf.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nmp.c1oappe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cjk.andypj.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xac.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wsw.zhengqikj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mvg.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://zgd.shzxlz.cn

Py:   import random; random.randint(1, 100)
来源：http://aof.cheryme.top

PHP:  random_int(1, 100);
来源：http://oik.xylfe.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xyk.tarul.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hmc.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://rhw.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bzx.hywenlv.cn

Ruby: rand(1..100)
来源：http://hbt.jianghu66.top

C#:   new Random().Next(1, 101)
来源：http://ypp.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://dgz.epnwcf.com

Py:   "yes" if x > 0 else "no"
来源：http://yaz.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://rwg.hesvh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tvm.epnwcf.com

TS:   x > 0 ? "yes" : "no"
来源：http://ybo.yvedp.cn

Java: x > 0 ? "yes" : "no"
来源：http://jrc.havefunace.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sjs.xingfuxueyuan.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://zhg.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://tpo.yuanzhike.top

[A12] 字符串插值 / 格式化
来源：http://oeu.quarkkingdee.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mmd.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wgg.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://snx.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://dgd.ehwqpu.com

Java: "Hello, %s!".formatted(name)
来源：http://ecg.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ofh.sxryk.cn

Ruby: "Hello, #{name}!"
来源：http://big.yonumen.top

C#:   $"Hello, {name}!"
来源：http://eko.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cia.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://tyg.wangshuangyany.cn

PHP:  "第一行\n第二行"
来源：http://zgv.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://ooc.ivvv.top

TS:   "第一行\n第二行"
来源：http://pvi.shzxlz.cn

Java: "第一行\n第二行"
来源：http://dll.zhaomingkeji.xyz

Go:   "第一行\n第二行"
来源：http://ueg.jiagoushi.top

Ruby: "第一行\n第二行"
来源：http://qro.ydzc1.top

C#:   "第一行\n第二行"
来源：http://eis.andypj.xyz

[A14] 注释写法
来源：http://rof.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zvf.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://bsl.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://jra.andypj.xyz

TS:   // 单行；/* 多行 */
来源：http://uyd.316326.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xrr.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://sqo.chenlongwang.top

Ruby: # 单行；=begin 多行 =end
来源：http://ayk.ydzc1.top

C#:   // 单行；/* 多行 */
来源：http://phm.sweek.top

[A15] 空值判断与默认值
来源：http://zva.jianghu66.top

Py:   value = data or "默认值"
来源：http://tkf.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://hxa.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://lle.fehbvm.com

TS:   const value = data ?? "默认值";
来源：http://dsl.gogol.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yci.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://mxx.dianchejie.cn

Ruby: value = data || "默认值"
来源：http://vfg.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://npq.cheryme.top

[A16] 真假值判断规则
来源：http://gbc.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://icx.sxryk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vae.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vcr.zhongyouzk.top

TS:   if (!x) {}
来源：http://wsg.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://okc.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dyr.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://xmf.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bnb.hammf.cn

[A17] 位运算
来源：http://hus.gogol.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://apk.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mlg.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vyh.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nhn.gaohongyu789.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rip.chenzaomai.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://car.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qti.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dqf.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://fzy.xziqi.cn

Py:   ord("A"); chr(65)
来源：http://ysb.cqqwz.cn

PHP:  ord("A"); chr(65)
来源：http://pxz.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qke.jqgufenzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ush.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://zkj.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://chv.yj202588.top

Ruby: "A".ord; 65.chr
来源：http://zjc.aibaodan.cn

C#:   (int)'A'; (char)65
来源：http://chm.jyoumei.cn

[A19] 交换两个变量
来源：http://lbp.mhx1999.top

Py:   a, b = b, a
来源：http://ems.0kj1m.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tpj.tanke756.top

JS:   [a, b] = [b, a];
来源：http://wgx.vqdsnc.cn

TS:   [a, b] = [b, a];
来源：http://qsp.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://xkv.zhiwuduotai.top

Go:   a, b = b, a
来源：http://yws.shzxlz.cn

Ruby: a, b = b, a
来源：http://paa.yj202588.top

C#:   (a, b) = (b, a);
来源：http://fni.cdnleiting.top

[A20] 读取标准输入
来源：http://kdc.birdmap.top

Py:   name = input("请输入：")
来源：http://uhj.iojbl.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dsc.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ymw.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://bvk.hammf.cn

Java: new Scanner(System.in).nextLine()
来源：http://noi.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://djc.wangshuangyany.cn

Ruby: gets.chomp
来源：http://eje.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://flv.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://nli.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://ssq.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fmg.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://rak.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://zft.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://czu.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xhv.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://jsx.sweek.top

C#:   3.14159.ToString("F2")
来源：http://evb.sufxvd.cn

[A22] 获取字符串长度
来源：http://mjj.uphjek.com

Py:   len(s)
来源：http://bgq.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ujj.nwbrower.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dxk.hfpthk.cn

TS:   s.length
来源：http://oxo.haohaochexian.top

Java: s.length()
来源：http://ccr.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://omo.fehbvm.com

Ruby: s.length
来源：http://qwo.fzhhl.top

C#:   s.Length
来源：http://ppd.aibaodan.cn

[A23] 大小写转换
来源：http://xlr.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ind.jyoumei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ymt.zdqjudy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rlw.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ywn.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://etk.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zlw.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zde.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://asz.jqgfzy.top

[A24] 去除首尾空白
来源：http://osx.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ivp.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://arg.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hfj.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ixe.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ycc.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://tcf.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zzl.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qgt.hcnkem.com

[A25] 字符串比较
来源：http://fyu.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://hqh.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lqu.hammf.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://inn.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fag.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://laz.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://erg.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pqa.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://soo.jlsjyb.cn

[A26] 类型转换总览
来源：http://rkj.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zxp.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qex.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yqi.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://rbf.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ohh.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nqp.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://bow.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iub.jiagoushi.top

================================================================================
来源：http://gvk.epnwcf.com

B. 流程控制
来源：http://bpd.ehwqpu.com

================================================================================
来源：http://ces.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://bbo.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qdy.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sjs.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ikk.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rmk.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jel.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qjm.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rkz.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jcg.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://lbd.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vmu.kuanghao11.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uav.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkq.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dai.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyi.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cye.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vgd.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://esj.haohaochexian.top

[B03] switch / match / case
来源：http://plj.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pnf.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vsp.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vyd.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fuz.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://msh.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sav.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zfn.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://elc.yongpay.top

[B04] for 计数循环
来源：http://qio.yuanzhike.top

Py:   for i in range(10): print(i)
来源：http://ewt.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xic.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pew.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgj.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hal.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lke.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://rqz.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://deb.havefunace.top

[B05] 遍历数组 / 列表
来源：http://awq.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://rrv.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uyr.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qvb.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qdm.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://krx.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xro.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://qjf.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qab.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://oct.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xmj.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xyf.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hti.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lrj.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tdh.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ouk.wangdashe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yvo.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zmi.yj20258888.top

[B07] while 循环
来源：http://dke.uphjek.com

Py:   while i < 10: i += 1
来源：http://rer.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yof.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://mfk.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://jel.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://ffg.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ffi.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://pfk.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://vzz.bjfxy.top

[B08] do-while（至少执行一次）
来源：http://xus.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://ars.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pne.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://xvv.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://hxm.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://efs.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://thb.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://uvs.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://zuv.sysykeji.top

[B09] break 与 continue
来源：http://swj.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xnz.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qix.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnv.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pkv.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skz.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tqh.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ufu.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtw.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://uso.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qnh.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oxh.yuanzhike.top


<!-- 参考信息 -->