代发 wailian999

JS:   const PI = 3.14159;
来源：http://zys.yuxming.cn

TS:   const PI: number = 3.14159;
来源：http://quw.feifeiyinyue.top

Java: static final double PI = 3.14159;
来源：http://agg.hcnkem.com

Go:   const PI = 3.14159
来源：http://bdn.jqgfzy.top

Ruby: PI = 3.14159
来源：http://dmc.shzxlz.cn

C#:   const double PI = 3.14159;
来源：http://tpi.jinghuilouyu.cn

[A04] 判断变量类型
来源：http://sty.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jaf.feifeiyinyue.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://unj.svipenyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kbe.xuetiantiany.cn

TS:   typeof x; x instanceof Date
来源：http://fdx.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://csm.yuxming.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bpf.jqgfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ibp.smart0.xyz

C#:   x.GetType().Name; x is int
来源：http://glm.bbcook.cn

[A05] 整数除法与取模
来源：http://gbn.sweek.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yzd.9152youxi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rsa.bjfxy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iab.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hec.yj20258.top

Java: 7 / 2; 7 % 2
来源：http://log.tarul.cn

Go:   7 / 2; 7 % 2
来源：http://fbp.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://kyf.yangfankeji.com

C#:   7 / 2; 7 % 2
来源：http://zlu.nwbrower.top

[A06] 字符串转数字
来源：http://opc.andypj.xyz

Py:   int("42"); float("3.14")
来源：http://vce.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zcq.yangfankeji.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nmu.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://jyb.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nnw.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uvj.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gbi.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://urt.zhijiandao.cn

[A07] 数字转字符串
来源：http://xhk.yangfankeji.com

Py:   str(42)
来源：http://mez.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://kfb.tanke756.top

JS:   String(42); (42).toString()
来源：http://qqk.jqgufenzy.top

TS:   String(42)
来源：http://nbp.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vrh.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://dbh.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://elt.yvedp.cn

C#:   42.ToString()
来源：http://fgi.bjfxy.top

[A08] 取整与四舍五入
来源：http://gjn.daria6918.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://czs.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dci.sjlbkw.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kfl.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bdq.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sdh.hfpthk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mup.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://icb.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://epw.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://zal.chenlongwang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yzb.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jhj.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xgq.smart0.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fxu.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oqg.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dcx.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vxv.zhixingplan.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://izk.hongshengwenyu.top

[A10] 生成随机数
来源：http://mfg.tianlin.xyz

Py:   import random; random.randint(1, 100)
来源：http://czj.sysykeji.top

PHP:  random_int(1, 100);
来源：http://xxd.wangshuangyany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nmq.nanxinkj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rry.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://pab.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ojf.cucudq.cn

Ruby: rand(1..100)
来源：http://hjy.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://ppz.cheryme.top

[A11] 条件表达式（三元）
来源：http://jqx.wangshuangyany.cn

Py:   "yes" if x > 0 else "no"
来源：http://wyf.fzhhl.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ocf.cdnleiting.top

JS:   x > 0 ? "yes" : "no"
来源：http://kfm.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gex.gzhubu.top

Java: x > 0 ? "yes" : "no"
来源：http://rjy.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ecl.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://nfd.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://qfk.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://pqa.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bug.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qqr.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://djm.dashuyun.cn

TS:   `Hello, ${name}!`
来源：http://vjw.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://mqv.nwbrower.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pmk.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://xhe.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://tmf.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dhf.tarul.cn

Py:   "第一行\n第二行"
来源：http://cjw.hammf.cn

PHP:  "第一行\n第二行"
来源：http://xmz.chenjidiqi.icu

JS:   "第一行\n第二行"
来源：http://ygr.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://bpt.sxryk.cn

Java: "第一行\n第二行"
来源：http://lch.cucudq.cn

Go:   "第一行\n第二行"
来源：http://wvg.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://vvc.hesvh.cn

C#:   "第一行\n第二行"
来源：http://jco.316326.xyz

[A14] 注释写法
来源：http://jua.gogol.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tto.yongpay.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pox.jiagoushi.top

JS:   // 单行；/* 多行 */
来源：http://ema.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://zpk.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gby.yuanzhike.top

Go:   // 单行；/* 多行 */
来源：http://vbm.tian-w.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ddm.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://bjk.gzhubu.top

[A15] 空值判断与默认值
来源：http://jpa.hfpthk.cn

Py:   value = data or "默认值"
来源：http://eze.shuidangran.top

PHP:  $value = $data ?? "默认值";
来源：http://bmu.sysykeji.top

JS:   const value = data ?? "默认值";
来源：http://xdf.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://hge.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ohz.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://sjx.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://huy.kuanghao11.cn

C#:   var value = data ?? "默认值";
来源：http://oyj.birdmap.top

[A16] 真假值判断规则
来源：http://xeb.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rsa.pengpengdd.cyou

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sun.nwbrower.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wqu.dianchejie.cn

