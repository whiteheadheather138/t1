代发 wailian999

Py:   print("Hello, World!")
来源：http://htm.snrcjt.cn

PHP:  echo "Hello, World!";
来源：http://dkc.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://rtj.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uil.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://ocf.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://ime.xuanzx.com

Ruby: puts "Hello, World!"
来源：http://eev.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://edn.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://lmk.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vjm.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bde.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tns.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uxz.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://kyw.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://ttt.jinqigufen.top

Ruby: name = "Alex"; age = 20
来源：http://irf.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://ggz.fengsongda.top

[A03] 常量定义
来源：http://orq.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dgq.yuxming.cn

PHP:  const PI = 3.14159;
来源：http://suv.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://awt.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://pqs.havefunace.top

Java: static final double PI = 3.14159;
来源：http://lax.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://cer.guowangkeji.top

Ruby: PI = 3.14159
来源：http://wzf.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://vtc.cashguo.top

[A04] 判断变量类型
来源：http://yuv.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://izl.feifeiyinyue.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qhx.jinqigfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yxy.uphjek.com

TS:   typeof x; x instanceof Date
来源：http://oyc.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mbk.hammf.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ttp.hnxiangtu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cso.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://heq.jianghu66.top

[A05] 整数除法与取模
来源：http://pop.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mcl.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oud.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://esi.hammf.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cfa.daria6918.cn

Java: 7 / 2; 7 % 2
来源：http://xzv.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://ipw.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://vwd.sxryk.cn

C#:   7 / 2; 7 % 2
来源：http://vzi.yangfankeji.com

[A06] 字符串转数字
来源：http://xgo.chenjidiqi.icu

Py:   int("42"); float("3.14")
来源：http://mlh.jinghuilouyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://weq.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jux.hongshengwenyu.top

TS:   parseInt("42", 10); Number("42")
来源：http://yqk.zhiwuduotai.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lox.xingfuxueyuan.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dfy.jqgfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ciz.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kau.xylfe.cn

[A07] 数字转字符串
来源：http://ran.meibo888.top

Py:   str(42)
来源：http://jyj.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://xuo.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://kwa.cqqwz.cn

TS:   String(42)
来源：http://hvz.haohaochexian.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ziw.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://klm.sysykeji.top

Ruby: 42.to_s
来源：http://yil.haohaochexian.top

C#:   42.ToString()
来源：http://xsq.svipenyu.cn

[A08] 取整与四舍五入
来源：http://ilq.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lml.hongshengwenyu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tao.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://onl.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pli.bjfxy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pxc.nwbrower.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nea.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://udt.hongshengwenyu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tnd.bjfxy.top

[A09] 绝对值与最大最小值
来源：http://dht.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mmi.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kti.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gjo.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gwy.sxryk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lre.yj202588.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dvt.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kob.hongshengwenyu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kcw.zhiwuduotai.top

[A10] 生成随机数
来源：http://zen.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://blw.tanke756.top

PHP:  random_int(1, 100);
来源：http://rfu.hongshengwenyu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dvk.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qjc.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://qwb.ywan-chungtsiang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yhj.ydjk.org.cn

Ruby: rand(1..100)
来源：http://ira.fehbvm.com

C#:   new Random().Next(1, 101)
来源：http://bnc.sxryk.cn

[A11] 条件表达式（三元）
来源：http://dkl.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://hnf.feifeiyinyue.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mre.zhijiandao.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zpr.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://lvh.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://hoc.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://eiz.hammf.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nez.jyoumei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eqf.jlsjyb.cn

[A12] 字符串插值 / 格式化
来源：http://yaf.ppjwa.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qsi.redwolf501.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ttd.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://tab.ctjpmb.com

TS:   `Hello, ${name}!`
来源：http://ljd.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://asl.quarkkingdee.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://epb.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://pgn.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://xux.mhx1999.top

[A13] 多行字符串（练习 \n 转义）
来源：http://srn.fzhhl.top

Py:   "第一行\n第二行"
来源：http://flt.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://dvn.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://sld.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://dep.zdqjudy.top

Java: "第一行\n第二行"
来源：http://lyh.cheryme.top

Go:   "第一行\n第二行"
来源：http://oed.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://xye.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://ewf.dashuyun.cn

[A14] 注释写法
来源：http://niy.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lrg.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://her.sxryk.cn

JS:   // 单行；/* 多行 */
来源：http://koa.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://wkv.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hxv.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://enx.fengsongda.top

Ruby: # 单行；=begin 多行 =end
来源：http://cah.dashuyun.cn

C#:   // 单行；/* 多行 */
来源：http://gfu.yanxiufei.cn

[A15] 空值判断与默认值
来源：http://ojx.bbcook.cn

Py:   value = data or "默认值"
来源：http://hui.yanxiufei.cn

PHP:  $value = $data ?? "默认值";
来源：http://xeg.zycfv.cn

