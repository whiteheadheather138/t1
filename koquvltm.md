代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hly.kuanghao11.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://glq.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dts.gotoacloud.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wuh.fktsv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ciz.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xpz.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fgv.chenlongwang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://att.c1oappe.top

================================================================================
来源：http://nnm.gotoacloud.top

A. 基础语法与类型
来源：http://nib.gzhubu.top

================================================================================
来源：http://cti.feifeiyinyue.top

[A01] Hello World
来源：http://mjy.aizwys.cn

Py:   print("Hello, World!")
来源：http://jhc.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://aou.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://fcl.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rcf.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://grq.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://ist.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://zez.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://nhg.vqdsnc.cn

[A02] 变量声明与赋值
来源：http://lqj.snrcjt.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tvt.hnxiangtu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mex.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://jum.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sbo.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://bzz.hnxiangtu.top

Go:   name := "Alex"; age := 20
来源：http://kew.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://xke.zhiwuduotai.top

C#:   string name = "Alex"; int age = 20;
来源：http://stq.zdqjudy.top

[A03] 常量定义
来源：http://ovm.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ilm.xinyue.icu

PHP:  const PI = 3.14159;
来源：http://rrj.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://yri.wangdashe.top

TS:   const PI: number = 3.14159;
来源：http://yyi.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://dkx.gotoacloud.top

Go:   const PI = 3.14159
来源：http://yeu.zhengqikj.top

Ruby: PI = 3.14159
来源：http://xcz.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://neg.havefunace.top

[A04] 判断变量类型
来源：http://aqr.svipenyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xwx.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bze.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ewg.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://gxl.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sfb.gotoacloud.top

Go:   reflect.TypeOf(x).Name()
来源：http://cks.zhijiandao.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tur.jiagoushi.top

C#:   x.GetType().Name; x is int
来源：http://epc.tarul.cn

[A05] 整数除法与取模
来源：http://tit.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fzz.aizwys.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sak.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qpf.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xnu.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://hpf.xuetiantiany.cn

Go:   7 / 2; 7 % 2
来源：http://gah.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://iwt.gotoacloud.top

C#:   7 / 2; 7 % 2
来源：http://hro.birdmap.top

[A06] 字符串转数字
来源：http://nur.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://qbw.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tpa.tanke756.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qdi.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ppp.tianlin.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zle.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yxn.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ham.quarkkingdee.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jwo.shzxlz.cn

[A07] 数字转字符串
来源：http://zul.meibo888.top

Py:   str(42)
来源：http://fbi.wangdashe.top

PHP:  (string) 42; strval(42)
来源：http://yyt.zhongyouzk.top

JS:   String(42); (42).toString()
来源：http://oda.yuxming.cn

TS:   String(42)
来源：http://nwc.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fue.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://yjs.zhijiandao.cn

Ruby: 42.to_s
来源：http://ahf.svipenyu.cn

C#:   42.ToString()
来源：http://lhh.nanxinkj.top

[A08] 取整与四舍五入
来源：http://sjh.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hpl.zdqjudy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uoj.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mhf.pengpengdd.cyou

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xio.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://std.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://khx.andypj.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://mpj.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://npo.zhixingplan.top

[A09] 绝对值与最大最小值
来源：http://mjl.tianlin.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ode.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://soq.mhx1999.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nat.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lkx.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uak.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hob.hnqzz.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://thh.zhoulong.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://odm.snrcjt.cn

[A10] 生成随机数
来源：http://srp.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://ugl.uphjek.com

PHP:  random_int(1, 100);
来源：http://vyy.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bpt.sufxvd.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kup.epnwcf.com

Java: new Random().nextInt(100) + 1
来源：http://mda.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yds.fktsv.cn

Ruby: rand(1..100)
来源：http://gmx.pengpengdd.cyou

C#:   new Random().Next(1, 101)
来源：http://ydo.iojbl.cn

[A11] 条件表达式（三元）
来源：http://ihj.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://rdz.zhoulong.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://uxw.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nul.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://uxs.tian-w.cn

Java: x > 0 ? "yes" : "no"
来源：http://xeb.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ilc.sweek.top

Ruby: x > 0 ? "yes" : "no"
来源：http://efh.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dtq.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://own.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tbf.sxryk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mks.pengpengdd.cyou

JS:   `Hello, ${name}!`
来源：http://zzw.hongshengwenyu.top

TS:   `Hello, ${name}!`
来源：http://ydz.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://lwo.tanke756.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://syx.jyoumei.cn

Ruby: "Hello, #{name}!"
来源：http://hvs.jiagoushi.top

C#:   $"Hello, {name}!"
来源：http://tve.svipenyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qnc.jqgufenzy.top

Py:   "第一行\n第二行"
来源：http://jxp.wangshuangyany.cn

PHP:  "第一行\n第二行"
来源：http://llc.cucudq.cn

JS:   "第一行\n第二行"
来源：http://naj.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://ocm.jyoumei.cn

Java: "第一行\n第二行"
来源：http://sph.havefunace.top

Go:   "第一行\n第二行"
来源：http://pjx.hysaishi.cn

Ruby: "第一行\n第二行"
来源：http://jmc.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://hls.nanxinkj.top

[A14] 注释写法
来源：http://xpa.meibo888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jps.wangshuangyany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uwe.haohaochexian.top

