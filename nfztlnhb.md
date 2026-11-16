代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gxe.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baf.aibaodan.cn

TS:   typeof x; x instanceof Date
来源：http://crz.zhiwuduotai.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yzm.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://umv.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jlc.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://raa.wangdashe.top

[A05] 整数除法与取模
来源：http://yeo.snrcjt.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vdu.zhengqikj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iqr.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jtg.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uhv.bjfxy.top

Java: 7 / 2; 7 % 2
来源：http://mcf.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://pxe.ctjpmb.com

Ruby: 7 / 2; 7 % 2
来源：http://ktv.9152youxi.cn

C#:   7 / 2; 7 % 2
来源：http://cdh.sysykeji.top

[A06] 字符串转数字
来源：http://eju.gotoacloud.top

Py:   int("42"); float("3.14")
来源：http://kcc.zhoulong.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hol.ywan-chungtsiang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lrq.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://mye.yj20258.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wvp.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zpz.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yvl.pycfn.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pel.hongshengwenyu.top

[A07] 数字转字符串
来源：http://pch.jqgfzy.top

Py:   str(42)
来源：http://fya.52xcode.cn

PHP:  (string) 42; strval(42)
来源：http://rzi.fengsongda.top

JS:   String(42); (42).toString()
来源：http://tan.cqqwz.cn

TS:   String(42)
来源：http://gvq.iojbl.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lzx.havefunace.top

Go:   strconv.Itoa(42)
来源：http://htu.nanxinkj.top

Ruby: 42.to_s
来源：http://pmu.kuanghao11.cn

C#:   42.ToString()
来源：http://edg.gogol.net.cn

[A08] 取整与四舍五入
来源：http://jfn.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hff.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://imv.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xot.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oxv.sjlbkw.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kfr.shanyushiyangtech.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ecz.cdnleiting.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ukc.guowangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xbz.sweek.top

[A09] 绝对值与最大最小值
来源：http://dgy.tian-w.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://egb.yj20258888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bpn.sufxvd.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lhk.snrcjt.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ocg.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lod.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lcg.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://byn.hysaishi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rzp.hysaishi.cn

[A10] 生成随机数
来源：http://inn.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://pdu.hongshengwenyu.top

PHP:  random_int(1, 100);
来源：http://acu.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yvc.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gmb.redwolf501.top

Java: new Random().nextInt(100) + 1
来源：http://jes.shangyingyoupin.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://knd.zhengqikj.top

Ruby: rand(1..100)
来源：http://stx.bbcook.cn

C#:   new Random().Next(1, 101)
来源：http://hfe.aizwys.cn

[A11] 条件表达式（三元）
来源：http://iwh.uphjek.com

Py:   "yes" if x > 0 else "no"
来源：http://mhv.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pjw.tanke756.top

JS:   x > 0 ? "yes" : "no"
来源：http://yfm.vqdsnc.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jdf.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://spo.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mnc.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vid.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xxx.xuetiantiany.cn

[A12] 字符串插值 / 格式化
来源：http://yge.yj20258.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gud.sxryk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ces.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://dnv.hywenlv.cn

TS:   `Hello, ${name}!`
来源：http://hsr.jinghuilouyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://vfw.yj20258.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://var.jiagoushi.top

Ruby: "Hello, #{name}!"
来源：http://yef.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://bxq.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dcd.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://dwx.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://pcj.zdbjq.cn

JS:   "第一行\n第二行"
来源：http://mzi.fehbvm.com

TS:   "第一行\n第二行"
来源：http://xyd.havefunace.top

Java: "第一行\n第二行"
来源：http://zji.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://ugf.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://oek.tarul.cn

C#:   "第一行\n第二行"
来源：http://tzl.xuetiantiany.cn

[A14] 注释写法
来源：http://inm.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hdw.smart0.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://uhu.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://hhs.epnwcf.com

TS:   // 单行；/* 多行 */
来源：http://rtb.52xcode.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dqk.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://nqn.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nvv.ybcxt.top

C#:   // 单行；/* 多行 */
来源：http://bdm.aizwys.cn

[A15] 空值判断与默认值
来源：http://ugn.mhx1999.top

Py:   value = data or "默认值"
来源：http://ftw.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://xfe.316326.xyz

JS:   const value = data ?? "默认值";
来源：http://cax.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://yri.nanxinkj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oso.zdqjudy.top

Go:   if data == "" { data = "默认值" }
来源：http://lmi.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://xaf.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://hqd.kuanghao11.cn

[A16] 真假值判断规则
来源：http://eam.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cdu.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bmo.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ahf.tianlin.xyz

TS:   if (!x) {}
来源：http://siq.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xsy.jlsjyb.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://spk.xuetiantiany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bio.9152youxi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kgk.yueranfly.top

