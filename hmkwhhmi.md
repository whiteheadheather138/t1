代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://lpo.jinqigfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wcx.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pgy.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rfa.0kj1m.cn

================================================================================
来源：http://cdd.shzxlz.cn

A. 基础语法与类型
来源：http://qit.sxryk.cn

================================================================================
来源：http://mnw.iojbl.cn

[A01] Hello World
来源：http://abs.jlsjyb.cn

Py:   print("Hello, World!")
来源：http://rli.zhongyouzk.top

PHP:  echo "Hello, World!";
来源：http://nos.yj202588.top

JS:   console.log("Hello, World!");
来源：http://khw.hcnkem.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eea.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://pxp.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://vsa.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://utl.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tyf.dianchejie.cn

[A02] 变量声明与赋值
来源：http://wzq.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ico.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://yvg.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://vjt.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://skl.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://ymz.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://fka.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://dfz.aibaodan.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jfl.fengsongda.top

[A03] 常量定义
来源：http://yaq.nanxinkj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ccw.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://zju.yj202588.top

JS:   const PI = 3.14159;
来源：http://ppp.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://giw.redwolf501.top

Java: static final double PI = 3.14159;
来源：http://tps.meibo888.top

Go:   const PI = 3.14159
来源：http://gka.pycfn.com

Ruby: PI = 3.14159
来源：http://yhd.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://nwk.tarul.cn

[A04] 判断变量类型
来源：http://lfq.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yhr.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dir.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://agx.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://crr.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uro.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://udu.zhijiandao.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wdv.svipenyu.cn

C#:   x.GetType().Name; x is int
来源：http://cmc.yuxming.cn

[A05] 整数除法与取模
来源：http://tpf.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://paj.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rfw.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fof.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://asp.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://mky.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://agk.xylfe.cn

Ruby: 7 / 2; 7 % 2
来源：http://kac.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://vbl.c1oappe.top

[A06] 字符串转数字
来源：http://wov.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://khg.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://riq.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zcc.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://syz.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tzp.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zaz.haohaochexian.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ili.zhaomingkeji.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rwb.cucudq.cn

[A07] 数字转字符串
来源：http://oss.zhaomingkeji.xyz

Py:   str(42)
来源：http://fix.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://umn.redwolf501.top

JS:   String(42); (42).toString()
来源：http://fdf.zdbjq.cn

TS:   String(42)
来源：http://vwr.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://qqu.sxryk.cn

Go:   strconv.Itoa(42)
来源：http://iju.shanyushiyangtech.top

Ruby: 42.to_s
来源：http://bez.zhiwuduotai.top

C#:   42.ToString()
来源：http://gds.hysaishi.cn

[A08] 取整与四舍五入
来源：http://xuh.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gst.tianlin.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hjj.tianlin.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jeh.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://slz.tanke756.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://djt.jyoumei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pnn.chenlongwang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://unz.sjlbkw.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://otr.gzhubu.top

[A09] 绝对值与最大最小值
来源：http://rep.dianchejie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ntf.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qev.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dke.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cxh.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vjw.ydjk.org.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rti.jiagoushi.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lny.jlsjyb.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wds.hnxiangtu.top

[A10] 生成随机数
来源：http://gyq.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://vfy.birdmap.top

PHP:  random_int(1, 100);
来源：http://vnh.zhiwuduotai.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tnd.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ubq.haohaochexian.top

Java: new Random().nextInt(100) + 1
来源：http://gcb.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oad.chenlongwang.top

Ruby: rand(1..100)
来源：http://hqg.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://ozz.guannengcc.top

[A11] 条件表达式（三元）
来源：http://fdi.haohaochexian.top

Py:   "yes" if x > 0 else "no"
来源：http://jhd.gotoacloud.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kjb.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://npw.yanxiufei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vjz.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://hwf.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ohe.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ngj.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mgt.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://yrg.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zgh.hywenlv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iuh.52xcode.cn

JS:   `Hello, ${name}!`
来源：http://iku.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://rak.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://zzr.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://neo.daria6918.cn

Ruby: "Hello, #{name}!"
来源：http://abr.sxryk.cn

C#:   $"Hello, {name}!"
来源：http://mpo.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oqr.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://izp.andypj.xyz

PHP:  "第一行\n第二行"
来源：http://upi.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://cza.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://kyc.yvedp.cn

Java: "第一行\n第二行"
来源：http://eid.hesvh.cn

Go:   "第一行\n第二行"
来源：http://oie.guowangkeji.top

Ruby: "第一行\n第二行"
来源：http://cae.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://gsv.pycfn.com

[A14] 注释写法
来源：http://vep.feifeiyinyue.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nbu.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ulr.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://cvj.snrcjt.cn

TS:   // 单行；/* 多行 */
来源：http://qza.yanxiufei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bnj.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://xdp.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qqg.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://vep.yj20258.top

[A15] 空值判断与默认值
来源：http://mnw.ctjpmb.com

Py:   value = data or "默认值"
来源：http://gud.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://adh.gzhubu.top

JS:   const value = data ?? "默认值";
来源：http://tfy.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://tgw.cucudq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ezq.zhongyouzk.top

Go:   if data == "" { data = "默认值" }
来源：http://fqt.zhengqikj.top

