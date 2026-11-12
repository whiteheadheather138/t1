代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://nxi.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pnh.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tnk.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iqu.shanyushiyangtech.top

================================================================================
来源：http://jlj.yfazqb.com

A. 基础语法与类型
来源：http://tyq.shuidangran.top

================================================================================
来源：http://ibv.shanyushiyangtech.top

[A01] Hello World
来源：http://aks.jlsjyb.cn

Py:   print("Hello, World!")
来源：http://jrq.sweek.top

PHP:  echo "Hello, World!";
来源：http://rko.chenzaomai.com

JS:   console.log("Hello, World!");
来源：http://bda.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wvn.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://mkt.dianchejie.cn

Go:   fmt.Println("Hello, World!")
来源：http://mbe.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://llf.chenzaomai.com

C#:   Console.WriteLine("Hello, World!");
来源：http://dax.pengpengdd.cyou

[A02] 变量声明与赋值
来源：http://ann.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vfc.hywenlv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uwr.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://agh.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://edc.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://sqs.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://pqp.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://ufc.ywan-chungtsiang.top

C#:   string name = "Alex"; int age = 20;
来源：http://fwx.hcnkem.com

[A03] 常量定义
来源：http://abm.sysykeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mey.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://fap.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://ven.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://hwa.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://ogd.bjfxy.top

Go:   const PI = 3.14159
来源：http://cgr.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://fou.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://tha.52xcode.cn

[A04] 判断变量类型
来源：http://ucj.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lee.ydzc1.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sgc.shangyingyoupin.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zwk.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://kgq.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bjm.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://mii.mhx1999.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kqd.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://lcg.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://sgb.hfpthk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rkz.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://twv.zhijiandao.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://koi.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://svx.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://rps.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://mfx.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://imj.tian-w.cn

C#:   7 / 2; 7 % 2
来源：http://pte.sweek.top

[A06] 字符串转数字
来源：http://kzr.tanke756.top

Py:   int("42"); float("3.14")
来源：http://xdx.yonumen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://isi.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mqt.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://bce.yfazqb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cjj.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://juk.jqgfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gbm.dianchejie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bli.chenjidiqi.icu

[A07] 数字转字符串
来源：http://reb.bbcook.cn

Py:   str(42)
来源：http://bgy.daxiang520.top

PHP:  (string) 42; strval(42)
来源：http://vks.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://qwr.havefunace.top

TS:   String(42)
来源：http://wsr.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vhm.xziqi.cn

Go:   strconv.Itoa(42)
来源：http://ojx.snrcjt.cn

Ruby: 42.to_s
来源：http://uqu.yuxming.cn

C#:   42.ToString()
来源：http://rit.daxiang520.top

[A08] 取整与四舍五入
来源：http://kfy.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lrg.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wtv.shzxlz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aox.guannengcc.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ywx.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ksj.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gaz.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lag.zhijiandao.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iwe.cdnleiting.top

[A09] 绝对值与最大最小值
来源：http://ldc.0kj1m.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wcr.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yxg.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qff.guannengcc.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mxf.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zbf.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pgv.hcnkem.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cfg.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dde.sysykeji.top

[A10] 生成随机数
来源：http://qjg.smart0.xyz

Py:   import random; random.randint(1, 100)
来源：http://zkb.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://ppj.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fbi.xziqi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bhu.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://xkm.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gmf.uphjek.com

Ruby: rand(1..100)
来源：http://jpn.sweek.top

C#:   new Random().Next(1, 101)
来源：http://lhv.yj202588.top

[A11] 条件表达式（三元）
来源：http://izq.hfpthk.cn

Py:   "yes" if x > 0 else "no"
来源：http://zmf.bbcook.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jat.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://pvy.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://agm.jqgfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://ede.aizwys.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jaj.gogol.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yzv.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://mii.yongpay.top

[A12] 字符串插值 / 格式化
来源：http://pdf.ydjk.org.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wnv.guannengcc.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wup.feifeiyinyue.top

JS:   `Hello, ${name}!`
来源：http://uhp.nanxinkj.top

TS:   `Hello, ${name}!`
来源：http://wtd.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://ctr.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cwh.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://rzf.0kj1m.cn

C#:   $"Hello, {name}!"
来源：http://jub.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fbx.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://pyz.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://rlz.yueranfly.top

JS:   "第一行\n第二行"
来源：http://nsl.ctjpmb.com

TS:   "第一行\n第二行"
来源：http://yfr.zhongyouzk.top

Java: "第一行\n第二行"
来源：http://cti.yuxming.cn

Go:   "第一行\n第二行"
来源：http://qah.jyoumei.cn

Ruby: "第一行\n第二行"
来源：http://mkl.jqgfzy.top

C#:   "第一行\n第二行"
来源：http://tqx.tian-w.cn

[A14] 注释写法
来源：http://cvn.redwolf501.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xjs.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mbb.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://yps.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://rgf.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://idg.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://cpt.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uaa.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://wrx.jinghuilouyu.cn

[A15] 空值判断与默认值
来源：http://upv.xuanzx.com

Py:   value = data or "默认值"
来源：http://dqu.yj20258888.top

PHP:  $value = $data ?? "默认值";
来源：http://cvt.pycfn.com

