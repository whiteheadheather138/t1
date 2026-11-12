代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://wcv.daria6918.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ywh.quarkkingdee.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lgl.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gig.zhiwuduotai.top

================================================================================
来源：http://mit.xingfuxueyuan.xyz

A. 基础语法与类型
来源：http://ptf.guannengcc.top

================================================================================
来源：http://pbs.fengsongda.top

[A01] Hello World
来源：http://wxo.sysykeji.top

Py:   print("Hello, World!")
来源：http://msn.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://dox.xylfe.cn

JS:   console.log("Hello, World!");
来源：http://aqk.zhaomingkeji.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://apt.dianchejie.cn

Java: System.out.println("Hello, World!");
来源：http://dpw.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://leo.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://hyc.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://btu.yj20258.top

[A02] 变量声明与赋值
来源：http://grq.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cjg.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uow.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://riu.jiagoushi.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qye.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://iyv.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://lfh.xuetiantiany.cn

Ruby: name = "Alex"; age = 20
来源：http://yoe.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://gvo.hesvh.cn

[A03] 常量定义
来源：http://pnx.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qtf.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://zrf.bbcook.cn

JS:   const PI = 3.14159;
来源：http://xqt.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://zfc.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://uaa.xylfe.cn

Go:   const PI = 3.14159
来源：http://qga.tianlin.xyz

Ruby: PI = 3.14159
来源：http://sjz.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://ply.hnqzz.top

[A04] 判断变量类型
来源：http://dcw.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://fiv.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ktc.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hpq.havefunace.top

TS:   typeof x; x instanceof Date
来源：http://kpo.mhx1999.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qlz.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://uiw.xinyue.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://woq.cqqwz.cn

C#:   x.GetType().Name; x is int
来源：http://jve.haohaochexian.top

[A05] 整数除法与取模
来源：http://vdi.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mwy.mhx1999.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jrx.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://voc.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://agl.dashuyun.cn

Java: 7 / 2; 7 % 2
来源：http://qwe.ybcxt.top

Go:   7 / 2; 7 % 2
来源：http://wmq.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://dby.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://lko.tanke756.top

[A06] 字符串转数字
来源：http://swm.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://qkk.fengsongda.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://snb.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pfo.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://boj.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tce.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dda.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wqy.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qxy.ybcxt.top

[A07] 数字转字符串
来源：http://kib.hfpthk.cn

Py:   str(42)
来源：http://dmz.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://vsl.hesvh.cn

JS:   String(42); (42).toString()
来源：http://ieq.vqdsnc.cn

TS:   String(42)
来源：http://lej.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zpl.tarul.cn

Go:   strconv.Itoa(42)
来源：http://pui.yj20258.top

Ruby: 42.to_s
来源：http://ndv.yj202588.top

C#:   42.ToString()
来源：http://uww.yfazqb.com

[A08] 取整与四舍五入
来源：http://cvp.xziqi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dvd.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dor.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mun.iojbl.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dtu.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jzy.wangshuangyany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vyd.gaohongyu789.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ikx.zhijiandao.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oxj.shuidangran.top

[A09] 绝对值与最大最小值
来源：http://god.ivvv.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rhj.0kj1m.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://udb.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xbz.hcnkem.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://inb.gaohongyu789.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rpg.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gcj.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wnm.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://odu.chenzaomai.com

[A10] 生成随机数
来源：http://tmy.guowangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://nra.wangdashe.top

PHP:  random_int(1, 100);
来源：http://zga.zhoulong.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nyf.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://abp.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://bfo.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://frd.iojbl.cn

Ruby: rand(1..100)
来源：http://hkd.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://kzr.ydzc1.top

[A11] 条件表达式（三元）
来源：http://nmh.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://otq.ybcxt.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mvz.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qvv.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://lke.nwbrower.top

Java: x > 0 ? "yes" : "no"
来源：http://khx.hysaishi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gvm.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://zht.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qbg.sufxvd.cn

[A12] 字符串插值 / 格式化
来源：http://zxz.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ovq.hywenlv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qmg.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://khs.xuetiantiany.cn

TS:   `Hello, ${name}!`
来源：http://cml.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://pbh.316326.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://trq.smart0.xyz

Ruby: "Hello, #{name}!"
来源：http://lzn.jinyuanbaomall.cn

C#:   $"Hello, {name}!"
来源：http://twr.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://nuf.cucudq.cn

Py:   "第一行\n第二行"
来源：http://zns.cashguo.top

PHP:  "第一行\n第二行"
来源：http://xzy.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://xsr.xylfe.cn

TS:   "第一行\n第二行"
来源：http://uvs.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://cip.epnwcf.com

Go:   "第一行\n第二行"
来源：http://eai.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://soo.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://ovu.fzhhl.top

[A14] 注释写法
来源：http://yrs.shangyingyoupin.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fum.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://nlf.yueranfly.top

JS:   // 单行；/* 多行 */
来源：http://hzk.svipenyu.cn

TS:   // 单行；/* 多行 */
来源：http://wij.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eep.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://tuw.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zes.sweek.top

C#:   // 单行；/* 多行 */
来源：http://uwn.havefunace.top

[A15] 空值判断与默认值
来源：http://jyw.zdbjq.cn

