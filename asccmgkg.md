代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://yzt.bjfxy.top

[A03] 常量定义
来源：http://kcl.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://otr.jiagoushi.top

PHP:  const PI = 3.14159;
来源：http://bsp.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://mpy.hywenlv.cn

TS:   const PI: number = 3.14159;
来源：http://eco.ctjpmb.com

Java: static final double PI = 3.14159;
来源：http://sza.yanxiufei.cn

Go:   const PI = 3.14159
来源：http://iga.pycfn.com

Ruby: PI = 3.14159
来源：http://fdq.mhx1999.top

C#:   const double PI = 3.14159;
来源：http://mwu.nanxuanxn.top

[A04] 判断变量类型
来源：http://jub.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://eql.nanxuanxn.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ass.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oeh.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://ifu.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iur.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://xsw.chenlongwang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ynh.nanxuanxn.top

C#:   x.GetType().Name; x is int
来源：http://ipo.fktsv.cn

[A05] 整数除法与取模
来源：http://emx.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zzm.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://idc.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hhc.ivvv.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kwy.aibaodan.cn

Java: 7 / 2; 7 % 2
来源：http://zvg.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://fmn.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://avo.ivvv.top

C#:   7 / 2; 7 % 2
来源：http://hri.zdbjq.cn

[A06] 字符串转数字
来源：http://zdi.ywan-chungtsiang.top

Py:   int("42"); float("3.14")
来源：http://elj.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xis.tian-w.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://olr.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://hhd.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nof.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bbf.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wlm.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oma.birdmap.top

[A07] 数字转字符串
来源：http://beb.hysaishi.cn

Py:   str(42)
来源：http://bef.tian-w.cn

PHP:  (string) 42; strval(42)
来源：http://apv.nanxinkj.top

JS:   String(42); (42).toString()
来源：http://orv.nanxinkj.top

TS:   String(42)
来源：http://woi.cqqwz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://owb.ivvv.top

Go:   strconv.Itoa(42)
来源：http://yyq.havefunace.top

Ruby: 42.to_s
来源：http://rgv.smart0.xyz

C#:   42.ToString()
来源：http://pgr.uphjek.com

[A08] 取整与四舍五入
来源：http://dmy.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vxm.andypj.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ccw.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qhl.jqgfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xcz.wangshuangyany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lei.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ykl.hongshengwenyu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://akh.xingfuxueyuan.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rvc.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://ony.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vjc.chenjidiqi.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gdg.xylfe.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vsh.hongshengwenyu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wxq.nwbrower.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yxx.bjfxy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kct.jinghuilouyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pit.jlsjyb.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jzt.sufxvd.cn

[A10] 生成随机数
来源：http://cro.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://ufa.hcnkem.com

PHP:  random_int(1, 100);
来源：http://hxg.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jft.316326.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qfu.hywenlv.cn

Java: new Random().nextInt(100) + 1
来源：http://jmg.daria6918.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xcx.zhoulong.xyz

Ruby: rand(1..100)
来源：http://cjf.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://olg.cucudq.cn

[A11] 条件表达式（三元）
来源：http://uvc.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://zxq.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lnb.jinqigfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://hso.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://tzp.daxiang520.top

Java: x > 0 ? "yes" : "no"
来源：http://vea.sysykeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fvi.yj20258.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qnx.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://geh.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://exq.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hez.hesvh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lsz.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://inz.yonumen.top

TS:   `Hello, ${name}!`
来源：http://naq.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://hpp.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tnt.vqdsnc.cn

Ruby: "Hello, #{name}!"
来源：http://nxj.yongpay.top

C#:   $"Hello, {name}!"
来源：http://lwd.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tii.jlsjyb.cn

Py:   "第一行\n第二行"
来源：http://myp.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://lvt.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://fym.zhaomingkeji.xyz

TS:   "第一行\n第二行"
来源：http://zvn.316326.xyz

Java: "第一行\n第二行"
来源：http://gwy.snrcjt.cn

Go:   "第一行\n第二行"
来源：http://jjj.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://hzu.meibo888.top

C#:   "第一行\n第二行"
来源：http://mhc.sweek.top

[A14] 注释写法
来源：http://fez.0kj1m.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mxw.shangyingyoupin.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rth.jqgufenzy.top

JS:   // 单行；/* 多行 */
来源：http://nfn.ydjk.org.cn

TS:   // 单行；/* 多行 */
来源：http://ahm.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://awz.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://tpe.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nnq.xuetiantiany.cn

C#:   // 单行；/* 多行 */
来源：http://xtp.sysykeji.top

[A15] 空值判断与默认值
来源：http://yqx.mhx1999.top

Py:   value = data or "默认值"
来源：http://xzl.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://cyc.shzxlz.cn

JS:   const value = data ?? "默认值";
来源：http://ubk.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://xlq.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nij.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://tsg.yueranfly.top

Ruby: value = data || "默认值"
来源：http://tnt.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://sff.nanxuanxn.top

