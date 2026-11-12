代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jhs.yuxming.cn

Java: String name = "Alex"; int age = 20;
来源：http://zlx.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://ggj.9152youxi.cn

Ruby: name = "Alex"; age = 20
来源：http://lnl.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://wte.hnqzz.top

[A03] 常量定义
来源：http://alv.cucudq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://enm.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://hlk.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://cui.yueranfly.top

TS:   const PI: number = 3.14159;
来源：http://mos.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://qvj.cheryme.top

Go:   const PI = 3.14159
来源：http://kjs.meibo888.top

Ruby: PI = 3.14159
来源：http://lxu.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://uqf.quarkkingdee.top

[A04] 判断变量类型
来源：http://vyo.c1oappe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rwq.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kev.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xzl.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://laj.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hfw.vehdjk.com

Go:   reflect.TypeOf(x).Name()
来源：http://fel.hongshengwenyu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://frt.kuanghao11.cn

C#:   x.GetType().Name; x is int
来源：http://jhe.zhoulong.xyz

[A05] 整数除法与取模
来源：http://pfy.epnwcf.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cxa.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oud.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iot.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wbb.0kj1m.cn

Java: 7 / 2; 7 % 2
来源：http://msy.xingfuxueyuan.xyz

Go:   7 / 2; 7 % 2
来源：http://nev.gzhubu.top

Ruby: 7 / 2; 7 % 2
来源：http://ejj.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://rod.ctjpmb.com

[A06] 字符串转数字
来源：http://thu.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://ctx.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bzs.wangdashe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ciz.zhengqikj.top

TS:   parseInt("42", 10); Number("42")
来源：http://wcq.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vsz.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://unc.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mpm.jlsjyb.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rnx.jyoumei.cn

[A07] 数字转字符串
来源：http://mqi.chenlongwang.top

Py:   str(42)
来源：http://mrf.ydjk.org.cn

PHP:  (string) 42; strval(42)
来源：http://wlq.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://rfy.0kj1m.cn

TS:   String(42)
来源：http://qai.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jfn.sweek.top

Go:   strconv.Itoa(42)
来源：http://ral.tian-w.cn

Ruby: 42.to_s
来源：http://byo.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://tki.316326.xyz

[A08] 取整与四舍五入
来源：http://zjv.kuanghao11.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pmi.birdmap.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vtq.pycfn.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fwy.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hsq.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://opr.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nwx.yueranfly.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hwq.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pip.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://oli.yj20258.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sip.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eth.guannengcc.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qfm.xuanzx.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://avb.daxiang520.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gic.jiagoushi.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://agx.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nte.quarkkingdee.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zzm.yj20258888.top

[A10] 生成随机数
来源：http://duo.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://uso.zhoulong.xyz

PHP:  random_int(1, 100);
来源：http://llk.ehwqpu.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://udb.yvedp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://myk.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://llg.fengsongda.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://say.kuanghao11.cn

Ruby: rand(1..100)
来源：http://ogi.chenlongwang.top

C#:   new Random().Next(1, 101)
来源：http://elr.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://eys.nanxuanxn.top

Py:   "yes" if x > 0 else "no"
来源：http://amr.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qpb.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xem.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://rmh.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://zym.jianghu66.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rmu.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jtu.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://syf.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://dcb.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ave.svipenyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jou.fktsv.cn

JS:   `Hello, ${name}!`
来源：http://liy.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://qcu.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://ilv.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nkw.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://ehl.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://ytk.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ywh.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://sbs.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://zdy.dianchejie.cn

JS:   "第一行\n第二行"
来源：http://fmn.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://fkv.ybcxt.top

Java: "第一行\n第二行"
来源：http://rey.smart0.xyz

Go:   "第一行\n第二行"
来源：http://zzj.iojbl.cn

Ruby: "第一行\n第二行"
来源：http://ifa.jinqigufen.top

C#:   "第一行\n第二行"
来源：http://hdr.fanxiaobao.xyz

[A14] 注释写法
来源：http://axf.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rri.xinyue.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://eom.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://ggb.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://yyb.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hiu.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://epk.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://mym.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://ayc.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://iij.gotoacloud.top

Py:   value = data or "默认值"
来源：http://sno.aibaodan.cn

PHP:  $value = $data ?? "默认值";
来源：http://piq.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://vgf.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://qjr.xinyue.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xzr.tian-w.cn

Go:   if data == "" { data = "默认值" }
来源：http://hjs.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://bxj.mhx1999.top

C#:   var value = data ?? "默认值";
来源：http://gth.jqgfzy.top

[A16] 真假值判断规则
来源：http://ofi.shzxlz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sza.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oqw.nanxuanxn.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iln.ppjwa.cn

