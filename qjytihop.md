代发 wailian999

JS:   const PI = 3.14159;
来源：http://tau.zhaomingkeji.xyz

TS:   const PI: number = 3.14159;
来源：http://nfj.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://kwo.shuidangran.top

Go:   const PI = 3.14159
来源：http://pnk.jianghu66.top

Ruby: PI = 3.14159
来源：http://xja.jinqigufen.top

C#:   const double PI = 3.14159;
来源：http://jxy.hongshengwenyu.top

[A04] 判断变量类型
来源：http://skb.tarul.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lsd.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rwe.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hgv.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://gja.hnxiangtu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://znv.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://tdq.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hrl.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://rcz.zhijiandao.cn

[A05] 整数除法与取模
来源：http://btx.quarkkingdee.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bvq.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ikz.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cwh.xuetiantiany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nlu.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://vqh.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://fhu.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://ljb.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://bcu.havefunace.top

[A06] 字符串转数字
来源：http://yjh.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://pxi.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oye.9152youxi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ejt.dashuyun.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bsu.ctjpmb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qft.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hez.jiagoushi.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ljc.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aua.zhiwuduotai.top

[A07] 数字转字符串
来源：http://shu.ybcxt.top

Py:   str(42)
来源：http://inx.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://mbt.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://wdq.fehbvm.com

TS:   String(42)
来源：http://tmd.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xgn.yuxming.cn

Go:   strconv.Itoa(42)
来源：http://phk.chenzaomai.com

Ruby: 42.to_s
来源：http://lpd.zdqjudy.top

C#:   42.ToString()
来源：http://ixa.fengsongda.top

[A08] 取整与四舍五入
来源：http://ype.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ndp.yj20258888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lkz.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://utx.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://veu.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://czv.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xwe.hongshengwenyu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cdp.shuidangran.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://poy.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://xwo.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ajl.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vcr.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vrg.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oip.gotoacloud.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aly.cheryme.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://usg.xuanzx.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lii.tanke756.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ofw.yangfankeji.com

[A10] 生成随机数
来源：http://int.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://oxv.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://gww.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ogf.ydjk.org.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ytq.ehwqpu.com

Java: new Random().nextInt(100) + 1
来源：http://bfx.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hgw.zdbjq.cn

Ruby: rand(1..100)
来源：http://emu.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://ezu.smart0.xyz

[A11] 条件表达式（三元）
来源：http://vix.yuxming.cn

Py:   "yes" if x > 0 else "no"
来源：http://usy.shanyushiyangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lfj.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://koy.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://onv.ybcxt.top

Java: x > 0 ? "yes" : "no"
来源：http://nkt.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nyw.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mjv.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xnf.tianlin.xyz

[A12] 字符串插值 / 格式化
来源：http://wax.zhengqikj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zee.hysaishi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oah.fktsv.cn

JS:   `Hello, ${name}!`
来源：http://owa.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://gad.aibaodan.cn

Java: "Hello, %s!".formatted(name)
来源：http://ham.aizwys.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jcc.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://awa.xingfuxueyuan.xyz

C#:   $"Hello, {name}!"
来源：http://pqw.zdbjq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tmo.yangfankeji.com

Py:   "第一行\n第二行"
来源：http://fwc.fehbvm.com

PHP:  "第一行\n第二行"
来源：http://kkl.ybcxt.top

JS:   "第一行\n第二行"
来源：http://kvc.meibo888.top

TS:   "第一行\n第二行"
来源：http://xzd.fehbvm.com

Java: "第一行\n第二行"
来源：http://oej.yanxiufei.cn

Go:   "第一行\n第二行"
来源：http://arf.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://mze.xingfuxueyuan.xyz

C#:   "第一行\n第二行"
来源：http://hhv.wangshuangyany.cn

[A14] 注释写法
来源：http://qwr.epnwcf.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://rjz.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vhx.hammf.cn

JS:   // 单行；/* 多行 */
来源：http://eew.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://ejz.haohaochexian.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zmv.yfazqb.com

Go:   // 单行；/* 多行 */
来源：http://hsz.jqgufenzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://uac.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://udn.jyoumei.cn

[A15] 空值判断与默认值
来源：http://vfv.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://dmk.chenzaomai.com

PHP:  $value = $data ?? "默认值";
来源：http://avl.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://laq.c1oappe.top

TS:   const value = data ?? "默认值";
来源：http://fwl.gotoacloud.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wnp.cqqwz.cn

Go:   if data == "" { data = "默认值" }
来源：http://kvc.bbcook.cn

Ruby: value = data || "默认值"
来源：http://fpk.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://ezq.dashuyun.cn

[A16] 真假值判断规则
来源：http://fzk.sweek.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rta.jyoumei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zug.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zff.jinqigfzy.top

TS:   if (!x) {}
来源：http://wnc.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uwb.jinqigfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kvl.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://pol.ehwqpu.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ban.nanxinkj.top