JS:   const value = data ?? "默认值";
来源：http://qhk.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://xbl.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jwc.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://lkx.shuidangran.top

Ruby: value = data || "默认值"
来源：http://zbq.sysykeji.top

C#:   var value = data ?? "默认值";
来源：http://bys.wangdashe.top

[A16] 真假值判断规则
来源：http://msf.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ipy.guannengcc.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://umo.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dfx.feifeiyinyue.top

TS:   if (!x) {}
来源：http://fev.nwbrower.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lto.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bjq.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://vwt.nanxinkj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rkr.hesvh.cn

[A17] 位运算
来源：http://mwc.nwbrower.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqb.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rkm.birdmap.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phi.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ucx.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rjz.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lwn.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://khz.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ajz.xinyue.icu

[A18] 字符与 ASCII 码互转
来源：http://huw.jinyuanbaomall.cn

Py:   ord("A"); chr(65)
来源：http://gmp.gaohongyu789.top

PHP:  ord("A"); chr(65)
来源：http://amo.sysykeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://avm.ctjpmb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ltd.yj20258.top

Java: (int) 'A'; (char) 65
来源：http://lgq.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pkh.ivvv.top

Ruby: "A".ord; 65.chr
来源：http://boq.dashuyun.cn

C#:   (int)'A'; (char)65
来源：http://fbf.fktsv.cn

[A19] 交换两个变量
来源：http://bxg.yj20258888.top

Py:   a, b = b, a
来源：http://yae.yuanzhike.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kut.pengpengdd.cyou

JS:   [a, b] = [b, a];
来源：http://sqi.guannengcc.top

TS:   [a, b] = [b, a];
来源：http://jvu.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://fwn.gotoacloud.top

Go:   a, b = b, a
来源：http://bap.shangyingyoupin.top

Ruby: a, b = b, a
来源：http://lwy.cashguo.top

C#:   (a, b) = (b, a);
来源：http://zsh.ydzc1.top

[A20] 读取标准输入
来源：http://msk.daria6918.cn

Py:   name = input("请输入：")
来源：http://iir.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nrk.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nnk.tanke756.top

TS:   // Node.js：readline 模块
来源：http://ydd.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://wgm.hysaishi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://poi.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://vlx.zycfv.cn

C#:   Console.ReadLine();
来源：http://gje.cucudq.cn

[A21] 保留指定小数位输出
来源：http://iwb.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://pfb.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fsr.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://laf.zhijiandao.cn

TS:   (3.14159).toFixed(2)
来源：http://pfo.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://qxa.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wyw.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://mfz.uphjek.com

C#:   3.14159.ToString("F2")
来源：http://lwu.gotoacloud.top

[A22] 获取字符串长度
来源：http://ekb.hfpthk.cn

Py:   len(s)
来源：http://ggz.gaohongyu789.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dmp.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hsd.xuanzx.com

TS:   s.length
来源：http://bsb.pycfn.com

Java: s.length()
来源：http://ywd.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bwh.fktsv.cn

Ruby: s.length
来源：http://yeg.hfpthk.cn

C#:   s.Length
来源：http://dpv.dianchejie.cn

[A23] 大小写转换
来源：http://vsi.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cry.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jdd.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dey.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lzf.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qwf.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cab.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zfd.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://gzb.smart0.xyz

[A24] 去除首尾空白
来源：http://yzi.daria6918.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lkz.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gpi.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jqr.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cgg.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yvi.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://brz.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ley.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hgm.fzhhl.top

[A25] 字符串比较
来源：http://lus.yuxming.cn

Py:   s1 == s2; s1 != s2
来源：http://abu.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://elz.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jpj.zdqjudy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dnf.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vpn.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ixj.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jyw.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kuh.hesvh.cn

[A26] 类型转换总览
来源：http://nrf.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cwr.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sud.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hgv.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://cta.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wcg.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wvp.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bwk.zhongyouzk.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dpk.yangfankeji.com

================================================================================
来源：http://kze.yuanzhike.top

B. 流程控制
来源：http://tjx.shanyushiyangtech.top

================================================================================
来源：http://sdt.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://qtw.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://afo.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jlk.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://edp.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dtm.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://qmf.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jre.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lgs.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qpg.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://ypt.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gvk.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uma.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cvu.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzi.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvk.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cxn.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hbh.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnl.aibaodan.cn

[B03] switch / match / case
来源：http://mpy.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://teb.jinyuanbaomall.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kib.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ynh.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vwh.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tll.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ibo.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tpj.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://esd.zdqjudy.top

[B04] for 计数循环
来源：http://pkv.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://ixq.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pxz.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rnr.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zbu.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xtw.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bon.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://wpo.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xzr.yj20258.top

[B05] 遍历数组 / 列表
来源：http://xux.yongpay.top

Py:   for item in arr: print(item)
来源：http://ugx.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lcf.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://ntn.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pwr.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nri.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hxm.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://bhx.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dfq.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://bjv.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gsn.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zoo.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lgd.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dvs.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hgz.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vqo.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ezx.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rpy.ydjk.org.cn

[B07] while 循环
来源：http://ffa.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://rcx.jinghuilouyu.cn


<!-- 参考信息 -->