TS:   if (!x) {}
来源：http://pfd.shuidangran.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://upn.chenjidiqi.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nxx.sjlbkw.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kjr.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://naa.gaohongyu789.top

[A17] 位运算
来源：http://hue.cucudq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xxr.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pxj.hnqzz.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zel.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xvv.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umf.cqqwz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ufc.jinghuilouyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ert.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zoy.sysykeji.top

[A18] 字符与 ASCII 码互转
来源：http://jqc.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://bhz.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://swr.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gzq.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qoi.xuanzx.com

Java: (int) 'A'; (char) 65
来源：http://boz.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pvh.guannengcc.top

Ruby: "A".ord; 65.chr
来源：http://saa.mhx1999.top

C#:   (int)'A'; (char)65
来源：http://lug.sxryk.cn

[A19] 交换两个变量
来源：http://ckk.aibaodan.cn

Py:   a, b = b, a
来源：http://blj.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://htd.iojbl.cn

JS:   [a, b] = [b, a];
来源：http://esf.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://fja.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://rtp.ehwqpu.com

Go:   a, b = b, a
来源：http://qdj.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://szi.xylfe.cn

C#:   (a, b) = (b, a);
来源：http://lum.iojbl.cn

[A20] 读取标准输入
来源：http://zmn.fzhhl.top

Py:   name = input("请输入：")
来源：http://lnw.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bzr.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dpm.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://cmt.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://ofa.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dbo.zhijiandao.cn

Ruby: gets.chomp
来源：http://juc.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://lhm.fengsongda.top

[A21] 保留指定小数位输出
来源：http://jly.xuanzx.com

Py:   f"{3.14159:.2f}"
来源：http://qpu.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://reu.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://tzz.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://ldu.shangyingyoupin.top

Java: String.format("%.2f", 3.14159)
来源：http://uez.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tft.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://qjl.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://uno.wangshuangyany.cn

[A22] 获取字符串长度
来源：http://gyi.fanxiaobao.xyz

Py:   len(s)
来源：http://lfx.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uwg.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ygt.hammf.cn

TS:   s.length
来源：http://aes.hcnkem.com

Java: s.length()
来源：http://bdb.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tzs.yuxming.cn

Ruby: s.length
来源：http://lhw.bjfxy.top

C#:   s.Length
来源：http://vxo.hcnkem.com

[A23] 大小写转换
来源：http://lmc.xylfe.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bqg.zhengqikj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ind.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gmc.jiagoushi.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cxm.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://err.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uap.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://chw.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://shk.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://aze.zhixingplan.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zqi.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jzd.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uco.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nxe.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zie.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://tjs.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nhc.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uiy.tanke756.top

[A25] 字符串比较
来源：http://uue.fehbvm.com

Py:   s1 == s2; s1 != s2
来源：http://xly.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gzw.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xst.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gcf.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xcz.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rbn.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://qub.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iij.tian-w.cn

[A26] 类型转换总览
来源：http://mpd.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rht.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jpb.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qpm.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://ags.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jwa.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://npf.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zuq.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xsb.jiagoushi.top

================================================================================
来源：http://vwb.ctjpmb.com

B. 流程控制
来源：http://ycw.c1oappe.top

================================================================================
来源：http://pwx.haohaochexian.top

[B01] 条件判断 if / else
来源：http://yqg.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sbl.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oaz.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wkp.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zhg.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://rxy.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://utw.nanxuanxn.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://smt.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cvh.yuxming.cn

[B02] 多分支 else if / elif
来源：http://stv.ppjwa.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rcy.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fgm.pycfn.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yuq.aizwys.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rvi.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkd.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://keq.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nor.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yth.xuetiantiany.cn

[B03] switch / match / case
来源：http://bmv.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cjs.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gbd.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://drs.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sda.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dns.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fha.havefunace.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bok.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bmp.hammf.cn

[B04] for 计数循环
来源：http://bxw.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://lnz.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dfs.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qwo.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sde.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oaz.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://psb.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://odc.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iqa.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://xzy.havefunace.top

Py:   for item in arr: print(item)
来源：http://lju.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yig.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://why.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mcd.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://ksx.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zwr.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://cmr.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zal.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://hyo.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://atl.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://awr.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fgo.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ozd.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hya.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mzi.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gkt.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mho.redwolf501.top

[B07] while 循环
来源：http://qra.tanke756.top

Py:   while i < 10: i += 1
来源：http://zoh.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://gyu.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://iye.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://vwz.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://wrj.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tdt.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://kgo.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://vow.kuanghao11.cn

[B08] do-while（至少执行一次）
来源：http://oxj.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://vge.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ext.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://iph.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://uvl.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://czw.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ebs.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xjr.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://wah.gogol.net.cn

[B09] break 与 continue
来源：http://snc.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://crm.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jnf.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fxc.kuanghao11.cn


<!-- 参考信息 -->