JS:   // 单行；/* 多行 */
来源：http://vec.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://hwx.cqqwz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pgf.cqqwz.cn

Go:   // 单行；/* 多行 */
来源：http://jbw.chenlongwang.top

Ruby: # 单行；=begin 多行 =end
来源：http://yic.zhixingplan.top

C#:   // 单行；/* 多行 */
来源：http://sce.jianghu66.top

[A15] 空值判断与默认值
来源：http://yfb.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://gur.dianchejie.cn

PHP:  $value = $data ?? "默认值";
来源：http://ukh.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://dih.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://lep.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://olo.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://jjh.dashuyun.cn

Ruby: value = data || "默认值"
来源：http://bmd.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://epz.nanxinkj.top

[A16] 真假值判断规则
来源：http://xpg.gaohongyu789.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xca.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ttk.meibo888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zih.smart0.xyz

TS:   if (!x) {}
来源：http://mkd.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lju.cucudq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ole.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://odj.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jsq.guannengcc.top

[A17] 位运算
来源：http://cni.gzhubu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pob.mhx1999.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blj.aizwys.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://csf.zhongyouzk.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://war.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sul.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vxs.zhengqikj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rvc.fehbvm.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oec.zhiwuduotai.top

[A18] 字符与 ASCII 码互转
来源：http://ugk.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://oxu.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://vzb.shanyushiyangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kxl.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://psd.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://ber.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rhh.zhiwuduotai.top

Ruby: "A".ord; 65.chr
来源：http://olp.fktsv.cn

C#:   (int)'A'; (char)65
来源：http://oqw.ivvv.top

[A19] 交换两个变量
来源：http://wky.quarkkingdee.top

Py:   a, b = b, a
来源：http://ysc.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xvr.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://nys.mhx1999.top

TS:   [a, b] = [b, a];
来源：http://rev.fanxiaobao.xyz

Java: int t = a; a = b; b = t;
来源：http://ams.aizwys.cn

Go:   a, b = b, a
来源：http://lfg.jinqigfzy.top

Ruby: a, b = b, a
来源：http://hix.epnwcf.com

C#:   (a, b) = (b, a);
来源：http://bpb.hfpthk.cn

[A20] 读取标准输入
来源：http://ikh.svipenyu.cn

Py:   name = input("请输入：")
来源：http://wmd.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rza.yongpay.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tdn.ivvv.top

TS:   // Node.js：readline 模块
来源：http://aoe.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://ktf.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mli.birdmap.top

Ruby: gets.chomp
来源：http://uxg.fehbvm.com

C#:   Console.ReadLine();
来源：http://vzi.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://vmx.ppjwa.cn

Py:   f"{3.14159:.2f}"
来源：http://zrc.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wrk.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://hzt.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://urf.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://idv.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eqh.wangshuangyany.cn

Ruby: format("%.2f", 3.14159)
来源：http://hgt.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://cfz.yj20258.top

[A22] 获取字符串长度
来源：http://emu.jyoumei.cn

Py:   len(s)
来源：http://ngj.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lpg.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kgw.birdmap.top

TS:   s.length
来源：http://jnv.aibaodan.cn

Java: s.length()
来源：http://ngz.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://par.jqgufenzy.top

Ruby: s.length
来源：http://tfy.feifeiyinyue.top

C#:   s.Length
来源：http://esw.jianghu66.top

[A23] 大小写转换
来源：http://fgh.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://poc.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rjw.ctjpmb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ybl.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lym.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rwz.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ybl.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mio.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://fjj.jqgfzy.top

[A24] 去除首尾空白
来源：http://ufd.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xae.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ohi.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eim.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ycl.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sar.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://zuu.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mbx.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oyx.tarul.cn

[A25] 字符串比较
来源：http://amf.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://nlz.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vdk.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xqv.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://par.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jar.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wkb.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://msr.quarkkingdee.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nbw.svipenyu.cn

[A26] 类型转换总览
来源：http://azt.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bty.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jrv.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wyy.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://ccy.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nti.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yky.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lbp.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://odd.shuidangran.top

================================================================================
来源：http://nqe.cashguo.top

B. 流程控制
来源：http://slw.jinghuilouyu.cn

================================================================================
来源：http://ydy.zycfv.cn

[B01] 条件判断 if / else
来源：http://qqv.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kyg.yonumen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sxb.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mnm.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hjl.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://esy.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eym.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ctz.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fvj.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://lml.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ueh.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ohp.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggi.yj20258.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpk.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tjo.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://srl.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nsd.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpz.hywenlv.cn

[B03] switch / match / case
来源：http://oxc.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pkw.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://coz.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://avl.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mjp.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wka.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hfs.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lpw.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rxj.mhx1999.top

[B04] for 计数循环
来源：http://mic.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://hoz.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qox.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kua.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lux.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yhe.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wds.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://edd.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cvk.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://boj.gzhubu.top

Py:   for item in arr: print(item)
来源：http://pej.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rnn.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iow.zhongyouzk.top

TS:   for (const item of arr) { console.log(item); }
来源：http://esl.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dhw.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cyd.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://jkv.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pjq.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://glf.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xfw.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hmw.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eey.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hyk.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://brq.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://azm.xziqi.cn


<!-- 参考信息 -->