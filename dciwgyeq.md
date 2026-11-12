代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://lon.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bus.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jqb.fehbvm.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wmc.hnxiangtu.top

================================================================================
来源：http://gao.jinqigufen.top

A. 基础语法与类型
来源：http://zuk.sufxvd.cn

================================================================================
来源：http://ynn.shzxlz.cn

[A01] Hello World
来源：http://ayn.nanxinkj.top

Py:   print("Hello, World!")
来源：http://smj.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://uml.cashguo.top

JS:   console.log("Hello, World!");
来源：http://yes.tian-w.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lhg.c1oappe.top

Java: System.out.println("Hello, World!");
来源：http://xjy.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://cld.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://foq.jlsjyb.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zqw.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://hlt.chenjidiqi.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tds.fanxiaobao.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://vqr.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fkj.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pub.sysykeji.top

Java: String name = "Alex"; int age = 20;
来源：http://eez.hesvh.cn

Go:   name := "Alex"; age := 20
来源：http://vkk.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://wbb.sysykeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://orb.jqgfzy.top

[A03] 常量定义
来源：http://plh.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yjr.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://orj.yuxming.cn

JS:   const PI = 3.14159;
来源：http://wzu.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://mtw.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://wdf.yj20258888.top

Go:   const PI = 3.14159
来源：http://tgy.yueranfly.top

Ruby: PI = 3.14159
来源：http://jje.yangfankeji.com

C#:   const double PI = 3.14159;
来源：http://ixm.wangshuangyany.cn

[A04] 判断变量类型
来源：http://mys.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://uvh.xuetiantiany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zej.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uaw.hesvh.cn

TS:   typeof x; x instanceof Date
来源：http://vul.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ify.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://aur.hammf.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jxz.dianchejie.cn

C#:   x.GetType().Name; x is int
来源：http://xrb.birdmap.top

[A05] 整数除法与取模
来源：http://ycr.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nty.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ils.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ylt.yj20258888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hee.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://bvd.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://wgz.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://wmw.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://pmy.zhijiandao.cn

[A06] 字符串转数字
来源：http://jfo.yfazqb.com

Py:   int("42"); float("3.14")
来源：http://ivd.epnwcf.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qjy.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bwo.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://tzh.hammf.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fql.snrcjt.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://orp.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://hzc.hnqzz.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://snz.snrcjt.cn

[A07] 数字转字符串
来源：http://mwi.shanyushiyangkeji.top

Py:   str(42)
来源：http://muw.andypj.xyz

PHP:  (string) 42; strval(42)
来源：http://rnz.chenjidiqi.icu

JS:   String(42); (42).toString()
来源：http://vxs.ppjwa.cn

TS:   String(42)
来源：http://nnx.ctjpmb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://lum.0kj1m.cn

Go:   strconv.Itoa(42)
来源：http://zli.fengsongda.top

Ruby: 42.to_s
来源：http://cbi.daxiang520.top

C#:   42.ToString()
来源：http://lzl.yangfankeji.com

[A08] 取整与四舍五入
来源：http://ynl.c1oappe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rga.nanxuanxn.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kyx.gaohongyu789.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://itr.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jsd.hcnkem.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yys.jqgufenzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yux.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bsc.yanxiufei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bsb.yvedp.cn

[A09] 绝对值与最大最小值
来源：http://gtu.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tyq.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dqj.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gzi.chenlongwang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://clk.bbcook.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hsu.yongpay.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jks.aizwys.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mqo.shanyushiyangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ekn.zhiwuduotai.top

[A10] 生成随机数
来源：http://wjz.chenzaomai.com

Py:   import random; random.randint(1, 100)
来源：http://qvp.feifeiyinyue.top

PHP:  random_int(1, 100);
来源：http://ljc.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fmg.jinqigufen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bgd.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://vqi.sweek.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://syu.uphjek.com

Ruby: rand(1..100)
来源：http://xjd.guowangkeji.top

C#:   new Random().Next(1, 101)
来源：http://nzl.fzhhl.top

[A11] 条件表达式（三元）
来源：http://ghi.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://qab.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ykv.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://ika.andypj.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://eue.yuanzhike.top

Java: x > 0 ? "yes" : "no"
来源：http://qim.yj20258888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://par.xylfe.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hia.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://vse.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://ugd.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://unj.aizwys.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://afo.svipenyu.cn

JS:   `Hello, ${name}!`
来源：http://eys.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://tky.yfazqb.com

Java: "Hello, %s!".formatted(name)
来源：http://beh.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mjt.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://cap.kuanghao11.cn

C#:   $"Hello, {name}!"
来源：http://czh.hnxiangtu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yci.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://vrt.nanxuanxn.top

PHP:  "第一行\n第二行"
来源：http://zop.cashguo.top

JS:   "第一行\n第二行"
来源：http://qwa.sxryk.cn

TS:   "第一行\n第二行"
来源：http://iop.yj202588.top

Java: "第一行\n第二行"
来源：http://zhv.gotoacloud.top

Go:   "第一行\n第二行"
来源：http://iyr.cheryme.top

Ruby: "第一行\n第二行"
来源：http://wdr.yvedp.cn

C#:   "第一行\n第二行"
来源：http://deo.cheryme.top

[A14] 注释写法
来源：http://yro.sxryk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://teo.cashguo.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dpm.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://aix.xziqi.cn

