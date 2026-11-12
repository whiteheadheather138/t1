代发 wailian999

Ruby: PI = 3.14159
来源：http://oyd.vehdjk.com

C#:   const double PI = 3.14159;
来源：http://kse.chenlongwang.top

[A04] 判断变量类型
来源：http://nqi.nanxuanxn.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://moa.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kzc.yuanzhike.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ksz.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://fyh.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cwy.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xex.jyoumei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kzl.zdbjq.cn

C#:   x.GetType().Name; x is int
来源：http://zsd.sufxvd.cn

[A05] 整数除法与取模
来源：http://bga.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vdl.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lom.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wgz.vehdjk.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uot.0kj1m.cn

Java: 7 / 2; 7 % 2
来源：http://izc.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://jbb.shuidangran.top

Ruby: 7 / 2; 7 % 2
来源：http://qzo.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://lct.snrcjt.cn

[A06] 字符串转数字
来源：http://kum.gogol.net.cn

Py:   int("42"); float("3.14")
来源：http://xxn.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vzo.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lww.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://vqe.sxryk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yom.yanxiufei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yyl.jinyuanbaomall.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ofu.snrcjt.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://krl.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://eni.sufxvd.cn

Py:   str(42)
来源：http://saq.hongshengwenyu.top

PHP:  (string) 42; strval(42)
来源：http://nld.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://fwf.tian-w.cn

TS:   String(42)
来源：http://rjs.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vum.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://zhi.316326.xyz

Ruby: 42.to_s
来源：http://egl.daxiang520.top

C#:   42.ToString()
来源：http://rdq.kuanghao11.cn

[A08] 取整与四舍五入
来源：http://afr.jqgufenzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gjj.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oup.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dxu.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uga.sxryk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mth.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cip.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://rdq.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aij.zhiwuduotai.top

[A09] 绝对值与最大最小值
来源：http://tta.bjfxy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mol.pycfn.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sey.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ihe.jinqigufen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fgq.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nmp.fanxiaobao.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://exy.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cuf.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qsw.zdqjudy.top

[A10] 生成随机数
来源：http://bga.feifeiyinyue.top

Py:   import random; random.randint(1, 100)
来源：http://ktz.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://cjf.yj20258888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sej.dianchejie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ntr.zhongyouzk.top

Java: new Random().nextInt(100) + 1
来源：http://ppl.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ekn.jinqigufen.top

Ruby: rand(1..100)
来源：http://qxw.yvedp.cn

C#:   new Random().Next(1, 101)
来源：http://hbz.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://ort.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://xds.vqdsnc.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wza.ctjpmb.com

JS:   x > 0 ? "yes" : "no"
来源：http://chn.hcnkem.com

TS:   x > 0 ? "yes" : "no"
来源：http://fzn.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://bqp.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://vah.yangfankeji.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ryb.yanxiufei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xol.zhongyouzk.top

[A12] 字符串插值 / 格式化
来源：http://yke.sysykeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sne.yj20258888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iap.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://bhy.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://pol.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://mpd.chenlongwang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://idx.gaohongyu789.top

Ruby: "Hello, #{name}!"
来源：http://evz.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://vuj.jlsjyb.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zuc.jinyuanbaomall.cn

Py:   "第一行\n第二行"
来源：http://znf.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://pnu.hfpthk.cn

JS:   "第一行\n第二行"
来源：http://rtt.havefunace.top

TS:   "第一行\n第二行"
来源：http://krp.fzhhl.top

Java: "第一行\n第二行"
来源：http://wam.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://ytq.zycfv.cn

Ruby: "第一行\n第二行"
来源：http://kyu.ydzc1.top

C#:   "第一行\n第二行"
来源：http://tfk.52xcode.cn

[A14] 注释写法
来源：http://vbw.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lti.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gvz.yonumen.top

JS:   // 单行；/* 多行 */
来源：http://sie.hysaishi.cn

TS:   // 单行；/* 多行 */
来源：http://doh.jqgufenzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dpd.chenlongwang.top

Go:   // 单行；/* 多行 */
来源：http://dmj.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cwl.gogol.net.cn

C#:   // 单行；/* 多行 */
来源：http://qys.tian-w.cn

[A15] 空值判断与默认值
来源：http://kar.wangdashe.top

Py:   value = data or "默认值"
来源：http://uox.chenlongwang.top

PHP:  $value = $data ?? "默认值";
来源：http://qfb.yanxiufei.cn

JS:   const value = data ?? "默认值";
来源：http://poj.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://enp.epnwcf.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rvp.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://gpk.jianghu66.top

Ruby: value = data || "默认值"
来源：http://qtc.chenjidiqi.icu

C#:   var value = data ?? "默认值";
来源：http://rih.redwolf501.top

[A16] 真假值判断规则
来源：http://ljw.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rmv.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://trn.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sjj.daxiang520.top

