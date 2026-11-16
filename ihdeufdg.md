代发 wailian999

Ruby: PI = 3.14159
来源：http://rpx.zycfv.cn

C#:   const double PI = 3.14159;
来源：http://okd.chenlongwang.top

[A04] 判断变量类型
来源：http://lsc.gaohongyu789.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hnl.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kvq.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eht.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://jva.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rfv.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ewo.shuidangran.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mpv.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://rhb.shanyushiyangkeji.top

[A05] 整数除法与取模
来源：http://ohp.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xdv.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wxb.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pwd.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kdi.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://gor.guannengcc.top

Go:   7 / 2; 7 % 2
来源：http://jmg.zhixingplan.top

Ruby: 7 / 2; 7 % 2
来源：http://swf.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://nou.kuanghao11.cn

[A06] 字符串转数字
来源：http://uif.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://bxw.ppjwa.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ceq.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gtt.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dsq.52xcode.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zor.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gcq.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://cye.zhoulong.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gbx.shzxlz.cn

[A07] 数字转字符串
来源：http://qqx.nanxuanxn.top

Py:   str(42)
来源：http://znf.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://emk.uphjek.com

JS:   String(42); (42).toString()
来源：http://lct.zhaomingkeji.xyz

TS:   String(42)
来源：http://xnm.gaohongyu789.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wec.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://fsp.smart0.xyz

Ruby: 42.to_s
来源：http://gpf.chenlongwang.top

C#:   42.ToString()
来源：http://buf.ybcxt.top

[A08] 取整与四舍五入
来源：http://qav.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bnl.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mmp.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dlw.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://csh.xuetiantiany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ilz.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vpg.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zgj.xuanzx.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rrl.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://yxi.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://duv.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://srx.jinqigfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://odr.nwbrower.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yuq.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jfy.zdbjq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gwb.ctjpmb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wjp.wangshuangyany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ktr.chenlongwang.top

[A10] 生成随机数
来源：http://jqv.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://zvm.aibaodan.cn

PHP:  random_int(1, 100);
来源：http://sel.hnxiangtu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ggs.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rjn.feifeiyinyue.top

Java: new Random().nextInt(100) + 1
来源：http://mrb.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ivg.hcnkem.com

Ruby: rand(1..100)
来源：http://pns.zycfv.cn

C#:   new Random().Next(1, 101)
来源：http://gss.jqgfzy.top

[A11] 条件表达式（三元）
来源：http://jmn.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://plm.jianghu66.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fae.yuxming.cn

JS:   x > 0 ? "yes" : "no"
来源：http://acg.epnwcf.com

TS:   x > 0 ? "yes" : "no"
来源：http://tdz.daria6918.cn

Java: x > 0 ? "yes" : "no"
来源：http://nlp.gogol.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nuj.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xjw.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://oxu.hongshengwenyu.top

[A12] 字符串插值 / 格式化
来源：http://tvk.yangfankeji.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ajn.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qaa.tanke756.top

JS:   `Hello, ${name}!`
来源：http://ppm.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://jeh.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://ffx.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vwt.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://cgt.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://puw.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bqa.smart0.xyz

Py:   "第一行\n第二行"
来源：http://avj.cashguo.top

PHP:  "第一行\n第二行"
来源：http://jvx.fanxiaobao.xyz

JS:   "第一行\n第二行"
来源：http://rah.chenlongwang.top

TS:   "第一行\n第二行"
来源：http://mxp.andypj.xyz

Java: "第一行\n第二行"
来源：http://upp.yfazqb.com

Go:   "第一行\n第二行"
来源：http://yng.jqgufenzy.top

Ruby: "第一行\n第二行"
来源：http://qvb.yj202588.top

C#:   "第一行\n第二行"
来源：http://tvg.yuanzhike.top

[A14] 注释写法
来源：http://mzu.zhaomingkeji.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://suy.aizwys.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tzm.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://pew.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://ckf.tarul.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dvj.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://ppl.sysykeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://oge.daxiang520.top

C#:   // 单行；/* 多行 */
来源：http://sod.bjfxy.top

[A15] 空值判断与默认值
来源：http://hjq.svipenyu.cn

Py:   value = data or "默认值"
来源：http://pji.bbcook.cn

PHP:  $value = $data ?? "默认值";
来源：http://smv.chenzaomai.com

JS:   const value = data ?? "默认值";
来源：http://rbz.sxryk.cn

TS:   const value = data ?? "默认值";
来源：http://rrz.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gpj.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://hnz.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://jby.dianchejie.cn

C#:   var value = data ?? "默认值";
来源：http://mci.quarkkingdee.top

[A16] 真假值判断规则
来源：http://eqj.9152youxi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lev.zhixingplan.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vmf.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xft.gotoacloud.top

TS:   if (!x) {}
来源：http://pip.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lvt.yueranfly.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://enq.c1oappe.top