[A17] 位运算
来源：http://ukf.vqdsnc.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nus.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qox.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mvw.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vvt.nanxinkj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mmr.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dvj.jlsjyb.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igu.nwbrower.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olv.zdqjudy.top

[A18] 字符与 ASCII 码互转
来源：http://kgr.yfazqb.com

Py:   ord("A"); chr(65)
来源：http://frg.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://stl.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hhb.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pcy.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://ytu.quarkkingdee.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qaq.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://cku.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://ewq.tianlin.xyz

[A19] 交换两个变量
来源：http://dfm.316326.xyz

Py:   a, b = b, a
来源：http://kcc.yanxiufei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oox.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://xtz.jqgfzy.top

TS:   [a, b] = [b, a];
来源：http://uxh.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://etx.shangyingyoupin.top

Go:   a, b = b, a
来源：http://ggk.meibo888.top

Ruby: a, b = b, a
来源：http://jqk.xziqi.cn

C#:   (a, b) = (b, a);
来源：http://roe.gotoacloud.top

[A20] 读取标准输入
来源：http://app.yuxming.cn

Py:   name = input("请输入：")
来源：http://lqv.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://jev.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vjh.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://dwr.gaohongyu789.top

Java: new Scanner(System.in).nextLine()
来源：http://kul.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ago.hnxiangtu.top

Ruby: gets.chomp
来源：http://jro.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://rgj.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://lop.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://ews.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://avk.shanyushiyangtech.top

JS:   (3.14159).toFixed(2)
来源：http://qdj.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://utc.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://szr.yuxming.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://edt.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://uek.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://qjy.havefunace.top

[A22] 获取字符串长度
来源：http://wlt.chenlongwang.top

Py:   len(s)
来源：http://veh.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rcd.zhengqikj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xoo.snrcjt.cn

TS:   s.length
来源：http://mka.0kj1m.cn

Java: s.length()
来源：http://bvy.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jok.shangyingyoupin.top

Ruby: s.length
来源：http://deu.hongshengwenyu.top

C#:   s.Length
来源：http://keh.ivvv.top

[A23] 大小写转换
来源：http://moe.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rae.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ecm.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vry.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vsz.yj20258888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mku.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rzm.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rad.52xcode.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uzn.yvedp.cn

[A24] 去除首尾空白
来源：http://lbl.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://khv.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nxz.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qzj.shanyushiyangtech.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kqz.jqgfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oop.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://xqq.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://clq.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tzl.chenzaomai.com

[A25] 字符串比较
来源：http://rdn.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://std.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tzl.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fvh.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jbm.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zbg.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nnk.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xoy.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mea.yanxiufei.cn

[A26] 类型转换总览
来源：http://hmw.epnwcf.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wub.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aut.chenjidiqi.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oah.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://btk.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dlj.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://brj.chenjidiqi.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://rrn.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nwt.yvedp.cn

================================================================================
来源：http://ute.hnqzz.top

B. 流程控制
来源：http://drf.52xcode.cn

================================================================================
来源：http://ofk.yuanzhike.top

[B01] 条件判断 if / else
来源：http://tii.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://dbb.uphjek.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bsq.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zqk.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mlv.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://kqd.c1oappe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://een.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://irv.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tum.iojbl.cn

[B02] 多分支 else if / elif
来源：http://azh.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://scw.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://elw.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://coq.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apv.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krt.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bhv.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ogo.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://woz.vqdsnc.cn

[B03] switch / match / case
来源：http://cmj.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ixt.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://edf.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dmo.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uwp.xziqi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bah.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hgz.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gnd.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://csn.bjfxy.top

[B04] for 计数循环
来源：http://yuf.havefunace.top

Py:   for i in range(10): print(i)
来源：http://lqj.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jmz.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mwb.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bnu.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sxv.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jwr.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://lja.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tzz.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://yzv.ydzc1.top

Py:   for item in arr: print(item)
来源：http://iej.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xih.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://hjt.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yot.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yet.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fke.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://xac.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pev.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://mmp.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rxe.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jgg.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gqb.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wht.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hhx.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bic.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iui.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fwk.guowangkeji.top

[B07] while 循环
来源：http://jqh.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://qgw.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://fyg.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://hej.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://fzi.hammf.cn

Java: while (i < 10) { i++; }
来源：http://kvk.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kir.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://cvr.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://ilb.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://fri.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://dug.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bvu.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://ntm.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://yft.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://xvi.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ysq.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pdq.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://voc.jqgufenzy.top

[B09] break 与 continue
来源：http://rnf.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nnx.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gbg.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkm.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qav.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://una.chenzaomai.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bkr.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kfl.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sez.52xcode.cn

[B10] 遍历同时拿索引
来源：http://lkl.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ccj.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mbj.jqgufenzy.top


<!-- 参考信息 -->