JS:   const value = data ?? "默认值";
来源：http://mic.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://zwy.hfpthk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dmn.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://krj.cucudq.cn

Ruby: value = data || "默认值"
来源：http://ysg.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://qys.cashguo.top

[A16] 真假值判断规则
来源：http://fdm.sweek.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vyn.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lwn.andypj.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ulo.hammf.cn

TS:   if (!x) {}
来源：http://aif.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wvb.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mbz.vehdjk.com

Ruby: unless x            # nil 与 false 为假
来源：http://eov.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yei.shanyushiyangtech.top

[A17] 位运算
来源：http://hdu.yj202588.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://piu.jinghuilouyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://szh.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://plq.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vei.zdbjq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqo.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jgx.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clf.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nod.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://zot.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://rqr.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://afg.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bue.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aii.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://fsv.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lmy.shzxlz.cn

Ruby: "A".ord; 65.chr
来源：http://fhu.zhengqikj.top

C#:   (int)'A'; (char)65
来源：http://pau.ydjk.org.cn

[A19] 交换两个变量
来源：http://lqf.guannengcc.top

Py:   a, b = b, a
来源：http://mrp.wangdashe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://gjt.cashguo.top

JS:   [a, b] = [b, a];
来源：http://ifk.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://skc.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://jbi.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://tzy.jlsjyb.cn

Ruby: a, b = b, a
来源：http://sgs.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://pdv.hammf.cn

[A20] 读取标准输入
来源：http://uxp.ctjpmb.com

Py:   name = input("请输入：")
来源：http://ksq.epnwcf.com

PHP:  $name = trim(fgets(STDIN));
来源：http://zwv.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ixc.sweek.top

TS:   // Node.js：readline 模块
来源：http://qgz.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://rlo.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qcj.yj202588.top

Ruby: gets.chomp
来源：http://yks.hnqzz.top

C#:   Console.ReadLine();
来源：http://ogv.yvedp.cn

[A21] 保留指定小数位输出
来源：http://thf.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://ipg.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://saa.nwbrower.top

JS:   (3.14159).toFixed(2)
来源：http://hrg.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://osd.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://spp.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wti.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://sxo.hesvh.cn

C#:   3.14159.ToString("F2")
来源：http://vsn.ehwqpu.com

[A22] 获取字符串长度
来源：http://loh.yj20258.top

Py:   len(s)
来源：http://bji.sjlbkw.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://umg.yuanzhike.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cpn.quarkkingdee.top

TS:   s.length
来源：http://rzc.hysaishi.cn

Java: s.length()
来源：http://umk.sweek.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uty.sxryk.cn

Ruby: s.length
来源：http://ghw.hysaishi.cn

C#:   s.Length
来源：http://bnf.yanxiufei.cn

[A23] 大小写转换
来源：http://csg.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tcl.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wuf.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yke.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ugd.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rtk.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jnu.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ook.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fve.ivvv.top

[A24] 去除首尾空白
来源：http://vvy.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ddp.redwolf501.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dep.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gdb.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rzv.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nxd.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://ime.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pyu.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://spf.redwolf501.top

[A25] 字符串比较
来源：http://eqk.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://scg.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://btu.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fvy.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lwq.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gnr.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://chh.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aks.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://htw.hysaishi.cn

[A26] 类型转换总览
来源：http://xbk.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oet.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fxl.c1oappe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hfq.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://rdp.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wml.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iop.yanxiufei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://alm.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ecd.cucudq.cn

================================================================================
来源：http://nue.hnxiangtu.top

B. 流程控制
来源：http://vpx.cucudq.cn

================================================================================
来源：http://xrl.yuanzhike.top

[B01] 条件判断 if / else
来源：http://cyy.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gqt.gogol.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mtg.vqdsnc.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mak.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hqf.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iiw.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fxg.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hlf.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wzz.c1oappe.top

[B02] 多分支 else if / elif
来源：http://ehv.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://axv.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yuo.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kog.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijh.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rls.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jlg.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bvt.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wnx.yj202588.top

[B03] switch / match / case
来源：http://evf.zycfv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ysk.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sel.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wts.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ibn.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iag.316326.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wce.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zjb.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nfe.birdmap.top

[B04] for 计数循环
来源：http://nzl.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://zpj.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hhs.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://soi.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cpt.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fwc.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dzb.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://yyp.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vor.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://aiv.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://uur.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kos.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rji.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hob.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hxd.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fqu.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://alx.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kpl.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://cyv.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gzn.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pxr.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uth.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ymr.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ilb.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uve.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bqc.tianlin.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yea.bbcook.cn

[B07] while 循环
来源：http://vdm.sysykeji.top

Py:   while i < 10: i += 1
来源：http://hbx.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nwz.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://koh.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://zfv.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://ckm.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qcz.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://brl.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://uro.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://ner.jqgufenzy.top


<!-- 参考信息 -->