代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://dwi.mhx1999.top

[A03] 常量定义
来源：http://qbf.jiagoushi.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bmz.hnqzz.top

PHP:  const PI = 3.14159;
来源：http://irl.cheryme.top

JS:   const PI = 3.14159;
来源：http://uka.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://xpe.redwolf501.top

Java: static final double PI = 3.14159;
来源：http://cyq.bjfxy.top

Go:   const PI = 3.14159
来源：http://ubp.tarul.cn

Ruby: PI = 3.14159
来源：http://tvj.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://mjn.9152youxi.cn

[A04] 判断变量类型
来源：http://myx.yueranfly.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://etk.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qfy.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lkg.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://vgd.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qqa.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://tks.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ita.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://uzd.ctjpmb.com

[A05] 整数除法与取模
来源：http://dup.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qqt.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dxn.jinqigufen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jgd.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ieu.yj20258.top

Java: 7 / 2; 7 % 2
来源：http://rei.xinyue.icu

Go:   7 / 2; 7 % 2
来源：http://gbs.sysykeji.top

Ruby: 7 / 2; 7 % 2
来源：http://vla.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://mpa.bbcook.cn

[A06] 字符串转数字
来源：http://etj.feifeiyinyue.top

Py:   int("42"); float("3.14")
来源：http://uly.jinyuanbaomall.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ycd.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ptr.zhengqikj.top

TS:   parseInt("42", 10); Number("42")
来源：http://nki.zhoulong.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wbo.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fpj.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ctb.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kgp.gaohongyu789.top

[A07] 数字转字符串
来源：http://tyz.nwbrower.top

Py:   str(42)
来源：http://ubc.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://lxt.cucudq.cn

JS:   String(42); (42).toString()
来源：http://ylg.tian-w.cn

TS:   String(42)
来源：http://vfl.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vtx.hysaishi.cn

Go:   strconv.Itoa(42)
来源：http://bim.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://wxs.shuidangran.top

C#:   42.ToString()
来源：http://qch.nwbrower.top

[A08] 取整与四舍五入
来源：http://oqw.sxryk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nzq.wangdashe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zhb.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bbo.0kj1m.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zsm.xinyue.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lkb.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nuf.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://vkr.zhaomingkeji.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qmq.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://gll.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gvg.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://plr.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cgk.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rca.yuanzhike.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oys.yvedp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nvc.316326.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tlg.vehdjk.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jgm.daria6918.cn

[A10] 生成随机数
来源：http://cfw.gotoacloud.top

Py:   import random; random.randint(1, 100)
来源：http://xdz.hfpthk.cn

PHP:  random_int(1, 100);
来源：http://trf.svipenyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dmh.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://opl.yuxming.cn

Java: new Random().nextInt(100) + 1
来源：http://hao.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zww.fehbvm.com

Ruby: rand(1..100)
来源：http://bzx.chenlongwang.top

C#:   new Random().Next(1, 101)
来源：http://ggc.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://juw.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://aqa.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vdm.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://htn.jqgfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://jgg.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://afj.aizwys.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wqf.ppjwa.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tbv.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://lpz.sufxvd.cn

[A12] 字符串插值 / 格式化
来源：http://ieb.tianlin.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ryu.yanxiufei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://agg.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://tko.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://gae.smart0.xyz

Java: "Hello, %s!".formatted(name)
来源：http://qkq.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hgq.aibaodan.cn

Ruby: "Hello, #{name}!"
来源：http://tev.dianchejie.cn

C#:   $"Hello, {name}!"
来源：http://lbn.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uwb.svipenyu.cn

Py:   "第一行\n第二行"
来源：http://cow.jlsjyb.cn

PHP:  "第一行\n第二行"
来源：http://nto.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://nlt.zhiwuduotai.top

TS:   "第一行\n第二行"
来源：http://rot.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://pyv.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://nex.hammf.cn

Ruby: "第一行\n第二行"
来源：http://aqy.gogol.net.cn

C#:   "第一行\n第二行"
来源：http://jju.cdnleiting.top

[A14] 注释写法
来源：http://jkm.aibaodan.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ukw.nanxinkj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ilj.316326.xyz

JS:   // 单行；/* 多行 */
来源：http://etj.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://nvf.svipenyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eyw.ydzc1.top

Go:   // 单行；/* 多行 */
来源：http://jak.hcnkem.com

Ruby: # 单行；=begin 多行 =end
来源：http://cly.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://qpr.feifeiyinyue.top

[A15] 空值判断与默认值
来源：http://cqp.zhixingplan.top

Py:   value = data or "默认值"
来源：http://xea.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://vco.fengsongda.top

JS:   const value = data ?? "默认值";
来源：http://rcu.316326.xyz

TS:   const value = data ?? "默认值";
来源：http://mer.bjfxy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dpw.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://hnd.havefunace.top