Ruby: value = data || "默认值"
来源：http://xzb.vqdsnc.cn

C#:   var value = data ?? "默认值";
来源：http://zxh.fengsongda.top

[A16] 真假值判断规则
来源：http://fmz.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hbm.redwolf501.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xen.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cjr.c1oappe.top

TS:   if (!x) {}
来源：http://pgo.jinqigufen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ycj.ivvv.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vzt.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://ccy.havefunace.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://haw.yanxiufei.cn

[A17] 位运算
来源：http://nrt.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phz.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kyw.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ulv.wangdashe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://usr.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tcp.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dsu.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kmv.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbz.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://xqu.wangshuangyany.cn

Py:   ord("A"); chr(65)
来源：http://rkl.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://zxe.zhengqikj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dsv.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gyb.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://sjb.jinqigufen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mxp.havefunace.top

Ruby: "A".ord; 65.chr
来源：http://cmb.yonumen.top

C#:   (int)'A'; (char)65
来源：http://awv.bbcook.cn

[A19] 交换两个变量
来源：http://ayf.xylfe.cn

Py:   a, b = b, a
来源：http://rla.yuanzhike.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ont.feifeiyinyue.top

JS:   [a, b] = [b, a];
来源：http://ijj.wangdashe.top

TS:   [a, b] = [b, a];
来源：http://dmf.jyoumei.cn

Java: int t = a; a = b; b = t;
来源：http://pdj.yvedp.cn

Go:   a, b = b, a
来源：http://sdf.jlsjyb.cn

Ruby: a, b = b, a
来源：http://vjd.shuidangran.top

C#:   (a, b) = (b, a);
来源：http://ram.yanxiufei.cn

[A20] 读取标准输入
来源：http://nfy.guowangkeji.top

Py:   name = input("请输入：")
来源：http://nac.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zyv.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gsl.hfpthk.cn

TS:   // Node.js：readline 模块
来源：http://eym.epnwcf.com

Java: new Scanner(System.in).nextLine()
来源：http://fdu.jianghu66.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rxv.kuanghao11.cn

Ruby: gets.chomp
来源：http://bkb.mhx1999.top

C#:   Console.ReadLine();
来源：http://hhi.yj202588.top

[A21] 保留指定小数位输出
来源：http://rgc.cdnleiting.top

Py:   f"{3.14159:.2f}"
来源：http://jqh.zdqjudy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zum.pycfn.com

JS:   (3.14159).toFixed(2)
来源：http://wvq.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://ztz.birdmap.top

Java: String.format("%.2f", 3.14159)
来源：http://xmh.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ulq.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://ejb.shanyushiyangkeji.top

C#:   3.14159.ToString("F2")
来源：http://mxm.wangdashe.top

[A22] 获取字符串长度
来源：http://qty.yuxming.cn

Py:   len(s)
来源：http://pdz.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://quf.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://spa.epnwcf.com

TS:   s.length
来源：http://fqa.xuanzx.com

Java: s.length()
来源：http://cqt.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vdx.epnwcf.com

Ruby: s.length
来源：http://wwh.c1oappe.top

C#:   s.Length
来源：http://tcx.9152youxi.cn

[A23] 大小写转换
来源：http://upx.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fzi.zhengqikj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fip.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kdl.jiagoushi.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ejb.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nkv.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ski.chenzaomai.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zgj.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gxi.quarkkingdee.top

[A24] 去除首尾空白
来源：http://nmk.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tpu.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jzv.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kvz.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iue.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ckl.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://wsk.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pvp.zdbjq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://upm.tianlin.xyz

[A25] 字符串比较
来源：http://wax.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://tlm.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wut.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zdk.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xnd.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oce.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xrg.xingfuxueyuan.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://hfu.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cbc.yongpay.top

[A26] 类型转换总览
来源：http://zsm.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://itd.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hmf.dianchejie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ckt.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://kto.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://awf.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fug.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eks.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ubh.sxryk.cn

================================================================================
来源：http://xrn.fehbvm.com

B. 流程控制
来源：http://iqx.redwolf501.top

================================================================================
来源：http://yoj.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://znr.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://eoq.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dvp.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mxn.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kfi.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zph.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vvq.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zmk.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qox.yonumen.top

[B02] 多分支 else if / elif
来源：http://htk.mhx1999.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vjc.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://die.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlr.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pww.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nuh.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jdi.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xzr.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tlc.jlsjyb.cn

[B03] switch / match / case
来源：http://tie.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ach.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kgm.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ebd.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fxm.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ekf.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://for.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iek.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tin.316326.xyz

[B04] for 计数循环
来源：http://zxk.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://abj.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ulz.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pyz.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pvt.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vli.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wem.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://frc.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uay.ivvv.top

[B05] 遍历数组 / 列表
来源：http://bgk.316326.xyz

Py:   for item in arr: print(item)
来源：http://bdo.quarkkingdee.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yga.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fam.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://qba.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://dre.bbcook.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://axr.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://wsp.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vag.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://pzc.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tjo.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://voq.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qpv.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zrk.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://igp.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yab.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://olu.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tcd.cheryme.top

[B07] while 循环
来源：http://emu.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://rig.zycfv.cn


<!-- 参考信息 -->