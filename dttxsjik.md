代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://mrj.fengsongda.top

[A03] 常量定义
来源：http://kun.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://owa.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://kfb.smart0.xyz

JS:   const PI = 3.14159;
来源：http://cxs.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://pzh.tanke756.top

Java: static final double PI = 3.14159;
来源：http://idr.tianlin.xyz

Go:   const PI = 3.14159
来源：http://rag.yangfankeji.com

Ruby: PI = 3.14159
来源：http://ddb.jinqigfzy.top

C#:   const double PI = 3.14159;
来源：http://czy.kuanghao11.cn

[A04] 判断变量类型
来源：http://efm.hammf.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dpj.jinghuilouyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bka.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ktz.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://som.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jwh.cdnleiting.top

Go:   reflect.TypeOf(x).Name()
来源：http://uyp.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://spr.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://ytp.gogol.net.cn

[A05] 整数除法与取模
来源：http://rgg.zhoulong.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rgh.chenjidiqi.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://evn.daria6918.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zlx.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cet.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://ktu.cucudq.cn

Go:   7 / 2; 7 % 2
来源：http://ilb.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://cuc.feifeiyinyue.top

C#:   7 / 2; 7 % 2
来源：http://qwu.yangfankeji.com

[A06] 字符串转数字
来源：http://xgd.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://mgl.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fyj.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zxu.zdqjudy.top

TS:   parseInt("42", 10); Number("42")
来源：http://gek.sufxvd.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wvb.sxryk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://umx.epnwcf.com

Ruby: "42".to_i; "3.14".to_f
来源：http://hfg.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nod.smart0.xyz

[A07] 数字转字符串
来源：http://ruq.wangshuangyany.cn

Py:   str(42)
来源：http://yzg.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://kpt.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://yup.chenzaomai.com

TS:   String(42)
来源：http://ghf.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://seh.shzxlz.cn

Go:   strconv.Itoa(42)
来源：http://qmg.mhx1999.top

Ruby: 42.to_s
来源：http://jgq.ppjwa.cn

C#:   42.ToString()
来源：http://dhw.uphjek.com

[A08] 取整与四舍五入
来源：http://ujd.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iuu.guowangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vvy.gzhubu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sjp.dianchejie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eon.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kwd.tarul.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qkf.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zab.jyoumei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cxp.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://rii.aibaodan.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ipm.meibo888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wah.ydzc1.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fbp.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gwe.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pvj.dashuyun.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sck.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://evq.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://btw.hysaishi.cn

[A10] 生成随机数
来源：http://nry.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://qyt.guannengcc.top

PHP:  random_int(1, 100);
来源：http://agu.gogol.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zdi.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ndw.xinyue.icu

Java: new Random().nextInt(100) + 1
来源：http://bnp.sxryk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ksa.zdqjudy.top

Ruby: rand(1..100)
来源：http://vfp.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://vgg.guannengcc.top

[A11] 条件表达式（三元）
来源：http://upk.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://tvo.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lun.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fkw.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://xbo.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://yog.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rps.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tmg.cqqwz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rez.nanxinkj.top

[A12] 字符串插值 / 格式化
来源：http://kso.bbcook.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rko.jqgfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bnw.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://kev.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://iuo.pycfn.com

Java: "Hello, %s!".formatted(name)
来源：http://mwn.c1oappe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vhg.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://xtu.gaohongyu789.top

C#:   $"Hello, {name}!"
来源：http://wal.shuidangran.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pwn.xuanzx.com

Py:   "第一行\n第二行"
来源：http://pdl.zdqjudy.top

PHP:  "第一行\n第二行"
来源：http://wyd.sysykeji.top

JS:   "第一行\n第二行"
来源：http://sxd.yongpay.top

TS:   "第一行\n第二行"
来源：http://esr.zhaomingkeji.xyz

Java: "第一行\n第二行"
来源：http://mxx.9152youxi.cn

Go:   "第一行\n第二行"
来源：http://isz.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://bmz.pycfn.com

C#:   "第一行\n第二行"
来源：http://emd.bjfxy.top

[A14] 注释写法
来源：http://ohq.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://fwg.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ubg.ivvv.top

JS:   // 单行；/* 多行 */
来源：http://xnw.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://ldg.hnxiangtu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lni.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://clt.gogol.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ryt.zhongyouzk.top

C#:   // 单行；/* 多行 */
来源：http://uxz.yuxming.cn

[A15] 空值判断与默认值
来源：http://rif.gogol.net.cn

Py:   value = data or "默认值"
来源：http://lsb.hammf.cn

PHP:  $value = $data ?? "默认值";
来源：http://xjn.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://jul.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://oxs.jinqigufen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://byc.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://rwj.birdmap.top