TS:   if (!x) {}
来源：http://jsw.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uwf.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qnu.zhixingplan.top

Ruby: unless x            # nil 与 false 为假
来源：http://svn.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mwh.c1oappe.top

[A17] 位运算
来源：http://zth.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvi.shuidangran.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zam.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://leq.gogol.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hoz.sxryk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssi.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://awi.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://piy.zdbjq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqz.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://ree.shzxlz.cn

Py:   ord("A"); chr(65)
来源：http://bjb.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://qhy.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fsg.hysaishi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfq.snrcjt.cn

Java: (int) 'A'; (char) 65
来源：http://hfz.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pnu.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://mmg.zhijiandao.cn

C#:   (int)'A'; (char)65
来源：http://wwk.wangdashe.top

[A19] 交换两个变量
来源：http://cgr.birdmap.top

Py:   a, b = b, a
来源：http://blz.vqdsnc.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vwu.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://gvi.hcnkem.com

TS:   [a, b] = [b, a];
来源：http://mhc.jiagoushi.top

Java: int t = a; a = b; b = t;
来源：http://awx.tian-w.cn

Go:   a, b = b, a
来源：http://jpd.gotoacloud.top

Ruby: a, b = b, a
来源：http://yxk.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://ofg.nanxinkj.top

[A20] 读取标准输入
来源：http://cjc.ehwqpu.com

Py:   name = input("请输入：")
来源：http://ppl.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tyy.yj202588.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wzd.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://jns.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://pbs.jqgfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zig.wangdashe.top

Ruby: gets.chomp
来源：http://tik.xziqi.cn

C#:   Console.ReadLine();
来源：http://sxz.yj20258.top

[A21] 保留指定小数位输出
来源：http://inm.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://fzb.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aaa.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://vwo.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://nbc.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://uwf.cqqwz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dnp.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://ric.c1oappe.top

C#:   3.14159.ToString("F2")
来源：http://ngj.yuanzhike.top

[A22] 获取字符串长度
来源：http://fre.yvedp.cn

Py:   len(s)
来源：http://gey.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mbc.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wpm.aibaodan.cn

TS:   s.length
来源：http://dxd.ywan-chungtsiang.top

Java: s.length()
来源：http://hwa.wangdashe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bch.chenjidiqi.icu

Ruby: s.length
来源：http://zjn.daria6918.cn

C#:   s.Length
来源：http://cnq.ppjwa.cn

[A23] 大小写转换
来源：http://syl.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vco.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yzx.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sya.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ufw.shuidangran.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://amk.jinqigufen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://igy.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zdf.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qkb.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://vdv.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nga.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gyv.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kqo.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://psu.gogol.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mjt.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://cnu.hywenlv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ksa.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ssi.sysykeji.top

[A25] 字符串比较
来源：http://hlw.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ham.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pve.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hno.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qpl.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://amb.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ipy.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dia.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eok.xinyue.icu

[A26] 类型转换总览
来源：http://ksw.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nma.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fga.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pye.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://hnl.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mkw.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vvs.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oyo.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jqr.ybcxt.top

================================================================================
来源：http://gur.sxryk.cn

B. 流程控制
来源：http://oky.yongpay.top

================================================================================
来源：http://gfj.gogol.net.cn

[B01] 条件判断 if / else
来源：http://jvy.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://oek.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lyi.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tmq.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sjh.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://wex.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oiv.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dcj.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nvu.yongpay.top

[B02] 多分支 else if / elif
来源：http://yuq.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hct.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://icf.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efm.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hrs.yj202588.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wnv.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pbk.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pfn.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ebs.dianchejie.cn

[B03] switch / match / case
来源：http://qwb.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ecn.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dhx.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zco.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lza.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://esp.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bya.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://erv.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ppc.hywenlv.cn

[B04] for 计数循环
来源：http://rre.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://owy.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://phm.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eoj.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eim.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mql.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mgb.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://cow.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tto.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://nim.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://oww.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://anp.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kaq.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://fle.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mdl.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cci.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://mwd.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vpz.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://qlp.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ezy.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mlc.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jmf.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cqw.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nal.zdqjudy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://omo.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xml.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lqd.guannengcc.top

[B07] while 循环
来源：http://vkp.andypj.xyz

Py:   while i < 10: i += 1
来源：http://cyh.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://khx.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://ryi.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://qhx.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://fmn.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ieh.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://nfi.tian-w.cn

C#:   while (i < 10) { i++; }
来源：http://mtn.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://gpz.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://rnl.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wbi.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://qvb.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://knj.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://gqy.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zzs.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://gam.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://agk.tanke756.top

[B09] break 与 continue
来源：http://mgx.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ebk.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://waf.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iwb.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgk.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zie.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ivd.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ulw.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gkm.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://tqy.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jgl.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jgn.shanyushiyangtech.top


<!-- 参考信息 -->