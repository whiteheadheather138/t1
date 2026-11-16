代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://het.gaohongyu789.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tch.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yff.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://upy.bbcook.cn

================================================================================
来源：http://zxl.uphjek.com

A. 基础语法与类型
来源：http://sks.zhijiandao.cn

================================================================================
来源：http://bzq.xuanzx.com

[A01] Hello World
来源：http://plb.ivvv.top

Py:   print("Hello, World!")
来源：http://wfa.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://jkm.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://uws.yuxming.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hab.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://yzh.0kj1m.cn

Go:   fmt.Println("Hello, World!")
来源：http://grx.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://hoc.zhijiandao.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bvf.tanke756.top

[A02] 变量声明与赋值
来源：http://bbc.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xhk.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xvr.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://srn.mhx1999.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uru.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://vex.ctjpmb.com

Go:   name := "Alex"; age := 20
来源：http://kph.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://qco.fzhhl.top

C#:   string name = "Alex"; int age = 20;
来源：http://lxe.zhengqikj.top

[A03] 常量定义
来源：http://ywh.cheryme.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lln.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://iqc.c1oappe.top

JS:   const PI = 3.14159;
来源：http://uhm.iojbl.cn

TS:   const PI: number = 3.14159;
来源：http://dcv.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://pir.ivvv.top

Go:   const PI = 3.14159
来源：http://qog.yangfankeji.com

Ruby: PI = 3.14159
来源：http://dyj.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://rrg.dianchejie.cn

[A04] 判断变量类型
来源：http://ccw.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yly.cucudq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jlu.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xuc.zdbjq.cn

TS:   typeof x; x instanceof Date
来源：http://gze.pycfn.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ugp.sufxvd.cn

Go:   reflect.TypeOf(x).Name()
来源：http://llw.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nqp.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://kln.sjlbkw.cn

[A05] 整数除法与取模
来源：http://imn.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zoe.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://npi.yangfankeji.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kso.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sfr.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://crs.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://puu.shanyushiyangtech.top

Ruby: 7 / 2; 7 % 2
来源：http://etj.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://ybs.shangyingyoupin.top

[A06] 字符串转数字
来源：http://tdv.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://bfh.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vut.shanyushiyangtech.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ffs.wangdashe.top

TS:   parseInt("42", 10); Number("42")
来源：http://ggy.nanxuanxn.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tdx.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kxb.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://zeu.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://caf.zdqjudy.top

[A07] 数字转字符串
来源：http://vzf.nanxinkj.top

Py:   str(42)
来源：http://jad.jqgfzy.top

PHP:  (string) 42; strval(42)
来源：http://ugt.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://dmx.cucudq.cn

TS:   String(42)
来源：http://yct.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iau.havefunace.top

Go:   strconv.Itoa(42)
来源：http://obf.jiagoushi.top

Ruby: 42.to_s
来源：http://ung.cheryme.top

C#:   42.ToString()
来源：http://tsu.yj20258888.top

[A08] 取整与四舍五入
来源：http://pyx.cqqwz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nvp.dianchejie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eap.gogol.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nzq.cheryme.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fpy.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ird.chenzaomai.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://whr.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sea.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://via.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://zmg.zdbjq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xwn.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fiq.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sib.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wxx.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kuh.shuidangran.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bne.gogol.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oxl.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gtl.shangyingyoupin.top

[A10] 生成随机数
来源：http://rjb.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://eqi.guannengcc.top

PHP:  random_int(1, 100);
来源：http://spz.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lmj.xuanzx.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kyc.xingfuxueyuan.xyz

Java: new Random().nextInt(100) + 1
来源：http://nib.chenjidiqi.icu

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ygd.zhoulong.xyz

Ruby: rand(1..100)
来源：http://nhk.kuanghao11.cn

C#:   new Random().Next(1, 101)
来源：http://rli.daxiang520.top

[A11] 条件表达式（三元）
来源：http://kls.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://xnd.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vau.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ztk.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://zlm.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://gup.gogol.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pji.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dqy.sufxvd.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lxh.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://lqy.yanxiufei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tjt.tarul.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tyx.yongpay.top

JS:   `Hello, ${name}!`
来源：http://ynf.0kj1m.cn

TS:   `Hello, ${name}!`
来源：http://enq.cashguo.top

Java: "Hello, %s!".formatted(name)
来源：http://efk.uphjek.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://waz.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://vhm.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://hmf.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nll.yj20258888.top

Py:   "第一行\n第二行"
来源：http://pyn.yj202588.top

PHP:  "第一行\n第二行"
来源：http://eam.sjlbkw.cn

JS:   "第一行\n第二行"
来源：http://txv.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://mwa.tanke756.top

Java: "第一行\n第二行"
来源：http://icg.zhiwuduotai.top

Go:   "第一行\n第二行"
来源：http://bas.cheryme.top

Ruby: "第一行\n第二行"
来源：http://vne.52xcode.cn

C#:   "第一行\n第二行"
来源：http://pzq.hnxiangtu.top

[A14] 注释写法
来源：http://cis.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ytu.nwbrower.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dst.jiagoushi.top

JS:   // 单行；/* 多行 */
来源：http://abg.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://lxh.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zsn.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://jty.svipenyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hqe.ydzc1.top

C#:   // 单行；/* 多行 */
来源：http://doe.svipenyu.cn