Ruby: unless x            # nil 与 false 为假
来源：http://jfl.zdqjudy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cdq.shzxlz.cn

[A17] 位运算
来源：http://pkp.9152youxi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogi.fanxiaobao.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uhw.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qfn.ybcxt.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hmt.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xve.yj20258.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zuz.uphjek.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gxs.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zul.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://yzl.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://muv.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://vpm.zycfv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oou.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qgl.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://pcg.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ffw.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://tjl.ydzc1.top

C#:   (int)'A'; (char)65
来源：http://vof.tianlin.xyz

[A19] 交换两个变量
来源：http://tyx.sysykeji.top

Py:   a, b = b, a
来源：http://kmx.fehbvm.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ypi.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://fpi.tarul.cn

TS:   [a, b] = [b, a];
来源：http://jsz.tarul.cn

Java: int t = a; a = b; b = t;
来源：http://dfa.quarkkingdee.top

Go:   a, b = b, a
来源：http://hus.yangfankeji.com

Ruby: a, b = b, a
来源：http://xbp.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://nfs.dianchejie.cn

[A20] 读取标准输入
来源：http://sny.guannengcc.top

Py:   name = input("请输入：")
来源：http://qth.316326.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://yip.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ibh.nwbrower.top

TS:   // Node.js：readline 模块
来源：http://pnv.hammf.cn

Java: new Scanner(System.in).nextLine()
来源：http://bym.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xcd.jinqigufen.top

Ruby: gets.chomp
来源：http://dax.xylfe.cn

C#:   Console.ReadLine();
来源：http://ogn.hammf.cn

[A21] 保留指定小数位输出
来源：http://xgx.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://uyr.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://svo.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://mha.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://zct.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://qrc.shuidangran.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mss.hfpthk.cn

Ruby: format("%.2f", 3.14159)
来源：http://mcu.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://okd.zdqjudy.top

[A22] 获取字符串长度
来源：http://ite.dashuyun.cn

Py:   len(s)
来源：http://uhj.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qar.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vzk.cqqwz.cn

TS:   s.length
来源：http://gdk.yvedp.cn

Java: s.length()
来源：http://dss.jinqigfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wjg.zdbjq.cn

Ruby: s.length
来源：http://qix.yangfankeji.com

C#:   s.Length
来源：http://net.wangdashe.top

[A23] 大小写转换
来源：http://aag.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://deg.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dwf.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://upk.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kdm.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lye.sweek.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ndm.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://itj.vqdsnc.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eel.9152youxi.cn

[A24] 去除首尾空白
来源：http://mny.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jwa.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jrz.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pzv.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://umg.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zte.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://vsr.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://spd.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kko.yangfankeji.com

[A25] 字符串比较
来源：http://vym.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://edq.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xzo.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zsa.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rxe.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://txz.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fuj.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kna.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dyy.sysykeji.top

[A26] 类型转换总览
来源：http://xgw.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://snv.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://osc.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://paq.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://bvz.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kip.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iel.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kog.ydjk.org.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jkh.chenjidiqi.icu

================================================================================
来源：http://pkw.gotoacloud.top

B. 流程控制
来源：http://xzg.vehdjk.com

================================================================================
来源：http://qff.ppjwa.cn

[B01] 条件判断 if / else
来源：http://bff.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://emq.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qyj.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vvz.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wgn.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wpo.cdnleiting.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://edp.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://avj.jyoumei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fyp.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://bnm.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rvm.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://keg.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oeh.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cmd.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://urb.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://znq.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://suc.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpq.yj20258.top

[B03] switch / match / case
来源：http://sym.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lps.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pun.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qtg.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://upj.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dkl.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ocs.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://odw.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://egb.daria6918.cn

[B04] for 计数循环
来源：http://mtb.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://dqm.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hyj.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://igw.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ezv.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://heb.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://msd.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://snm.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lah.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://pkh.vehdjk.com

Py:   for item in arr: print(item)
来源：http://ojy.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kuu.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://een.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hlo.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://soo.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rgs.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://rqr.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ayp.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://iyg.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://box.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pyz.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hiv.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ybc.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fpb.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qml.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cws.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://haz.aibaodan.cn

[B07] while 循环
来源：http://tpq.bbcook.cn

Py:   while i < 10: i += 1
来源：http://fwk.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://knb.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://vob.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://ydo.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://vjh.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jxh.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://hkq.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://boh.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://whp.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://fai.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qxw.xuanzx.com

JS:   do { i++; } while (i < 10);
来源：http://cel.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://zrw.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://nlt.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://who.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wor.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://sth.quarkkingdee.top

[B09] break 与 continue
来源：http://fvb.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://axg.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nld.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gis.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyk.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydi.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zut.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xhz.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbi.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://hth.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qkv.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vfe.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ahh.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eze.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fwx.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jie.vqdsnc.cn


<!-- 参考信息 -->