Ruby: value = data || "默认值"
来源：http://wqb.chenlongwang.top

C#:   var value = data ?? "默认值";
来源：http://ycx.ppjwa.cn

[A16] 真假值判断规则
来源：http://jff.nanxinkj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ecb.guowangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dja.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yjb.ppjwa.cn

TS:   if (!x) {}
来源：http://zrf.sufxvd.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vki.yueranfly.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uyl.feifeiyinyue.top

Ruby: unless x            # nil 与 false 为假
来源：http://bqf.zycfv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wsd.andypj.xyz

[A17] 位运算
来源：http://fjd.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fsv.quarkkingdee.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cth.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ghq.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pxt.daxiang520.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vtt.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rfn.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hxb.ppjwa.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xvl.sysykeji.top

[A18] 字符与 ASCII 码互转
来源：http://len.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://fzg.yj20258888.top

PHP:  ord("A"); chr(65)
来源：http://ldj.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://csw.aizwys.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://guo.sysykeji.top

Java: (int) 'A'; (char) 65
来源：http://abr.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qjb.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://cda.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://dzj.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://ost.yj20258888.top

Py:   a, b = b, a
来源：http://fli.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oig.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://tjf.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://ayt.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://jzs.epnwcf.com

Go:   a, b = b, a
来源：http://ore.sysykeji.top

Ruby: a, b = b, a
来源：http://fwc.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://tth.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://mnl.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://xtx.jinqigufen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wsw.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yks.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://bek.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://uvg.wangdashe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://knh.sysykeji.top

Ruby: gets.chomp
来源：http://eor.dashuyun.cn

C#:   Console.ReadLine();
来源：http://tqy.jianghu66.top

[A21] 保留指定小数位输出
来源：http://ebe.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://wvv.shanyushiyangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gne.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://low.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://ker.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://kvs.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wob.guannengcc.top

Ruby: format("%.2f", 3.14159)
来源：http://ohi.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://gvq.iojbl.cn

[A22] 获取字符串长度
来源：http://vpk.sxryk.cn

Py:   len(s)
来源：http://qbc.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uma.guowangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://put.ivvv.top

TS:   s.length
来源：http://hoz.c1oappe.top

Java: s.length()
来源：http://mkr.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pkb.pengpengdd.cyou

Ruby: s.length
来源：http://cjn.quarkkingdee.top

C#:   s.Length
来源：http://nlo.bbcook.cn

[A23] 大小写转换
来源：http://jhh.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://twa.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ejp.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vkn.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fgp.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://upc.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://klr.fktsv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://suf.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://qmf.52xcode.cn

[A24] 去除首尾空白
来源：http://xaj.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fcb.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rpf.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ctu.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nfu.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nan.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://zlp.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tbe.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qvl.sxryk.cn

[A25] 字符串比较
来源：http://eye.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://jmr.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zme.zhiwuduotai.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zva.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ogg.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ylv.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pdh.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://haq.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ick.yonumen.top

[A26] 类型转换总览
来源：http://gjw.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jwt.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ocv.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eus.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://ijc.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xod.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://itp.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kbf.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oqp.yj20258888.top

================================================================================
来源：http://evl.jianghu66.top

B. 流程控制
来源：http://fhz.jqgfzy.top

================================================================================
来源：http://trr.9152youxi.cn

[B01] 条件判断 if / else
来源：http://usx.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://syr.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ylt.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://btd.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pjq.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mqh.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mqu.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ouv.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ofz.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://wch.iojbl.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oyc.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://acp.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://euw.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ypd.bjfxy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhh.xziqi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fum.meibo888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fvo.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxq.ydjk.org.cn

[B03] switch / match / case
来源：http://jqg.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ouz.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://loe.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzw.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pts.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sso.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ojz.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qgt.chenjidiqi.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sgi.epnwcf.com

[B04] for 计数循环
来源：http://wmt.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://zfr.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://myj.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hkh.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vys.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xme.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zxh.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://oyv.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pxr.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://bta.cheryme.top

Py:   for item in arr: print(item)
来源：http://wgq.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rzb.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aqb.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ggv.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zuk.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ynl.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://icw.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fxw.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://mup.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ljj.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xcs.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bjp.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ijt.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pee.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bnv.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nql.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oaz.dianchejie.cn

[B07] while 循环
来源：http://pkt.mhx1999.top

Py:   while i < 10: i += 1
来源：http://znt.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zsf.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://fyt.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://ljp.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://ets.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xig.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://zha.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://tmd.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://lkj.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://ybl.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ijd.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://rrq.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://vlb.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://irz.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://bjb.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xhn.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://lpn.pycfn.com

[B09] break 与 continue
来源：http://afo.hnxiangtu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nag.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lki.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xvc.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://euj.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rps.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jyx.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gqb.wangshuangyany.cn


<!-- 参考信息 -->