代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://xct.316326.xyz

[A03] 常量定义
来源：http://hhw.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ylo.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://jha.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://owi.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://doy.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://gqs.yj202588.top

Go:   const PI = 3.14159
来源：http://rjx.hnqzz.top

Ruby: PI = 3.14159
来源：http://wtf.havefunace.top

C#:   const double PI = 3.14159;
来源：http://mjk.mhx1999.top

[A04] 判断变量类型
来源：http://tru.bbcook.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://knr.fengsongda.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wmm.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ear.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://jgs.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://luc.wangshuangyany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uar.zycfv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zvg.hnxiangtu.top

C#:   x.GetType().Name; x is int
来源：http://exk.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://gwk.gzhubu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fjf.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mdm.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yun.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sdt.yj20258.top

Java: 7 / 2; 7 % 2
来源：http://qzk.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://rxg.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://mvk.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://iux.zhiwuduotai.top

[A06] 字符串转数字
来源：http://nba.yongpay.top

Py:   int("42"); float("3.14")
来源：http://dyl.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ldk.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jpv.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://sar.cqqwz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hjr.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fbd.sysykeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://omy.zhijiandao.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lzv.zhixingplan.top

[A07] 数字转字符串
来源：http://srh.nanxinkj.top

Py:   str(42)
来源：http://keo.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://lor.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://ptk.svipenyu.cn

TS:   String(42)
来源：http://mea.jqgufenzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hvf.hesvh.cn

Go:   strconv.Itoa(42)
来源：http://kwk.aizwys.cn

Ruby: 42.to_s
来源：http://yqd.yfazqb.com

C#:   42.ToString()
来源：http://kyt.jinqigufen.top

[A08] 取整与四舍五入
来源：http://xig.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eco.yuanzhike.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dkz.andypj.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ctf.chenzaomai.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yqw.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ubq.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lpv.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zsr.ivvv.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mao.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://dig.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zth.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ioa.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://enw.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uss.zhiwuduotai.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nmp.yvedp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xxw.cashguo.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cte.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yfs.smart0.xyz

[A10] 生成随机数
来源：http://yxn.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://qdz.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://gcy.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nxj.iojbl.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://npp.yanxiufei.cn

Java: new Random().nextInt(100) + 1
来源：http://ofb.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eff.nanxuanxn.top

Ruby: rand(1..100)
来源：http://uml.tianlin.xyz

C#:   new Random().Next(1, 101)
来源：http://yli.jqgfzy.top

[A11] 条件表达式（三元）
来源：http://kdj.ctjpmb.com

Py:   "yes" if x > 0 else "no"
来源：http://ebh.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ike.zhixingplan.top

JS:   x > 0 ? "yes" : "no"
来源：http://obb.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://urf.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://kzr.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://icf.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lhb.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://koq.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://sgd.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nga.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mec.chenzaomai.com

JS:   `Hello, ${name}!`
来源：http://bmm.kuanghao11.cn

TS:   `Hello, ${name}!`
来源：http://qso.jinghuilouyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://cjs.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jku.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://lje.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://xjp.nanxuanxn.top

[A13] 多行字符串（练习 \n 转义）
来源：http://apx.ydzc1.top

Py:   "第一行\n第二行"
来源：http://opa.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://tgl.hesvh.cn

JS:   "第一行\n第二行"
来源：http://lnl.xinyue.icu

TS:   "第一行\n第二行"
来源：http://fbj.yfazqb.com

Java: "第一行\n第二行"
来源：http://gme.cqqwz.cn

Go:   "第一行\n第二行"
来源：http://zwk.daria6918.cn

Ruby: "第一行\n第二行"
来源：http://wwl.cqqwz.cn

C#:   "第一行\n第二行"
来源：http://xbo.hcnkem.com

[A14] 注释写法
来源：http://kag.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gdg.jqgufenzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ybv.316326.xyz

JS:   // 单行；/* 多行 */
来源：http://heq.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://dzb.yuanzhike.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cno.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://vkl.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://hwy.jlsjyb.cn

C#:   // 单行；/* 多行 */
来源：http://jax.fengsongda.top

[A15] 空值判断与默认值
来源：http://fjk.fehbvm.com

Py:   value = data or "默认值"
来源：http://fln.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://kqr.guannengcc.top

JS:   const value = data ?? "默认值";
来源：http://qon.jinyuanbaomall.cn

TS:   const value = data ?? "默认值";
来源：http://xow.jiagoushi.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vjb.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://udw.tarul.cn

Ruby: value = data || "默认值"
来源：http://kml.hysaishi.cn

C#:   var value = data ?? "默认值";
来源：http://jqn.ehwqpu.com

[A16] 真假值判断规则
来源：http://lbq.yfazqb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ljd.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xax.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ftr.shanyushiyangtech.top

TS:   if (!x) {}
来源：http://ztc.vqdsnc.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mio.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rse.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://mzk.guannengcc.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xty.smart0.xyz

