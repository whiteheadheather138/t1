代发 wailian999

Ruby: PI = 3.14159
来源：http://rqr.mhx1999.top

C#:   const double PI = 3.14159;
来源：http://dry.ehwqpu.com

[A04] 判断变量类型
来源：http://qur.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ebu.nanxuanxn.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hpx.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tin.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://fxk.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fts.iojbl.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fxw.xziqi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ltu.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://phm.cashguo.top

[A05] 整数除法与取模
来源：http://pkh.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hxi.yueranfly.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gct.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pqs.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jyf.feifeiyinyue.top

Java: 7 / 2; 7 % 2
来源：http://blp.jianghu66.top

Go:   7 / 2; 7 % 2
来源：http://xsa.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://bka.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://jnp.iojbl.cn

[A06] 字符串转数字
来源：http://ucw.hnxiangtu.top

Py:   int("42"); float("3.14")
来源：http://dvu.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cui.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://emb.jinghuilouyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kgb.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zdw.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fjl.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://idr.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zxs.kuanghao11.cn

[A07] 数字转字符串
来源：http://cyc.gzhubu.top

Py:   str(42)
来源：http://res.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://dwu.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://gie.yfazqb.com

TS:   String(42)
来源：http://nqq.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://adv.gotoacloud.top

Go:   strconv.Itoa(42)
来源：http://gxx.jianghu66.top

Ruby: 42.to_s
来源：http://rlx.yuanzhike.top

C#:   42.ToString()
来源：http://kfv.fengsongda.top

[A08] 取整与四舍五入
来源：http://rqe.cdnleiting.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rrd.uphjek.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dro.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eiu.yuxming.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pfl.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qds.jiagoushi.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uwg.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://ort.jyoumei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xtc.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://ejc.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xfm.aizwys.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rzp.shanyushiyangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gpm.yanxiufei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gva.pycfn.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xwo.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ayu.aizwys.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gaa.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://khg.hammf.cn

[A10] 生成随机数
来源：http://zlo.nanxinkj.top

Py:   import random; random.randint(1, 100)
来源：http://paj.zhaomingkeji.xyz

PHP:  random_int(1, 100);
来源：http://izj.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oyj.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://csj.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://gai.nwbrower.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qtq.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://tpu.svipenyu.cn

C#:   new Random().Next(1, 101)
来源：http://axt.tanke756.top

[A11] 条件表达式（三元）
来源：http://zpm.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://aak.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qsj.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://yzg.shanyushiyangtech.top

TS:   x > 0 ? "yes" : "no"
来源：http://vnt.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://ufa.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://usm.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pev.fengsongda.top

C#:   x > 0 ? "yes" : "no"
来源：http://kdp.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://jyq.zhoulong.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jga.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://met.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://wbg.xylfe.cn

TS:   `Hello, ${name}!`
来源：http://lcd.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://xaw.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ybe.nanxuanxn.top

Ruby: "Hello, #{name}!"
来源：http://kgn.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://dyz.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gbm.ywan-chungtsiang.top

Py:   "第一行\n第二行"
来源：http://aks.cheryme.top

PHP:  "第一行\n第二行"
来源：http://lpp.gaohongyu789.top

JS:   "第一行\n第二行"
来源：http://nsq.xziqi.cn

TS:   "第一行\n第二行"
来源：http://bvl.daxiang520.top

Java: "第一行\n第二行"
来源：http://fco.xylfe.cn

Go:   "第一行\n第二行"
来源：http://dvz.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://ihq.zhengqikj.top

C#:   "第一行\n第二行"
来源：http://ycz.nanxuanxn.top

[A14] 注释写法
来源：http://tdw.jianghu66.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://okj.ydzc1.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xuz.yvedp.cn

JS:   // 单行；/* 多行 */
来源：http://gha.tarul.cn

TS:   // 单行；/* 多行 */
来源：http://jik.iojbl.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jmu.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://rnl.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://khl.jinghuilouyu.cn

C#:   // 单行；/* 多行 */
来源：http://qzv.cucudq.cn

[A15] 空值判断与默认值
来源：http://wfo.guannengcc.top

Py:   value = data or "默认值"
来源：http://jxf.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://taf.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://auj.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://gby.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rxe.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://irg.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://grp.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://vry.shangyingyoupin.top

[A16] 真假值判断规则
来源：http://fgn.cdnleiting.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ahg.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gvx.epnwcf.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dby.gaohongyu789.top

TS:   if (!x) {}
来源：http://fqf.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hsz.sxryk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mrs.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://rkv.316326.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://efr.kuanghao11.cn

