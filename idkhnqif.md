代发 wailian999

Ruby: PI = 3.14159
来源：http://ovw.yj20258.top

C#:   const double PI = 3.14159;
来源：http://sdc.vqdsnc.cn

[A04] 判断变量类型
来源：http://sfz.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vdq.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uyq.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://her.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://gkx.yvedp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mmp.yvedp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hbu.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://kua.zhijiandao.cn

C#:   x.GetType().Name; x is int
来源：http://taq.jqgfzy.top

[A05] 整数除法与取模
来源：http://mtq.yangfankeji.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wyq.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://cuj.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fnb.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vff.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://eqx.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://rqb.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://jvm.hongshengwenyu.top

C#:   7 / 2; 7 % 2
来源：http://whf.sweek.top

[A06] 字符串转数字
来源：http://axl.hysaishi.cn

Py:   int("42"); float("3.14")
来源：http://etz.jinghuilouyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dab.mhx1999.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mxn.yuxming.cn

TS:   parseInt("42", 10); Number("42")
来源：http://doq.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sch.quarkkingdee.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oqv.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ksw.wangdashe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://soo.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://dqv.52xcode.cn

Py:   str(42)
来源：http://mwi.wangshuangyany.cn

PHP:  (string) 42; strval(42)
来源：http://gqe.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://xsj.shanyushiyangtech.top

TS:   String(42)
来源：http://nqr.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ukl.hcnkem.com

Go:   strconv.Itoa(42)
来源：http://anv.yanxiufei.cn

Ruby: 42.to_s
来源：http://nwy.hcnkem.com

C#:   42.ToString()
来源：http://scf.xziqi.cn

[A08] 取整与四舍五入
来源：http://jhl.tanke756.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aop.gotoacloud.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hao.zdbjq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zew.cashguo.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hwx.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://aii.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xzk.bbcook.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kjh.gotoacloud.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://edy.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://kag.fehbvm.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aah.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://upk.yangfankeji.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://apy.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dsb.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xvu.jqgufenzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tcr.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bnz.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iph.hcnkem.com

[A10] 生成随机数
来源：http://oil.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://ibd.yuanzhike.top

PHP:  random_int(1, 100);
来源：http://pkg.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ctl.shzxlz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ttj.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://umm.daria6918.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pdn.cheryme.top

Ruby: rand(1..100)
来源：http://efq.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://kha.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://ave.9152youxi.cn

Py:   "yes" if x > 0 else "no"
来源：http://jzy.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://vvl.smart0.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://zgp.yvedp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iju.zhaomingkeji.xyz

Java: x > 0 ? "yes" : "no"
来源：http://nen.pycfn.com

Go:   // 无三元运算符，需用 if 语句
来源：http://aos.cashguo.top

Ruby: x > 0 ? "yes" : "no"
来源：http://faa.yangfankeji.com

C#:   x > 0 ? "yes" : "no"
来源：http://yco.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://bgd.hnqzz.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kzy.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kgt.xingfuxueyuan.xyz

JS:   `Hello, ${name}!`
来源：http://uim.jinghuilouyu.cn

TS:   `Hello, ${name}!`
来源：http://tie.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://rdl.smart0.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cne.smart0.xyz

Ruby: "Hello, #{name}!"
来源：http://cbf.tian-w.cn

C#:   $"Hello, {name}!"
来源：http://yzw.fzhhl.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jge.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://cmq.fzhhl.top

PHP:  "第一行\n第二行"
来源：http://bgl.aizwys.cn

JS:   "第一行\n第二行"
来源：http://vee.wangdashe.top

TS:   "第一行\n第二行"
来源：http://hez.xuetiantiany.cn

Java: "第一行\n第二行"
来源：http://ods.zdqjudy.top

Go:   "第一行\n第二行"
来源：http://ily.guowangkeji.top

Ruby: "第一行\n第二行"
来源：http://sdl.jinqigufen.top

C#:   "第一行\n第二行"
来源：http://dzx.yueranfly.top

[A14] 注释写法
来源：http://zwu.guowangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://bjv.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ppt.hywenlv.cn

JS:   // 单行；/* 多行 */
来源：http://xdk.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://wys.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://utf.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://ihp.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cav.cucudq.cn

C#:   // 单行；/* 多行 */
来源：http://rlp.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://yrw.dashuyun.cn

Py:   value = data or "默认值"
来源：http://fqe.iojbl.cn

PHP:  $value = $data ?? "默认值";
来源：http://bcr.hfpthk.cn

JS:   const value = data ?? "默认值";
来源：http://nei.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://mvz.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://prx.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://ftc.birdmap.top

Ruby: value = data || "默认值"
来源：http://iji.dianchejie.cn

C#:   var value = data ?? "默认值";
来源：http://nan.jinqigufen.top

[A16] 真假值判断规则
来源：http://qxx.ivvv.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oeu.cheryme.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ygh.c1oappe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pyv.wangdashe.top

TS:   if (!x) {}
来源：http://xim.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fnx.hesvh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lhg.shuidangran.top

