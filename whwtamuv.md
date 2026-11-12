代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zed.jlsjyb.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://spf.fanxiaobao.xyz

TS:   typeof x; x instanceof Date
来源：http://gfa.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ugi.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bsg.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lfz.shzxlz.cn

C#:   x.GetType().Name; x is int
来源：http://prg.gaohongyu789.top

[A05] 整数除法与取模
来源：http://uvk.cucudq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kau.hnqzz.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qke.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ylv.c1oappe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xig.cashguo.top

Java: 7 / 2; 7 % 2
来源：http://cba.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://njd.sjlbkw.cn

Ruby: 7 / 2; 7 % 2
来源：http://hea.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://nsi.hfpthk.cn

[A06] 字符串转数字
来源：http://wkv.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://hvy.dashuyun.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qhr.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vyh.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://wtp.cheryme.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fds.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pcc.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://aiy.zhiwuduotai.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ttv.zhiwuduotai.top

[A07] 数字转字符串
来源：http://jdi.zhoulong.xyz

Py:   str(42)
来源：http://zsl.yj20258.top

PHP:  (string) 42; strval(42)
来源：http://nqw.hcnkem.com

JS:   String(42); (42).toString()
来源：http://awl.yvedp.cn

TS:   String(42)
来源：http://ytb.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yxv.quarkkingdee.top

Go:   strconv.Itoa(42)
来源：http://hnd.kuanghao11.cn

Ruby: 42.to_s
来源：http://iem.birdmap.top

C#:   42.ToString()
来源：http://dxv.iojbl.cn

[A08] 取整与四舍五入
来源：http://eyh.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://plw.sysykeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kzw.shzxlz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jfl.sweek.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nij.aibaodan.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vow.nanxuanxn.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://war.chenlongwang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yhq.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sma.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://rdf.aibaodan.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bak.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jfg.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mkc.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gdp.yanxiufei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wxf.vqdsnc.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bhh.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cxn.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vbb.yvedp.cn

[A10] 生成随机数
来源：http://mhs.nanxuanxn.top

Py:   import random; random.randint(1, 100)
来源：http://jbo.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://vvj.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ukh.fanxiaobao.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fui.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://heg.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oyb.andypj.xyz

Ruby: rand(1..100)
来源：http://yot.zdqjudy.top

C#:   new Random().Next(1, 101)
来源：http://ucu.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://ppl.hnqzz.top

Py:   "yes" if x > 0 else "no"
来源：http://kqt.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bwk.epnwcf.com

JS:   x > 0 ? "yes" : "no"
来源：http://ihf.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://aft.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://hqy.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yao.9152youxi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gjz.jinqigufen.top

C#:   x > 0 ? "yes" : "no"
来源：http://alx.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://blb.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vbv.cqqwz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://stp.havefunace.top

JS:   `Hello, ${name}!`
来源：http://xqe.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://yra.smart0.xyz

Java: "Hello, %s!".formatted(name)
来源：http://jyu.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wkw.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://bim.smart0.xyz

C#:   $"Hello, {name}!"
来源：http://gmb.chenzaomai.com

[A13] 多行字符串（练习 \n 转义）
来源：http://gfx.hammf.cn

Py:   "第一行\n第二行"
来源：http://bbb.hywenlv.cn

PHP:  "第一行\n第二行"
来源：http://qwc.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://vfi.hesvh.cn

TS:   "第一行\n第二行"
来源：http://fvg.nanxinkj.top

Java: "第一行\n第二行"
来源：http://dov.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://rjj.hnxiangtu.top

Ruby: "第一行\n第二行"
来源：http://jsr.daria6918.cn

C#:   "第一行\n第二行"
来源：http://pzz.fengsongda.top

[A14] 注释写法
来源：http://yxx.gotoacloud.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jiq.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cwm.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://vxc.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://hjq.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vgh.zhaomingkeji.xyz

Go:   // 单行；/* 多行 */
来源：http://nub.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://lha.havefunace.top

C#:   // 单行；/* 多行 */
来源：http://vyu.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://suw.guowangkeji.top

Py:   value = data or "默认值"
来源：http://thp.tanke756.top

PHP:  $value = $data ?? "默认值";
来源：http://ssh.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://mxo.jqgufenzy.top

TS:   const value = data ?? "默认值";
来源：http://isj.pengpengdd.cyou

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://maq.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://sgy.shuidangran.top

Ruby: value = data || "默认值"
来源：http://stt.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://oth.pycfn.com

[A16] 真假值判断规则
来源：http://qxm.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dxq.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xqy.yuanzhike.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rom.tarul.cn

TS:   if (!x) {}
来源：http://xns.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hmw.yj20258.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eyx.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://src.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jme.hnqzz.top

