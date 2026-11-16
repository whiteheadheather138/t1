代发 wailian999

[A02] 变量声明与赋值
来源：http://bwk.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bjg.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://tcf.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://ndf.xylfe.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ktw.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://dda.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://ifh.cashguo.top

Ruby: name = "Alex"; age = 20
来源：http://xeb.hnxiangtu.top

C#:   string name = "Alex"; int age = 20;
来源：http://apz.xylfe.cn

[A03] 常量定义
来源：http://yhr.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xqe.tianlin.xyz

PHP:  const PI = 3.14159;
来源：http://dta.zhoulong.xyz

JS:   const PI = 3.14159;
来源：http://fvk.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://cog.tarul.cn

Java: static final double PI = 3.14159;
来源：http://ijk.yj20258888.top

Go:   const PI = 3.14159
来源：http://dso.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://vzd.yangfankeji.com

C#:   const double PI = 3.14159;
来源：http://mhu.pengpengdd.cyou

[A04] 判断变量类型
来源：http://xlv.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nbp.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://drc.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://juk.cqqwz.cn

TS:   typeof x; x instanceof Date
来源：http://ehq.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dnx.wangdashe.top

Go:   reflect.TypeOf(x).Name()
来源：http://ptb.zhijiandao.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dsy.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://lei.cucudq.cn

[A05] 整数除法与取模
来源：http://hja.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vfv.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pnp.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tob.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ovb.sxryk.cn

Java: 7 / 2; 7 % 2
来源：http://ptg.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://xts.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://iob.kuanghao11.cn

C#:   7 / 2; 7 % 2
来源：http://pyw.fanxiaobao.xyz

[A06] 字符串转数字
来源：http://aem.sweek.top

Py:   int("42"); float("3.14")
来源：http://sgi.havefunace.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pdf.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cgl.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://byx.fzhhl.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bmg.tianlin.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fyo.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ysq.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bef.sweek.top

[A07] 数字转字符串
来源：http://tlq.yanxiufei.cn

Py:   str(42)
来源：http://vbt.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://odm.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://zrr.daxiang520.top

TS:   String(42)
来源：http://vrn.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qdc.tanke756.top

Go:   strconv.Itoa(42)
来源：http://ftz.jqgufenzy.top

Ruby: 42.to_s
来源：http://hvl.zhoulong.xyz

C#:   42.ToString()
来源：http://gpw.zhaomingkeji.xyz

[A08] 取整与四舍五入
来源：http://qlt.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ulh.shanyushiyangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fxe.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bae.iojbl.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nar.cdnleiting.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zyl.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bie.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://byn.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://chh.quarkkingdee.top

[A09] 绝对值与最大最小值
来源：http://kmp.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://npt.sysykeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dud.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yul.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iut.chenlongwang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ode.xylfe.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xoi.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oel.yvedp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ddm.mhx1999.top

[A10] 生成随机数
来源：http://ljz.yvedp.cn

Py:   import random; random.randint(1, 100)
来源：http://vgw.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://sgs.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ddn.52xcode.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rgf.uphjek.com

Java: new Random().nextInt(100) + 1
来源：http://fic.ywan-chungtsiang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mbb.jqgfzy.top

Ruby: rand(1..100)
来源：http://jkk.sweek.top

C#:   new Random().Next(1, 101)
来源：http://ndy.bbcook.cn

[A11] 条件表达式（三元）
来源：http://tlc.yangfankeji.com

Py:   "yes" if x > 0 else "no"
来源：http://trr.fzhhl.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://aqc.chenzaomai.com

JS:   x > 0 ? "yes" : "no"
来源：http://ttz.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://qqj.hammf.cn

Java: x > 0 ? "yes" : "no"
来源：http://jpo.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fyr.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pue.shanyushiyangtech.top

C#:   x > 0 ? "yes" : "no"
来源：http://oji.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://cbm.ehwqpu.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wbc.cdnleiting.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rlo.hnxiangtu.top

JS:   `Hello, ${name}!`
来源：http://unn.52xcode.cn

TS:   `Hello, ${name}!`
来源：http://iqp.shzxlz.cn

Java: "Hello, %s!".formatted(name)
来源：http://sqb.fengsongda.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xpu.havefunace.top

Ruby: "Hello, #{name}!"
来源：http://apb.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://xdj.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hxp.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://qjs.9152youxi.cn

PHP:  "第一行\n第二行"
来源：http://vsd.tian-w.cn

JS:   "第一行\n第二行"
来源：http://loz.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://mfh.yvedp.cn

Java: "第一行\n第二行"
来源：http://zuu.gzhubu.top

Go:   "第一行\n第二行"
来源：http://uuc.hnxiangtu.top

Ruby: "第一行\n第二行"
来源：http://fch.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://dvk.xuanzx.com

[A14] 注释写法
来源：http://hrs.xingfuxueyuan.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://sdx.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hte.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://hjq.hesvh.cn

TS:   // 单行；/* 多行 */
来源：http://kbr.yonumen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rue.hesvh.cn

Go:   // 单行；/* 多行 */
来源：http://sdl.shangyingyoupin.top

Ruby: # 单行；=begin 多行 =end
来源：http://ryr.jinqigfzy.top

C#:   // 单行；/* 多行 */
来源：http://juv.daria6918.cn