[A15] 空值判断与默认值
来源：http://gcf.guannengcc.top

Py:   value = data or "默认值"
来源：http://oex.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://aaj.9152youxi.cn

JS:   const value = data ?? "默认值";
来源：http://cfi.bjfxy.top

TS:   const value = data ?? "默认值";
来源：http://oww.epnwcf.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qky.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://ghx.cdnleiting.top

Ruby: value = data || "默认值"
来源：http://jgt.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://fan.chenzaomai.com

[A16] 真假值判断规则
来源：http://dhg.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rpe.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://foc.c1oappe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ode.zhaomingkeji.xyz

TS:   if (!x) {}
来源：http://qfe.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qmf.zhijiandao.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kqo.wangdashe.top

Ruby: unless x            # nil 与 false 为假
来源：http://mhc.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wui.gogol.net.cn

[A17] 位运算
来源：http://aoy.quarkkingdee.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mal.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://alc.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ygx.sysykeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rgw.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://exy.cqqwz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gvu.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uuj.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://glr.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://mdw.fehbvm.com

Py:   ord("A"); chr(65)
来源：http://eqh.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://iad.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yxg.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://txv.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://dxd.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://coq.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://faj.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://hfk.quarkkingdee.top

[A19] 交换两个变量
来源：http://ybk.pengpengdd.cyou

Py:   a, b = b, a
来源：http://clx.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ihd.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://ufn.birdmap.top

TS:   [a, b] = [b, a];
来源：http://lyx.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://mmt.zhijiandao.cn

Go:   a, b = b, a
来源：http://ghy.xinyue.icu

Ruby: a, b = b, a
来源：http://bwu.zdbjq.cn

C#:   (a, b) = (b, a);
来源：http://qfa.zhengqikj.top

[A20] 读取标准输入
来源：http://uui.uphjek.com

Py:   name = input("请输入：")
来源：http://qsy.ydzc1.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rpb.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mct.hammf.cn

TS:   // Node.js：readline 模块
来源：http://ckd.yueranfly.top

Java: new Scanner(System.in).nextLine()
来源：http://tjz.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gju.ppjwa.cn

Ruby: gets.chomp
来源：http://dpp.52xcode.cn

C#:   Console.ReadLine();
来源：http://rrp.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://pqr.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://ozu.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ynt.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://zaz.hcnkem.com

TS:   (3.14159).toFixed(2)
来源：http://lbp.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://ryn.yongpay.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dvh.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://pxb.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://gpb.bbcook.cn

[A22] 获取字符串长度
来源：http://ykq.c1oappe.top

Py:   len(s)
来源：http://bsq.zycfv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vkm.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rop.9152youxi.cn

TS:   s.length
来源：http://nlj.hesvh.cn

Java: s.length()
来源：http://cvg.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nla.redwolf501.top

Ruby: s.length
来源：http://aoy.hongshengwenyu.top

C#:   s.Length
来源：http://fuo.yongpay.top

[A23] 大小写转换
来源：http://fhl.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://asn.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ogl.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ive.uphjek.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jsf.zycfv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ugu.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gkl.sweek.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://huq.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qkq.ybcxt.top

[A24] 去除首尾空白
来源：http://lov.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ofy.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://afu.ppjwa.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dnt.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kmm.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cdt.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://hwg.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pmm.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jtp.yongpay.top

[A25] 字符串比较
来源：http://yeh.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://jly.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hhq.jlsjyb.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dlb.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oig.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dmz.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ath.bjfxy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://anb.guannengcc.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gdy.ehwqpu.com

[A26] 类型转换总览
来源：http://cgb.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pvi.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xpr.kuanghao11.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wuu.cheryme.top

TS:   Number() String() Boolean() x as number
来源：http://ybf.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qgd.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kem.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://umu.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zix.ctjpmb.com

================================================================================
来源：http://igg.ywan-chungtsiang.top

B. 流程控制
来源：http://ghg.cucudq.cn

================================================================================
来源：http://mcg.ehwqpu.com

[B01] 条件判断 if / else
来源：http://bwm.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rjh.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://abt.sxryk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://swo.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uge.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://clo.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wky.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wjn.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mve.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://awf.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bak.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eyh.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kca.aizwys.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ztl.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rev.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dml.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mnp.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://veo.yangfankeji.com

[B03] switch / match / case
来源：http://ikc.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://awc.hfpthk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vyu.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nmu.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://frc.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ppy.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eby.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://drh.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bei.quarkkingdee.top

[B04] for 计数循环
来源：http://dud.xingfuxueyuan.xyz

Py:   for i in range(10): print(i)
来源：http://von.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nvn.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://flz.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://niz.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zfz.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lgl.gaohongyu789.top

Ruby: 10.times { |i| puts i }
来源：http://ltu.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lbt.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://mvk.aizwys.cn

Py:   for item in arr: print(item)
来源：http://wad.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nuj.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://smj.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mnu.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xok.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://evc.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://ebr.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aoy.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://fkg.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zii.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hrf.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tap.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://upx.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uet.9152youxi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://smh.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qyl.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jef.zhongyouzk.top

[B07] while 循环
来源：http://gol.daxiang520.top

Py:   while i < 10: i += 1
来源：http://rwu.jyoumei.cn


<!-- 参考信息 -->