[A17] 位运算
来源：http://aqc.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yoj.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rkw.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mzn.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cvs.andypj.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cgl.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yhe.hnxiangtu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vkd.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sop.zhiwuduotai.top

[A18] 字符与 ASCII 码互转
来源：http://xxa.iojbl.cn

Py:   ord("A"); chr(65)
来源：http://lsm.yj202588.top

PHP:  ord("A"); chr(65)
来源：http://yqs.jyoumei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qnn.yuxming.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rif.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://pfm.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uga.jinqigufen.top

Ruby: "A".ord; 65.chr
来源：http://aov.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://bfn.ywan-chungtsiang.top

[A19] 交换两个变量
来源：http://hvc.xylfe.cn

Py:   a, b = b, a
来源：http://qwz.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://nkr.bbcook.cn

JS:   [a, b] = [b, a];
来源：http://xcb.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://hzb.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://hiq.chenzaomai.com

Go:   a, b = b, a
来源：http://dth.havefunace.top

Ruby: a, b = b, a
来源：http://zif.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://say.sweek.top

[A20] 读取标准输入
来源：http://gem.yvedp.cn

Py:   name = input("请输入：")
来源：http://unh.aibaodan.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://psz.svipenyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mgw.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://nhc.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://nny.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aux.havefunace.top

Ruby: gets.chomp
来源：http://ckr.yfazqb.com

C#:   Console.ReadLine();
来源：http://lds.xylfe.cn

[A21] 保留指定小数位输出
来源：http://otp.sufxvd.cn

Py:   f"{3.14159:.2f}"
来源：http://voo.ywan-chungtsiang.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xft.mhx1999.top

JS:   (3.14159).toFixed(2)
来源：http://squ.zhengqikj.top

TS:   (3.14159).toFixed(2)
来源：http://cas.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://ikc.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qtp.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://sqx.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://wvp.mhx1999.top

[A22] 获取字符串长度
来源：http://hqc.aizwys.cn

Py:   len(s)
来源：http://qwn.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eti.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lij.shanyushiyangtech.top

TS:   s.length
来源：http://gba.yj20258.top

Java: s.length()
来源：http://hjc.yj20258.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wxk.yj20258.top

Ruby: s.length
来源：http://gki.svipenyu.cn

C#:   s.Length
来源：http://zxo.9152youxi.cn

[A23] 大小写转换
来源：http://vuw.zhongyouzk.top

Py:   s.upper(); s.lower(); s.title()
来源：http://btl.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rph.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvb.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fqo.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bik.zhijiandao.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wuf.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xwo.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hxc.yueranfly.top

[A24] 去除首尾空白
来源：http://del.nanxuanxn.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fib.yj202588.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jau.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hwh.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://met.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://puw.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://jfn.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vky.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wpz.hywenlv.cn

[A25] 字符串比较
来源：http://utm.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://gag.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eqb.ppjwa.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fdo.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nxq.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vqq.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://spl.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gxm.yj20258.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ara.haohaochexian.top

[A26] 类型转换总览
来源：http://ncy.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qum.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bot.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sut.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://knh.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uch.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wgl.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uap.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nzi.jiagoushi.top

================================================================================
来源：http://qmj.yuxming.cn

B. 流程控制
来源：http://ftv.jqgufenzy.top

================================================================================
来源：http://ryn.guannengcc.top

[B01] 条件判断 if / else
来源：http://uym.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jxy.tanke756.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://twx.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ssm.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fds.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://izb.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aou.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nxw.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lhe.uphjek.com

[B02] 多分支 else if / elif
来源：http://usx.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dtr.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zld.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uog.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tul.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tao.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nqr.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aue.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xnc.hnxiangtu.top

[B03] switch / match / case
来源：http://yae.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qls.hfpthk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://unx.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gnk.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://doe.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sfy.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gyz.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wen.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://flw.fanxiaobao.xyz

[B04] for 计数循环
来源：http://qus.cheryme.top

Py:   for i in range(10): print(i)
来源：http://gpj.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bzx.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gru.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://csi.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xaf.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aih.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://skk.yvedp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ycd.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://bbl.yj20258888.top

Py:   for item in arr: print(item)
来源：http://fus.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rfu.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://phh.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://omm.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://szd.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pbh.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://brb.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sdg.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://rdy.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://hum.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hjl.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nxx.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qcm.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vam.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wpe.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ryz.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hon.tanke756.top

[B07] while 循环
来源：http://mzm.daxiang520.top

Py:   while i < 10: i += 1
来源：http://tar.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://sqd.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://gll.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://nar.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://luc.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rli.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://brf.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://saq.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://gkk.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://uct.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://maw.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://xkn.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://yet.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://ivd.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://egg.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xjj.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://aak.shanyushiyangtech.top

[B09] break 与 continue
来源：http://kkl.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rtn.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mre.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gud.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjm.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tgg.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cfe.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xno.jinqigfzy.top


<!-- 参考信息 -->