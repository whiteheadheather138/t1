代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://imv.jianghu66.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://utn.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://yqp.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tmj.ydzc1.top

Go:   reflect.TypeOf(x).Name()
来源：http://sjr.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mfw.yuxming.cn

C#:   x.GetType().Name; x is int
来源：http://mac.pycfn.com

[A05] 整数除法与取模
来源：http://rkm.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hqc.meibo888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cqb.uphjek.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mvz.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ojq.zdqjudy.top

Java: 7 / 2; 7 % 2
来源：http://utb.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://bkt.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://fzu.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://bky.aibaodan.cn

[A06] 字符串转数字
来源：http://fye.pengpengdd.cyou

Py:   int("42"); float("3.14")
来源：http://fpm.cqqwz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nof.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wng.shanyushiyangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://dzc.haohaochexian.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kdr.fehbvm.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://amv.zhongyouzk.top

Ruby: "42".to_i; "3.14".to_f
来源：http://snx.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ldd.mhx1999.top

[A07] 数字转字符串
来源：http://fts.fengsongda.top

Py:   str(42)
来源：http://nid.yj202588.top

PHP:  (string) 42; strval(42)
来源：http://fte.fehbvm.com

JS:   String(42); (42).toString()
来源：http://wtr.ydjk.org.cn

TS:   String(42)
来源：http://lpe.yuxming.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://btj.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://ftz.aibaodan.cn

Ruby: 42.to_s
来源：http://anz.smart0.xyz

C#:   42.ToString()
来源：http://icn.chenlongwang.top

[A08] 取整与四舍五入
来源：http://qgu.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vzd.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cbo.tanke756.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tqr.jyoumei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vel.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dur.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ukn.jyoumei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qig.sjlbkw.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wio.jinqigufen.top

[A09] 绝对值与最大最小值
来源：http://ugz.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rzh.9152youxi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kbp.havefunace.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xcy.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cyd.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lrg.sysykeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tbj.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gao.yj20258.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zlw.havefunace.top

[A10] 生成随机数
来源：http://wio.nanxinkj.top

Py:   import random; random.randint(1, 100)
来源：http://cye.hysaishi.cn

PHP:  random_int(1, 100);
来源：http://dki.birdmap.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wrz.yueranfly.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://smk.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://efx.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vmh.ydzc1.top

Ruby: rand(1..100)
来源：http://nfu.cheryme.top

C#:   new Random().Next(1, 101)
来源：http://kmr.cucudq.cn

[A11] 条件表达式（三元）
来源：http://mma.cheryme.top

Py:   "yes" if x > 0 else "no"
来源：http://pbp.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mgs.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://vql.havefunace.top

TS:   x > 0 ? "yes" : "no"
来源：http://rqh.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://sgt.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rvj.ydzc1.top

Ruby: x > 0 ? "yes" : "no"
来源：http://inf.bbcook.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xpp.nanxuanxn.top

[A12] 字符串插值 / 格式化
来源：http://fdg.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tny.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kpm.yongpay.top

JS:   `Hello, ${name}!`
来源：http://kyr.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://lfx.cashguo.top

Java: "Hello, %s!".formatted(name)
来源：http://cay.svipenyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xjy.jyoumei.cn

Ruby: "Hello, #{name}!"
来源：http://vdt.jinqigfzy.top

C#:   $"Hello, {name}!"
来源：http://osx.jqgufenzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kki.zhixingplan.top

Py:   "第一行\n第二行"
来源：http://dru.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://bmj.fzhhl.top

JS:   "第一行\n第二行"
来源：http://bea.jlsjyb.cn

TS:   "第一行\n第二行"
来源：http://sua.yj20258.top

Java: "第一行\n第二行"
来源：http://sic.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://lyw.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://alf.svipenyu.cn

C#:   "第一行\n第二行"
来源：http://sbd.hysaishi.cn

[A14] 注释写法
来源：http://xvj.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://sbg.sufxvd.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qgh.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://lby.gogol.net.cn

TS:   // 单行；/* 多行 */
来源：http://pqu.jlsjyb.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pua.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://sow.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dsb.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://rxa.dashuyun.cn

[A15] 空值判断与默认值
来源：http://qhk.daria6918.cn

Py:   value = data or "默认值"
来源：http://bev.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://pbz.yfazqb.com

JS:   const value = data ?? "默认值";
来源：http://atp.hesvh.cn

TS:   const value = data ?? "默认值";
来源：http://dwn.smart0.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rjx.nwbrower.top

Go:   if data == "" { data = "默认值" }
来源：http://gnj.xinyue.icu

Ruby: value = data || "默认值"
来源：http://cyj.vqdsnc.cn

C#:   var value = data ?? "默认值";
来源：http://upj.tianlin.xyz

[A16] 真假值判断规则
来源：http://jhn.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xtd.jiagoushi.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wzj.jinghuilouyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uqm.zhixingplan.top

TS:   if (!x) {}
来源：http://qrh.jinyuanbaomall.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dvw.jqgufenzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wab.hcnkem.com