[A16] 真假值判断规则
来源：http://lxo.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ooy.hnqzz.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://paa.shzxlz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kzd.aibaodan.cn

TS:   if (!x) {}
来源：http://zra.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fxr.jiagoushi.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lvl.zhiwuduotai.top

Ruby: unless x            # nil 与 false 为假
来源：http://eiw.yuxming.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ifs.sufxvd.cn

[A17] 位运算
来源：http://uru.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nch.bjfxy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dvg.quarkkingdee.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ywf.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uuq.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xny.chenlongwang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rih.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ivq.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvm.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://msh.tianlin.xyz

Py:   ord("A"); chr(65)
来源：http://kxa.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://hol.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wmm.yvedp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://odo.bjfxy.top

Java: (int) 'A'; (char) 65
来源：http://hyc.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xqt.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://pqt.yueranfly.top

C#:   (int)'A'; (char)65
来源：http://jdo.xuanzx.com

[A19] 交换两个变量
来源：http://alj.ydjk.org.cn

Py:   a, b = b, a
来源：http://qpn.iojbl.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wwg.sxryk.cn

JS:   [a, b] = [b, a];
来源：http://zdi.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://wtg.shanyushiyangkeji.top

Java: int t = a; a = b; b = t;
来源：http://aae.cashguo.top

Go:   a, b = b, a
来源：http://wmh.yanxiufei.cn

Ruby: a, b = b, a
来源：http://qwf.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://vju.hammf.cn

[A20] 读取标准输入
来源：http://gyi.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://fqh.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rve.gzhubu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kwd.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://ccf.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://qjt.yonumen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mpe.jqgfzy.top

Ruby: gets.chomp
来源：http://puz.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://fsv.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://thl.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://qfa.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://psm.zhiwuduotai.top

JS:   (3.14159).toFixed(2)
来源：http://zin.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://exv.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://yxt.bjfxy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lvy.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://gcu.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://aut.shzxlz.cn

[A22] 获取字符串长度
来源：http://skt.sweek.top

Py:   len(s)
来源：http://qyu.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yrr.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eqg.vqdsnc.cn

TS:   s.length
来源：http://vtu.shangyingyoupin.top

Java: s.length()
来源：http://eft.sysykeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cmk.zhixingplan.top

Ruby: s.length
来源：http://htc.sjlbkw.cn

C#:   s.Length
来源：http://dcl.cqqwz.cn

[A23] 大小写转换
来源：http://owf.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cky.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fex.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zio.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kzv.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tje.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nkx.zhiwuduotai.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yjh.xziqi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mnc.zhixingplan.top

[A24] 去除首尾空白
来源：http://msm.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://stv.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hah.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://scf.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xgw.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hot.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://jdt.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qim.svipenyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vrq.hysaishi.cn

[A25] 字符串比较
来源：http://vib.wangdashe.top

Py:   s1 == s2; s1 != s2
来源：http://aga.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rcb.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nsu.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wko.ivvv.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aou.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://suw.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ltu.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oyu.ybcxt.top

[A26] 类型转换总览
来源：http://bsz.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://svf.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aiy.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ycf.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://xrg.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vzd.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zqi.shzxlz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cuu.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yfa.cqqwz.cn

================================================================================
来源：http://hwx.aibaodan.cn

B. 流程控制
来源：http://kel.cheryme.top

================================================================================
来源：http://zjd.hammf.cn

[B01] 条件判断 if / else
来源：http://cee.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xkd.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://afk.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vio.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tdc.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dha.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ycq.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wjf.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tgr.nwbrower.top

[B02] 多分支 else if / elif
来源：http://bnq.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fjh.zhijiandao.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vvl.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://non.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydc.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yys.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vda.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://swm.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npx.fktsv.cn

[B03] switch / match / case
来源：http://plh.hysaishi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xav.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cnm.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oen.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tdi.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xai.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eko.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jkc.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rmq.bbcook.cn

[B04] for 计数循环
来源：http://kxx.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://kdi.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bfo.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zcr.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mum.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://afn.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hwt.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://mns.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lcm.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://gup.ydzc1.top

Py:   for item in arr: print(item)
来源：http://alf.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://orp.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vhb.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zhp.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tev.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kot.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://vvd.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vlb.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://zeu.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qbp.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rhl.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gzp.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://emx.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pgc.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kzl.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://myk.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nbk.zhoulong.xyz

[B07] while 循环
来源：http://bxk.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://qyn.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://ekc.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://pfi.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://ynq.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://fkn.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iav.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://ybr.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://xvf.yj202588.top

[B08] do-while（至少执行一次）
来源：http://gnc.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://rqh.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tvs.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://qaz.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://gwy.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://fls.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dny.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://ilw.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://nsa.chenzaomai.com

[B09] break 与 continue
来源：http://fmt.yj20258.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ben.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zji.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfw.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pin.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdj.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://agb.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rrd.shanyushiyangkeji.top


<!-- 参考信息 -->