TS:   if (!x) {}
来源：http://dim.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ljj.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qvw.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fvo.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://edy.cqqwz.cn

[A17] 位运算
来源：http://wty.kuanghao11.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://koq.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rsj.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ynn.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xde.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://act.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dcj.chenjidiqi.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lui.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dsi.sweek.top

[A18] 字符与 ASCII 码互转
来源：http://tbd.smart0.xyz

Py:   ord("A"); chr(65)
来源：http://syn.cashguo.top

PHP:  ord("A"); chr(65)
来源：http://fvc.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ryx.yfazqb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cpm.sysykeji.top

Java: (int) 'A'; (char) 65
来源：http://hiq.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ysa.ydzc1.top

Ruby: "A".ord; 65.chr
来源：http://dub.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://joo.snrcjt.cn

[A19] 交换两个变量
来源：http://nxt.yfazqb.com

Py:   a, b = b, a
来源：http://dlh.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xzw.yvedp.cn

JS:   [a, b] = [b, a];
来源：http://kiw.jiagoushi.top

TS:   [a, b] = [b, a];
来源：http://cvm.ydjk.org.cn

Java: int t = a; a = b; b = t;
来源：http://ivl.bjfxy.top

Go:   a, b = b, a
来源：http://aiq.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://ehx.zdbjq.cn

C#:   (a, b) = (b, a);
来源：http://laz.zhongyouzk.top

[A20] 读取标准输入
来源：http://jtu.dashuyun.cn

Py:   name = input("请输入：")
来源：http://xjh.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://lyv.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gto.c1oappe.top

TS:   // Node.js：readline 模块
来源：http://nyw.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://sdl.xingfuxueyuan.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://asl.sxryk.cn

Ruby: gets.chomp
来源：http://qxs.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://kzh.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://csx.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://xmj.jinqigufen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jlf.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://xnd.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://let.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://fnk.xylfe.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ghl.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://rze.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://aid.ydzc1.top

[A22] 获取字符串长度
来源：http://pmk.gotoacloud.top

Py:   len(s)
来源：http://lud.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oyg.hnqzz.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zha.jinqigufen.top

TS:   s.length
来源：http://qag.316326.xyz

Java: s.length()
来源：http://umn.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wid.cdnleiting.top

Ruby: s.length
来源：http://kma.jiagoushi.top

C#:   s.Length
来源：http://jmb.hfpthk.cn

[A23] 大小写转换
来源：http://jqi.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fpr.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ufy.tian-w.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yyd.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qty.zhoulong.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cca.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hmw.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bie.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ikj.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://wdi.bbcook.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mcl.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cow.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ioy.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eau.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ddu.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://svl.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pva.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zae.9152youxi.cn

[A25] 字符串比较
来源：http://cko.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://inx.zhixingplan.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lye.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://coo.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://akt.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://crg.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hrf.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zqq.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ita.jinqigufen.top

[A26] 类型转换总览
来源：http://gan.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nms.ehwqpu.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://izm.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ung.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://kjw.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zdr.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://efe.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://krf.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lyh.smart0.xyz

================================================================================
来源：http://uyr.pengpengdd.cyou

B. 流程控制
来源：http://myy.zhongyouzk.top

================================================================================
来源：http://ejt.fzhhl.top

[B01] 条件判断 if / else
来源：http://qqq.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pna.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://trd.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://obr.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qai.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pju.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gcl.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pzr.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://woa.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://zgm.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gku.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tsc.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hcl.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tpd.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gzb.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ihm.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lzh.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpr.yj20258.top

[B03] switch / match / case
来源：http://com.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zft.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aot.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iru.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mht.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dzz.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vga.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ewm.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bqm.cheryme.top

[B04] for 计数循环
来源：http://eph.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://dbq.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tto.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ukk.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gkv.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pwv.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dhk.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://dnf.mhx1999.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://znz.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://ppi.yonumen.top

Py:   for item in arr: print(item)
来源：http://gom.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fcs.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dsf.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gjw.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wpx.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gvi.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://cwb.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jrq.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://jux.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://kjv.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uwc.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qei.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tdf.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bbe.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xza.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://faq.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yad.epnwcf.com

[B07] while 循环
来源：http://hhq.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://jns.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://yae.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://xqh.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://tpo.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://jii.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wbd.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://jwt.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://rze.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://dts.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://uau.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eba.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://igq.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://xxj.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://gpu.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://upc.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://jme.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://yif.zycfv.cn

[B09] break 与 continue
来源：http://czg.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jku.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tlg.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mea.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cvb.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vuh.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mso.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rqa.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxm.cucudq.cn

[B10] 遍历同时拿索引
来源：http://jcd.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dhv.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ejx.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fsd.xuanzx.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sjj.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hbq.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hfn.0kj1m.cn


<!-- 参考信息 -->