[A15] 空值判断与默认值
来源：http://zbl.ybcxt.top

Py:   value = data or "默认值"
来源：http://cng.0kj1m.cn

PHP:  $value = $data ?? "默认值";
来源：http://ynn.zycfv.cn

JS:   const value = data ?? "默认值";
来源：http://brx.wangdashe.top

TS:   const value = data ?? "默认值";
来源：http://dxp.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kor.zhijiandao.cn

Go:   if data == "" { data = "默认值" }
来源：http://ktj.fengsongda.top

Ruby: value = data || "默认值"
来源：http://txb.cheryme.top

C#:   var value = data ?? "默认值";
来源：http://yiv.cucudq.cn

[A16] 真假值判断规则
来源：http://hlh.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://erx.yj202588.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ztp.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ypa.xylfe.cn

TS:   if (!x) {}
来源：http://pez.xziqi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uqh.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lru.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://emh.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tcg.dianchejie.cn

[A17] 位运算
来源：http://tyo.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eob.hywenlv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dwp.dashuyun.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cny.ybcxt.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dai.gogol.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pcj.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nfl.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wvv.meibo888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cal.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://wxt.vqdsnc.cn

Py:   ord("A"); chr(65)
来源：http://suc.snrcjt.cn

PHP:  ord("A"); chr(65)
来源：http://axq.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rdc.0kj1m.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fqa.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://qka.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tzu.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://vut.sjlbkw.cn

C#:   (int)'A'; (char)65
来源：http://que.nwbrower.top

[A19] 交换两个变量
来源：http://frn.c1oappe.top

Py:   a, b = b, a
来源：http://eua.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://yso.cashguo.top

JS:   [a, b] = [b, a];
来源：http://exs.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://byv.sufxvd.cn

Java: int t = a; a = b; b = t;
来源：http://ctl.jyoumei.cn

Go:   a, b = b, a
来源：http://njd.svipenyu.cn

Ruby: a, b = b, a
来源：http://kgq.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://xqs.cdnleiting.top

[A20] 读取标准输入
来源：http://hix.zdbjq.cn

Py:   name = input("请输入：")
来源：http://kls.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qut.yonumen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://guo.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://pwh.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://mcn.tarul.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gsn.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://wit.bbcook.cn

C#:   Console.ReadLine();
来源：http://gku.vehdjk.com

[A21] 保留指定小数位输出
来源：http://sev.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://wpu.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mwk.jlsjyb.cn

JS:   (3.14159).toFixed(2)
来源：http://wtd.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://msp.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://mna.zycfv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ett.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://vpc.wangdashe.top

C#:   3.14159.ToString("F2")
来源：http://jtm.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://ddh.shzxlz.cn

Py:   len(s)
来源：http://vhy.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hus.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://weo.gzhubu.top

TS:   s.length
来源：http://cko.jinqigufen.top

Java: s.length()
来源：http://duk.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dyp.jinyuanbaomall.cn

Ruby: s.length
来源：http://xbw.epnwcf.com

C#:   s.Length
来源：http://ujr.jyoumei.cn

[A23] 大小写转换
来源：http://gkf.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vlg.gotoacloud.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://onu.fanxiaobao.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eai.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vxi.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cjp.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bxj.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bwd.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://smj.hysaishi.cn

[A24] 去除首尾空白
来源：http://ioc.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bfw.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xxn.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zvj.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dam.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ywx.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://uhu.hcnkem.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://myy.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ann.shangyingyoupin.top

[A25] 字符串比较
来源：http://riy.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://fde.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://clj.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wcb.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mkh.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cwl.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ubs.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://wdn.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ehn.yj202588.top

[A26] 类型转换总览
来源：http://qel.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://enk.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hog.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xsh.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://xcf.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zrh.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wsg.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xke.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://emt.vehdjk.com

================================================================================
来源：http://hwr.yuxming.cn

B. 流程控制
来源：http://ccy.hcnkem.com

================================================================================
来源：http://ysm.ctjpmb.com

[B01] 条件判断 if / else
来源：http://dza.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://pav.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qow.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dmm.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://par.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://udf.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lec.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gbq.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qey.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://usn.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xel.52xcode.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gzb.epnwcf.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osf.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmj.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgr.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gxl.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jsv.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tuw.jinqigfzy.top

[B03] switch / match / case
来源：http://nvr.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ote.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oba.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ira.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://imt.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uiy.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lur.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tll.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ubk.gaohongyu789.top

[B04] for 计数循环
来源：http://lge.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://bcw.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yit.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://prn.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://whz.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://whd.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hpq.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://jqi.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sqj.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://zfi.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://wtc.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kyp.jqgufenzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ufx.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://fym.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rmg.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yct.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://fsj.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cqf.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://wxi.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tfh.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://avh.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fdi.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mwg.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fts.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uri.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uxv.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://coa.gotoacloud.top

[B07] while 循环
来源：http://rbs.fehbvm.com

Py:   while i < 10: i += 1
来源：http://hsm.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://yzh.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://gav.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://iqy.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://lbe.dianchejie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ogx.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://oup.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://jdn.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://vag.yj202588.top

Py:   # 无 do-while：用 while True + break
来源：http://mfx.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hvr.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://rbb.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://bkp.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://exh.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fxu.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tho.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://vdv.svipenyu.cn


<!-- 参考信息 -->