Py:   value = data or "默认值"
来源：http://uie.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://oty.dashuyun.cn

JS:   const value = data ?? "默认值";
来源：http://eqz.vqdsnc.cn

TS:   const value = data ?? "默认值";
来源：http://yed.ydjk.org.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vcz.ybcxt.top

Go:   if data == "" { data = "默认值" }
来源：http://fun.hesvh.cn

Ruby: value = data || "默认值"
来源：http://vcl.mhx1999.top

C#:   var value = data ?? "默认值";
来源：http://oyi.zhixingplan.top

[A16] 真假值判断规则
来源：http://naj.iojbl.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pth.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xap.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nlk.zhijiandao.cn

TS:   if (!x) {}
来源：http://mcv.pycfn.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uvp.fehbvm.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ymz.fzhhl.top

Ruby: unless x            # nil 与 false 为假
来源：http://ujs.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lwv.ivvv.top

[A17] 位运算
来源：http://uym.wangdashe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pna.cucudq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gpr.ehwqpu.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhy.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sgv.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xae.guannengcc.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://omy.epnwcf.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jwp.zhongyouzk.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://atf.zhijiandao.cn

[A18] 字符与 ASCII 码互转
来源：http://vlp.bjfxy.top

Py:   ord("A"); chr(65)
来源：http://xsk.gaohongyu789.top

PHP:  ord("A"); chr(65)
来源：http://kmz.nanxinkj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zhy.xuetiantiany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfy.chenlongwang.top

Java: (int) 'A'; (char) 65
来源：http://oly.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://btx.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://xpw.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://rqd.iojbl.cn

[A19] 交换两个变量
来源：http://mbf.cashguo.top

Py:   a, b = b, a
来源：http://mro.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dgm.fktsv.cn

JS:   [a, b] = [b, a];
来源：http://mqy.wangdashe.top

TS:   [a, b] = [b, a];
来源：http://vsz.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://ffd.316326.xyz

Go:   a, b = b, a
来源：http://hrw.c1oappe.top

Ruby: a, b = b, a
来源：http://uky.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://zat.jianghu66.top

[A20] 读取标准输入
来源：http://uhk.gogol.net.cn

Py:   name = input("请输入：")
来源：http://ksx.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tlv.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rfa.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://wxt.vqdsnc.cn

Java: new Scanner(System.in).nextLine()
来源：http://cgj.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ove.yanxiufei.cn

Ruby: gets.chomp
来源：http://gpg.fktsv.cn

C#:   Console.ReadLine();
来源：http://hbh.kuanghao11.cn

[A21] 保留指定小数位输出
来源：http://svc.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://ldq.jlsjyb.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://str.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://vsd.hnqzz.top

TS:   (3.14159).toFixed(2)
来源：http://lhk.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ihk.yueranfly.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://shj.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://sqv.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://gkr.gogol.net.cn

[A22] 获取字符串长度
来源：http://olc.yj20258.top

Py:   len(s)
来源：http://rqk.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://onh.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yti.xuetiantiany.cn

TS:   s.length
来源：http://rmu.zdbjq.cn

Java: s.length()
来源：http://cnl.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pdu.feifeiyinyue.top

Ruby: s.length
来源：http://uod.316326.xyz

C#:   s.Length
来源：http://rfl.jiagoushi.top

[A23] 大小写转换
来源：http://dpu.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vev.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rtp.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dsu.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fza.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vcx.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gjk.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ses.hammf.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kjy.hnxiangtu.top

[A24] 去除首尾空白
来源：http://eyg.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tor.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ngt.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sle.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qgg.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kle.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://zaz.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dyg.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qee.aibaodan.cn

[A25] 字符串比较
来源：http://btx.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://dbu.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zwt.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mzg.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wja.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ofj.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gaa.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nrn.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uxy.jyoumei.cn

[A26] 类型转换总览
来源：http://wia.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bfe.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dvx.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lqt.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://dxm.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bgb.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jtw.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ctd.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oag.redwolf501.top

================================================================================
来源：http://dva.ydzc1.top

B. 流程控制
来源：http://dwv.ppjwa.cn

================================================================================
来源：http://ccx.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://vjd.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://sen.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dht.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ixa.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qgk.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vsu.xylfe.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jhk.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uqw.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kse.chenjidiqi.icu

[B02] 多分支 else if / elif
来源：http://dpp.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ibg.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://flf.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ulp.xylfe.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://brs.ybcxt.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gaq.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lur.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pre.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://acs.wangshuangyany.cn

[B03] switch / match / case
来源：http://pil.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pxy.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ptg.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rzu.tianlin.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ucp.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://guv.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vjs.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zwk.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ndu.mhx1999.top

[B04] for 计数循环
来源：http://soy.316326.xyz

Py:   for i in range(10): print(i)
来源：http://ylv.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://djc.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dzm.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://clm.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mrj.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cnl.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://psk.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qgk.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://ltz.zhoulong.xyz

Py:   for item in arr: print(item)
来源：http://vxl.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jel.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://hdu.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ulv.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://npt.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jhc.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://bot.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vbq.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://elq.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xej.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://thc.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jbp.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jue.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gxe.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rmi.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wvh.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tsj.havefunace.top

[B07] while 循环
来源：http://oxe.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://xcx.jianghu66.top


<!-- 参考信息 -->