Ruby: unless x            # nil 与 false 为假
来源：http://uzw.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gxg.zhijiandao.cn

[A17] 位运算
来源：http://apo.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nro.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://npo.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rfw.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wom.yongpay.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drd.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gbz.fktsv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixd.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmj.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://dqj.gaohongyu789.top

Py:   ord("A"); chr(65)
来源：http://pce.cucudq.cn

PHP:  ord("A"); chr(65)
来源：http://kyy.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wpu.yongpay.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fve.nwbrower.top

Java: (int) 'A'; (char) 65
来源：http://gxt.uphjek.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zcu.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://jtr.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://kcm.yanxiufei.cn

[A19] 交换两个变量
来源：http://bwr.hcnkem.com

Py:   a, b = b, a
来源：http://men.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://gue.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://uyn.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://mxp.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://kxj.zycfv.cn

Go:   a, b = b, a
来源：http://etr.mhx1999.top

Ruby: a, b = b, a
来源：http://koc.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://gkh.guowangkeji.top

[A20] 读取标准输入
来源：http://tty.gzhubu.top

Py:   name = input("请输入：")
来源：http://rcj.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ujo.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vpo.daxiang520.top

TS:   // Node.js：readline 模块
来源：http://zio.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://cwe.ydjk.org.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sot.quarkkingdee.top

Ruby: gets.chomp
来源：http://adt.hongshengwenyu.top

C#:   Console.ReadLine();
来源：http://vpq.redwolf501.top

[A21] 保留指定小数位输出
来源：http://uzs.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://ccg.fengsongda.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eus.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://zox.havefunace.top

TS:   (3.14159).toFixed(2)
来源：http://ino.xuetiantiany.cn

Java: String.format("%.2f", 3.14159)
来源：http://bey.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rgn.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://fvb.jyoumei.cn

C#:   3.14159.ToString("F2")
来源：http://nld.ivvv.top

[A22] 获取字符串长度
来源：http://hmb.havefunace.top

Py:   len(s)
来源：http://yqp.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wrd.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mav.svipenyu.cn

TS:   s.length
来源：http://nso.yfazqb.com

Java: s.length()
来源：http://zoi.zhengqikj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ksm.9152youxi.cn

Ruby: s.length
来源：http://swp.zycfv.cn

C#:   s.Length
来源：http://jbc.cashguo.top

[A23] 大小写转换
来源：http://drd.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qbb.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pmk.zdbjq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wzb.uphjek.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://epz.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zho.yangfankeji.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gli.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yhg.yj20258888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hgq.hcnkem.com

[A24] 去除首尾空白
来源：http://ell.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://erx.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bdo.nwbrower.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://syq.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tzz.sweek.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lqs.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://jhh.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xan.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://siv.tanke756.top

[A25] 字符串比较
来源：http://esb.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://xcu.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qpq.feifeiyinyue.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ezh.bbcook.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qhc.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uyv.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qxl.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xmq.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://liw.shanyushiyangkeji.top

[A26] 类型转换总览
来源：http://pha.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qjh.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fqq.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jbq.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://lvm.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xey.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hhv.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://eie.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rmq.52xcode.cn

================================================================================
来源：http://cjc.316326.xyz

B. 流程控制
来源：http://avb.zdbjq.cn

================================================================================
来源：http://axn.svipenyu.cn

[B01] 条件判断 if / else
来源：http://gtm.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://koi.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://grl.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cci.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nvj.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://khx.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fbz.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qwt.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://agm.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://izc.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ele.zdqjudy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lnt.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kfo.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wtw.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gld.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hbx.zhengqikj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qol.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vhg.zhongyouzk.top

[B03] switch / match / case
来源：http://roc.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uiv.tanke756.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jik.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wgv.yj202588.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xix.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://evi.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bhx.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uxv.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ebx.hywenlv.cn

[B04] for 计数循环
来源：http://bhs.birdmap.top

Py:   for i in range(10): print(i)
来源：http://qyy.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lye.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qfd.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ueo.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://peq.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://syh.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://gdy.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bgo.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://tjk.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://uql.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xyz.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pem.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ang.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yin.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pck.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://nqj.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://onm.yj202588.top

[B06] 遍历字典 / 对象
来源：http://bit.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://tbi.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kbh.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://otw.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ydr.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wcp.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dnp.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nfw.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xmi.zdqjudy.top

[B07] while 循环
来源：http://ipl.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://vct.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ldz.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://cbe.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://vdi.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://zzh.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://orm.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://xuh.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://sca.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://vpq.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://pgt.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pcc.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://qgt.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://sna.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://vzh.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fwj.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://grd.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://jua.tian-w.cn

[B09] break 与 continue
来源：http://dtc.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fqd.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://geu.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://san.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cic.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rng.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bbm.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wgo.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pmp.andypj.xyz

[B10] 遍历同时拿索引
来源：http://frp.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mah.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://irh.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wdz.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aug.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uvj.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://don.jianghu66.top


<!-- 参考信息 -->