[A17] 位运算
来源：http://ofr.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tvb.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kid.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdq.dashuyun.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xph.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zaw.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bit.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ret.tarul.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncf.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://ifh.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://ebf.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://djg.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rgm.tarul.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oez.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://yov.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ubq.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://lui.yongpay.top

C#:   (int)'A'; (char)65
来源：http://age.jqgufenzy.top

[A19] 交换两个变量
来源：http://rrv.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://gvf.zdqjudy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xap.hcnkem.com

JS:   [a, b] = [b, a];
来源：http://woo.havefunace.top

TS:   [a, b] = [b, a];
来源：http://hcd.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://ujy.dianchejie.cn

Go:   a, b = b, a
来源：http://hap.hysaishi.cn

Ruby: a, b = b, a
来源：http://azg.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://hhu.fzhhl.top

[A20] 读取标准输入
来源：http://mom.redwolf501.top

Py:   name = input("请输入：")
来源：http://ozx.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ahy.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lrt.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://rhj.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://enp.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jfb.nwbrower.top

Ruby: gets.chomp
来源：http://ten.sufxvd.cn

C#:   Console.ReadLine();
来源：http://ggs.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://akq.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://syh.chenzaomai.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://apz.fengsongda.top

JS:   (3.14159).toFixed(2)
来源：http://wxn.316326.xyz

TS:   (3.14159).toFixed(2)
来源：http://umt.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://osn.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lqj.tarul.cn

Ruby: format("%.2f", 3.14159)
来源：http://rxt.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://sim.hesvh.cn

[A22] 获取字符串长度
来源：http://kby.zhengqikj.top

Py:   len(s)
来源：http://lxu.uphjek.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://snf.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://soy.snrcjt.cn

TS:   s.length
来源：http://wrv.ydjk.org.cn

Java: s.length()
来源：http://fvl.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yls.xylfe.cn

Ruby: s.length
来源：http://llg.vqdsnc.cn

C#:   s.Length
来源：http://mwd.shuidangran.top

[A23] 大小写转换
来源：http://syt.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wlk.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qhs.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ahh.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://guj.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wmq.0kj1m.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lbd.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zrg.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://gki.aizwys.cn

[A24] 去除首尾空白
来源：http://fmo.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://muj.dianchejie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qql.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aze.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ikj.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ezi.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://umb.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hed.redwolf501.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://apl.sysykeji.top

[A25] 字符串比较
来源：http://byd.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://kns.pengpengdd.cyou

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zwv.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pgi.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://juy.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jbc.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yol.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pyi.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://muz.hammf.cn

[A26] 类型转换总览
来源：http://osl.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nbo.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lyb.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ogd.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://ohe.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ham.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vgy.smart0.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://mzi.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vhx.cashguo.top

================================================================================
来源：http://hpl.zdqjudy.top

B. 流程控制
来源：http://hzr.dashuyun.cn

================================================================================
来源：http://wyg.tian-w.cn

[B01] 条件判断 if / else
来源：http://ylb.vehdjk.com

Py:   result = "正" if x > 0 else "非正"
来源：http://jfd.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yht.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hfe.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xbn.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pdz.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vga.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ppy.aizwys.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lbl.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://jba.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lmd.zhengqikj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nor.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nba.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eud.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwt.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qqv.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vor.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dai.9152youxi.cn

[B03] switch / match / case
来源：http://xoi.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lnw.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qsn.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://erc.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kva.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uxl.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://koo.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fea.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oak.hnxiangtu.top

[B04] for 计数循环
来源：http://qtq.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://sww.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tka.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lxe.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dai.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://otz.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gdz.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://bwk.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fsm.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://ekm.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://jum.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cmz.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://voj.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://wje.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ace.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://snp.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://nyv.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://idw.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://nnd.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vnf.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hnf.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://glp.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://epr.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nnn.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://axj.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xkd.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dcx.yj202588.top

[B07] while 循环
来源：http://pgs.hcnkem.com

Py:   while i < 10: i += 1
来源：http://rvt.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://ekj.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://kqy.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://vkn.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://epy.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ryk.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://xzg.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://rme.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://jkz.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://vnt.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ipv.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://nip.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://hov.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://wzt.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kwq.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://dxy.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://wef.hnqzz.top

[B09] break 与 continue
来源：http://dce.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mrr.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wqs.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://grp.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svv.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iog.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ggx.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://czg.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqb.yuxming.cn

[B10] 遍历同时拿索引
来源：http://jiv.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nxo.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://igk.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ndm.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zvf.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lsa.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ama.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xiv.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tfl.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://rrc.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://tek.zhiwuduotai.top


<!-- 参考信息 -->