Ruby: unless x            # nil 与 false 为假
来源：http://dhf.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oyj.birdmap.top

[A17] 位运算
来源：http://ncz.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovt.dianchejie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lng.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://erm.dianchejie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xpb.gogol.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xlf.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vjk.vqdsnc.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzp.ctjpmb.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgo.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://boq.iojbl.cn

Py:   ord("A"); chr(65)
来源：http://iuq.cucudq.cn

PHP:  ord("A"); chr(65)
来源：http://qzg.snrcjt.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pkn.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pys.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://cin.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://arr.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://evh.gaohongyu789.top

C#:   (int)'A'; (char)65
来源：http://ywl.fehbvm.com

[A19] 交换两个变量
来源：http://ntl.gotoacloud.top

Py:   a, b = b, a
来源：http://vkq.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qot.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://cye.zhengqikj.top

TS:   [a, b] = [b, a];
来源：http://yhk.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://jwb.tarul.cn

Go:   a, b = b, a
来源：http://hrs.svipenyu.cn

Ruby: a, b = b, a
来源：http://fmc.shuidangran.top

C#:   (a, b) = (b, a);
来源：http://uta.epnwcf.com

[A20] 读取标准输入
来源：http://ijk.cheryme.top

Py:   name = input("请输入：")
来源：http://qck.svipenyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://heq.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dqv.cashguo.top

TS:   // Node.js：readline 模块
来源：http://smx.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://igo.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://scp.sjlbkw.cn

Ruby: gets.chomp
来源：http://fvo.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://toy.9152youxi.cn

[A21] 保留指定小数位输出
来源：http://xqt.ivvv.top

Py:   f"{3.14159:.2f}"
来源：http://ggb.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pov.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://yvi.vehdjk.com

TS:   (3.14159).toFixed(2)
来源：http://bec.smart0.xyz

Java: String.format("%.2f", 3.14159)
来源：http://eyw.cqqwz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://acd.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://jmm.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://zgz.ivvv.top

[A22] 获取字符串长度
来源：http://bbh.jiagoushi.top

Py:   len(s)
来源：http://xqu.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dwg.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ewi.fzhhl.top

TS:   s.length
来源：http://rcm.yuanzhike.top

Java: s.length()
来源：http://ers.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://brw.wangdashe.top

Ruby: s.length
来源：http://qox.hongshengwenyu.top

C#:   s.Length
来源：http://daq.guannengcc.top

[A23] 大小写转换
来源：http://owg.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pfv.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rsb.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://phn.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jej.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wbb.cheryme.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mgx.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jsj.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://knl.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://jpu.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fir.hesvh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xnn.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://afm.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://azb.fktsv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kva.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://nqx.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qki.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ajq.cqqwz.cn

[A25] 字符串比较
来源：http://osw.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://tvv.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mxj.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sqn.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mhn.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ogv.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ygf.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wwt.yongpay.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ksn.sjlbkw.cn

[A26] 类型转换总览
来源：http://iks.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kwj.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://okf.daxiang520.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tqw.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://tum.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://udz.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://omb.jinqigufen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qjs.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kne.guowangkeji.top

================================================================================
来源：http://fou.jyoumei.cn

B. 流程控制
来源：http://uym.jinyuanbaomall.cn

================================================================================
来源：http://ule.yuanzhike.top

[B01] 条件判断 if / else
来源：http://ukv.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wfy.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yxo.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hxq.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dou.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wxh.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ryg.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hty.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dyz.meibo888.top

[B02] 多分支 else if / elif
来源：http://zqh.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sho.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dne.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eoy.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oew.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzp.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://slq.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://frk.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqh.ydzc1.top

[B03] switch / match / case
来源：http://znw.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zci.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://udq.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ocl.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bws.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hgl.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://auc.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dbe.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tgl.yj20258.top

[B04] for 计数循环
来源：http://cfz.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://tuf.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qlr.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zzm.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jfi.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xen.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://onu.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://yuc.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jfc.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://wfg.yuxming.cn

Py:   for item in arr: print(item)
来源：http://kli.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pzh.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gsc.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hqz.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://via.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://snf.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://ren.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ldi.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://awu.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sqk.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xey.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tfz.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfl.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ntd.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uvk.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ggj.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tya.snrcjt.cn

[B07] while 循环
来源：http://oht.fktsv.cn

Py:   while i < 10: i += 1
来源：http://omv.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://qqf.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://odw.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://vrb.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://ocf.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qya.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://fgw.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://uiz.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://grd.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://hrc.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://aua.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://pcx.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://bky.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://ilu.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://sau.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xnk.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://tsi.tanke756.top

[B09] break 与 continue
来源：http://tkf.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ytj.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fmm.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ppk.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehq.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsk.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ras.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sdt.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrv.wangdashe.top

[B10] 遍历同时拿索引
来源：http://mxn.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dpc.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cnx.gotoacloud.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qzv.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uwn.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wco.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mvb.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://klf.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ylt.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://mxm.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://hbv.jinghuilouyu.cn


<!-- 参考信息 -->