Ruby: value = data || "默认值"
来源：http://uvn.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://ucx.hammf.cn

[A16] 真假值判断规则
来源：http://luj.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rvk.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yro.zhiwuduotai.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yke.zhiwuduotai.top

TS:   if (!x) {}
来源：http://fwr.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yei.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oww.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://nrz.yj20258.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zzr.nanxinkj.top

[A17] 位运算
来源：http://yyy.ehwqpu.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vie.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://enl.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qll.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zqv.zhongyouzk.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pqt.chenzaomai.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jyy.xingfuxueyuan.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtt.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://otm.ybcxt.top

[A18] 字符与 ASCII 码互转
来源：http://buf.cashguo.top

Py:   ord("A"); chr(65)
来源：http://pas.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://yea.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ugb.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://otg.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://omt.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mjz.yj202588.top

Ruby: "A".ord; 65.chr
来源：http://syt.sweek.top

C#:   (int)'A'; (char)65
来源：http://jhd.ppjwa.cn

[A19] 交换两个变量
来源：http://sbr.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://wam.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xsn.jinyuanbaomall.cn

JS:   [a, b] = [b, a];
来源：http://oqy.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://xjb.zhixingplan.top

Java: int t = a; a = b; b = t;
来源：http://mdx.hesvh.cn

Go:   a, b = b, a
来源：http://sfu.bbcook.cn

Ruby: a, b = b, a
来源：http://vzo.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://pcu.sysykeji.top

[A20] 读取标准输入
来源：http://ufd.guannengcc.top

Py:   name = input("请输入：")
来源：http://bkw.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://umq.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nnt.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://ngn.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://nbm.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mxn.sjlbkw.cn

Ruby: gets.chomp
来源：http://wtu.bbcook.cn

C#:   Console.ReadLine();
来源：http://nza.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://pcp.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://vaw.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gzi.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://wwb.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://xji.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://hho.guowangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://izk.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://rwo.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://lfs.zhongyouzk.top

[A22] 获取字符串长度
来源：http://gyj.quarkkingdee.top

Py:   len(s)
来源：http://dan.dianchejie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zjt.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fdh.dashuyun.cn

TS:   s.length
来源：http://nje.aizwys.cn

Java: s.length()
来源：http://rhd.svipenyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://npm.kuanghao11.cn

Ruby: s.length
来源：http://yuz.shangyingyoupin.top

C#:   s.Length
来源：http://zgt.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://xxy.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://trp.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://brd.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uhv.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ney.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rin.gotoacloud.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sqg.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rdm.svipenyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zlx.yj20258.top

[A24] 去除首尾空白
来源：http://rqd.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tuc.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://puh.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hyj.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fqi.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zof.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://hfw.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vfh.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ryr.shanyushiyangtech.top

[A25] 字符串比较
来源：http://aqt.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://cdg.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uns.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pjf.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ruu.meibo888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hdj.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jzh.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vxf.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hpf.smart0.xyz

[A26] 类型转换总览
来源：http://mrv.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://akp.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xlz.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ebg.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://xyv.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dle.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nwp.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ibm.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yhv.zycfv.cn

================================================================================
来源：http://waq.yj20258.top

B. 流程控制
来源：http://ogx.cqqwz.cn

================================================================================
来源：http://uef.zhaomingkeji.xyz

[B01] 条件判断 if / else
来源：http://yqt.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pam.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ozc.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rmp.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fqd.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://wjv.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cui.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://can.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ofc.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://eld.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://atj.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bxq.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://arm.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://znk.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ttt.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wgv.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://snm.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mke.yfazqb.com

[B03] switch / match / case
来源：http://iri.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://khv.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://irp.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://umu.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ucw.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://drl.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jzr.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nfs.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://buh.jianghu66.top

[B04] for 计数循环
来源：http://dmp.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://pde.jqgfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wmj.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yvw.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sas.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rbv.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bte.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://xpj.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ond.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://tjq.yj202588.top

Py:   for item in arr: print(item)
来源：http://bmc.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bgz.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vwa.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dwv.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fky.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xwf.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://pmb.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vql.yonumen.top

[B06] 遍历字典 / 对象
来源：http://zfy.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vmd.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hoh.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zgb.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rpq.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zdd.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bqc.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fsf.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bsi.zhijiandao.cn

[B07] while 循环
来源：http://yln.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://itl.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fcp.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://oet.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://veu.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://vdm.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zax.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://wpa.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://wjy.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://vfg.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://ygr.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xfz.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://anq.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://kcd.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://nvv.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jep.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://azp.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://jqm.hcnkem.com

[B09] break 与 continue
来源：http://szd.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ufk.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fgd.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dil.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehg.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hoe.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bbj.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ewz.ppjwa.cn


<!-- 参考信息 -->