TS:   // 单行；/* 多行 */
来源：http://hjl.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rpb.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://eai.svipenyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pts.52xcode.cn

C#:   // 单行；/* 多行 */
来源：http://oiw.yfazqb.com

[A15] 空值判断与默认值
来源：http://puo.yuxming.cn

Py:   value = data or "默认值"
来源：http://fsm.haohaochexian.top

PHP:  $value = $data ?? "默认值";
来源：http://cep.tian-w.cn

JS:   const value = data ?? "默认值";
来源：http://icg.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://eyl.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://atu.xziqi.cn

Go:   if data == "" { data = "默认值" }
来源：http://afz.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://nkw.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://dve.cashguo.top

[A16] 真假值判断规则
来源：http://ffx.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nlx.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rfi.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hwk.cucudq.cn

TS:   if (!x) {}
来源：http://spu.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://soh.ivvv.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://osj.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://oeh.tarul.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aja.52xcode.cn

[A17] 位运算
来源：http://cys.sysykeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ztb.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vvt.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ewg.snrcjt.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://low.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giv.nanxinkj.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hcj.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyg.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://odj.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://gyw.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://xnx.guowangkeji.top

PHP:  ord("A"); chr(65)
来源：http://dwm.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gbi.haohaochexian.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zrp.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://vfh.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://soc.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://lkf.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://zfs.hnxiangtu.top

[A19] 交换两个变量
来源：http://jib.haohaochexian.top

Py:   a, b = b, a
来源：http://hgk.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://fnx.zhoulong.xyz

JS:   [a, b] = [b, a];
来源：http://ygn.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://fsd.guannengcc.top

Java: int t = a; a = b; b = t;
来源：http://kbe.hnxiangtu.top

Go:   a, b = b, a
来源：http://lxa.andypj.xyz

Ruby: a, b = b, a
来源：http://hso.zhoulong.xyz

C#:   (a, b) = (b, a);
来源：http://dwc.mhx1999.top

[A20] 读取标准输入
来源：http://zdw.jinghuilouyu.cn

Py:   name = input("请输入：")
来源：http://qvk.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ybb.snrcjt.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wzn.hnqzz.top

TS:   // Node.js：readline 模块
来源：http://nsg.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://ynr.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eux.xuetiantiany.cn

Ruby: gets.chomp
来源：http://glk.yongpay.top

C#:   Console.ReadLine();
来源：http://ubw.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://soe.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://xfo.aibaodan.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fxo.pycfn.com

JS:   (3.14159).toFixed(2)
来源：http://zzl.fehbvm.com

TS:   (3.14159).toFixed(2)
来源：http://fsy.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://fge.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pvd.meibo888.top

Ruby: format("%.2f", 3.14159)
来源：http://lcv.hnxiangtu.top

C#:   3.14159.ToString("F2")
来源：http://ser.yuxming.cn

[A22] 获取字符串长度
来源：http://kwy.sufxvd.cn

Py:   len(s)
来源：http://jwt.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gzd.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aqh.yj20258.top

TS:   s.length
来源：http://ujy.tarul.cn

Java: s.length()
来源：http://iqf.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nqf.fanxiaobao.xyz

Ruby: s.length
来源：http://wrm.fehbvm.com

C#:   s.Length
来源：http://ftk.gzhubu.top

[A23] 大小写转换
来源：http://sjy.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fye.meibo888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bjd.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://whi.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://owv.tian-w.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oqk.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tzx.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://thk.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qbv.zdbjq.cn

[A24] 去除首尾空白
来源：http://mjd.xingfuxueyuan.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hac.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wie.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ktl.gogol.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tni.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kvs.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://szb.epnwcf.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mvw.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qth.sysykeji.top

[A25] 字符串比较
来源：http://xpj.feifeiyinyue.top

Py:   s1 == s2; s1 != s2
来源：http://wyy.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ilb.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xld.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vss.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eqb.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bef.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://rvw.iojbl.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wkx.hnqzz.top

[A26] 类型转换总览
来源：http://qnk.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ybc.sweek.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mqy.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xcl.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://nes.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bib.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wck.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ipp.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vka.9152youxi.cn

================================================================================
来源：http://shv.tian-w.cn

B. 流程控制
来源：http://sbb.fzhhl.top

================================================================================
来源：http://wpp.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://tby.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://etd.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wev.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pvj.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://prh.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://iml.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wfm.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oyn.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ocp.sysykeji.top

[B02] 多分支 else if / elif
来源：http://avi.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gov.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uhs.ehwqpu.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qkq.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klx.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uxd.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pnz.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ezu.yonumen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzg.fzhhl.top

[B03] switch / match / case
来源：http://mhl.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rvy.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ptw.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wxt.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://whd.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aca.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lmk.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xwx.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nln.vehdjk.com

[B04] for 计数循环
来源：http://krc.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://vzm.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lbc.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://plh.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://txn.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zxs.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jwn.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://kob.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xml.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://wrc.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://akv.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://idz.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://qrb.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zbk.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nsg.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ube.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://wzp.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ugz.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://tib.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sxw.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xkd.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://idr.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ldx.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kuj.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hge.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bpx.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epc.daxiang520.top

[B07] while 循环
来源：http://trz.yj20258888.top

Py:   while i < 10: i += 1
来源：http://yeo.jinghuilouyu.cn


<!-- 参考信息 -->