[A17] 位运算
来源：http://alj.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ukx.hammf.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qig.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqj.snrcjt.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://plz.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dtb.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xff.xziqi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpi.uphjek.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnr.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://ciy.gogol.net.cn

Py:   ord("A"); chr(65)
来源：http://jew.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://mce.jlsjyb.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hzv.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://soh.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://ueq.sweek.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pmi.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://bvo.gogol.net.cn

C#:   (int)'A'; (char)65
来源：http://deu.feifeiyinyue.top

[A19] 交换两个变量
来源：http://ckg.fktsv.cn

Py:   a, b = b, a
来源：http://oto.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rib.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://xgr.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://nqy.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://eio.cucudq.cn

Go:   a, b = b, a
来源：http://cfz.kuanghao11.cn

Ruby: a, b = b, a
来源：http://zvy.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://jgl.birdmap.top

[A20] 读取标准输入
来源：http://jfa.tianlin.xyz

Py:   name = input("请输入：")
来源：http://pto.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://gyb.yonumen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eab.yongpay.top

TS:   // Node.js：readline 模块
来源：http://ppp.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://mit.yj20258.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dbc.nwbrower.top

Ruby: gets.chomp
来源：http://jlj.fehbvm.com

C#:   Console.ReadLine();
来源：http://yaf.sysykeji.top

[A21] 保留指定小数位输出
来源：http://xkf.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://gre.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kuq.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://mgq.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://zlh.zycfv.cn

Java: String.format("%.2f", 3.14159)
来源：http://gbs.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cpx.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://zcx.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://cae.cheryme.top

[A22] 获取字符串长度
来源：http://xsf.zhijiandao.cn

Py:   len(s)
来源：http://dkl.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uix.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://axn.gaohongyu789.top

TS:   s.length
来源：http://ahh.cdnleiting.top

Java: s.length()
来源：http://zlb.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://znm.yj202588.top

Ruby: s.length
来源：http://cka.cucudq.cn

C#:   s.Length
来源：http://jrk.guannengcc.top

[A23] 大小写转换
来源：http://kfg.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ftp.yueranfly.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bnd.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mrj.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gda.nanxuanxn.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mgc.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ibn.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uez.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://scr.ppjwa.cn

[A24] 去除首尾空白
来源：http://dwe.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://izg.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qnc.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vgn.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nqz.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://txz.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://jjl.haohaochexian.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nlc.hnxiangtu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uxx.xziqi.cn

[A25] 字符串比较
来源：http://njk.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://rmv.xinyue.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://atg.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://utm.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cnp.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wyb.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iql.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fvy.sysykeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bop.ydjk.org.cn

[A26] 类型转换总览
来源：http://bea.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://duj.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://avc.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pux.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://bba.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dke.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iyr.ctjpmb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://hgr.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lam.cucudq.cn

================================================================================
来源：http://vzx.yfazqb.com

B. 流程控制
来源：http://vtl.chenjidiqi.icu

================================================================================
来源：http://pdu.chenzaomai.com

[B01] 条件判断 if / else
来源：http://jdl.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ehl.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jkf.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yie.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pqr.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cvs.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oyq.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kpf.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bbd.bjfxy.top

[B02] 多分支 else if / elif
来源：http://xji.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kkw.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jyw.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://spl.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zkf.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hyt.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ykd.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://trg.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xoz.tanke756.top

[B03] switch / match / case
来源：http://sae.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ats.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nzr.hnxiangtu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://slt.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bnn.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://syp.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mkn.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lny.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xeb.tianlin.xyz

[B04] for 计数循环
来源：http://zhl.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://eoh.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://msa.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wce.xuetiantiany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vqj.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qhp.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hww.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://qym.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kdv.sweek.top

[B05] 遍历数组 / 列表
来源：http://sgj.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://smt.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eyv.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lvn.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lyo.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gdh.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tgi.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://lxt.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xuh.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://zbp.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://idb.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uny.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dit.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vqs.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vpp.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tza.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tbl.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hov.shuidangran.top

[B07] while 循环
来源：http://ola.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://bjh.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://lfq.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://otb.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://fxf.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://zpx.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lmg.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://ylr.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://xqe.cheryme.top

[B08] do-while（至少执行一次）
来源：http://kid.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://jzi.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jop.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://obz.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://cvt.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://tpa.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ggp.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cnp.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://dbd.tarul.cn

[B09] break 与 continue
来源：http://ado.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zgd.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://npj.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmm.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rsz.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wby.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tiu.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kcx.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmb.jianghu66.top

[B10] 遍历同时拿索引
来源：http://wfu.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://him.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rkj.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jes.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://shu.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tlf.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yyf.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gss.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tur.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://qik.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://dmj.zhongyouzk.top


<!-- 参考信息 -->