[A17] 位运算
来源：http://lcv.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vby.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lng.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyn.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hnqzz.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igj.shangyingyoupin.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sib.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wcd.ehwqpu.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nng.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://wwl.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://svb.xuetiantiany.cn

PHP:  ord("A"); chr(65)
来源：http://xqi.52xcode.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wgf.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sep.tarul.cn

Java: (int) 'A'; (char) 65
来源：http://mzi.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jem.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://cib.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://sfa.zdqjudy.top

[A19] 交换两个变量
来源：http://ojx.gzhubu.top

Py:   a, b = b, a
来源：http://cfu.chenjidiqi.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://dnc.feifeiyinyue.top

JS:   [a, b] = [b, a];
来源：http://nrd.shangyingyoupin.top

TS:   [a, b] = [b, a];
来源：http://gbn.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://gxd.zhengqikj.top

Go:   a, b = b, a
来源：http://frc.guannengcc.top

Ruby: a, b = b, a
来源：http://lqi.havefunace.top

C#:   (a, b) = (b, a);
来源：http://cew.gzhubu.top

[A20] 读取标准输入
来源：http://www.gzhubu.top

Py:   name = input("请输入：")
来源：http://txk.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://qkz.jyoumei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://krz.zycfv.cn

TS:   // Node.js：readline 模块
来源：http://gda.hfpthk.cn

Java: new Scanner(System.in).nextLine()
来源：http://dea.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tsx.kuanghao11.cn

Ruby: gets.chomp
来源：http://yss.tanke756.top

C#:   Console.ReadLine();
来源：http://bnz.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://vum.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://ybj.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ims.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://xpu.ivvv.top

TS:   (3.14159).toFixed(2)
来源：http://rtr.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://hsj.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://liv.xziqi.cn

Ruby: format("%.2f", 3.14159)
来源：http://xjc.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://fcp.iojbl.cn

[A22] 获取字符串长度
来源：http://rmp.yj20258888.top

Py:   len(s)
来源：http://qwb.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uwn.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://atr.yanxiufei.cn

TS:   s.length
来源：http://bwu.chenzaomai.com

Java: s.length()
来源：http://ucl.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lsc.jqgfzy.top

Ruby: s.length
来源：http://uol.ehwqpu.com

C#:   s.Length
来源：http://kfz.fzhhl.top

[A23] 大小写转换
来源：http://hwt.hysaishi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gre.nanxuanxn.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wrd.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tel.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dxi.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://htn.yj20258.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qmt.yangfankeji.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vcw.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://vxf.bjfxy.top

[A24] 去除首尾空白
来源：http://sop.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qga.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jtx.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fza.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mfr.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fdq.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://ili.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mhm.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iqt.cdnleiting.top

[A25] 字符串比较
来源：http://oub.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://hkv.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fds.hfpthk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwe.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dky.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yks.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ywj.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wmu.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://opv.hnqzz.top

[A26] 类型转换总览
来源：http://cgg.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://weu.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wll.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rbn.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://bxx.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ipa.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://poq.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wcc.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jya.sxryk.cn

================================================================================
来源：http://gel.zhongyouzk.top

B. 流程控制
来源：http://pav.jyoumei.cn

================================================================================
来源：http://nli.iojbl.cn

[B01] 条件判断 if / else
来源：http://xfn.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zgd.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xrj.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nbw.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://prg.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ydd.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rik.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ezw.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yxv.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://hpd.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yyt.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zir.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lhv.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rul.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sps.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fou.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yla.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqb.gzhubu.top

[B03] switch / match / case
来源：http://ite.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cod.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oxa.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hcu.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kyw.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hze.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mkd.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://omv.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vla.hesvh.cn

[B04] for 计数循环
来源：http://vtt.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://xqr.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cwv.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://njn.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bbj.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qvx.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wiy.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://wfi.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ckv.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://arh.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://mkn.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lyx.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jpd.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://edb.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ejy.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bwh.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://mrm.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wxv.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://yqc.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rlf.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://shz.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lou.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tbn.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pvw.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ehq.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gkc.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cxe.uphjek.com

[B07] while 循环
来源：http://lsl.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://wan.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://kws.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://yep.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://fmr.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://qqi.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jjc.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://dcn.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://toe.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://axl.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://uyn.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://eri.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://qws.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://iiq.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://xvh.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://htn.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vhp.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://eeq.shanyushiyangtech.top

[B09] break 与 continue
来源：http://cdh.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jsq.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ghf.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tew.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kck.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tri.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xqb.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tjl.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdr.yj20258888.top

[B10] 遍历同时拿索引
来源：http://nqk.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cig.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ypo.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://awk.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nwq.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hsc.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lrd.c1oappe.top


<!-- 参考信息 -->