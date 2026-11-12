代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://keh.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oka.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wak.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://muk.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dpz.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vvx.jinyuanbaomall.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tgz.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hqe.bbcook.cn

================================================================================
来源：http://irf.nwbrower.top

A. 基础语法与类型
来源：http://rkl.gzhubu.top

================================================================================
来源：http://vlq.zhengqikj.top

[A01] Hello World
来源：http://zfr.xylfe.cn

Py:   print("Hello, World!")
来源：http://cxm.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://btb.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://xul.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jqv.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://zfc.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://wjc.sweek.top

Ruby: puts "Hello, World!"
来源：http://byc.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qkh.gogol.net.cn

[A02] 变量声明与赋值
来源：http://oem.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nzj.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bln.jqgufenzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://bcn.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://axm.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://snj.yongpay.top

Go:   name := "Alex"; age := 20
来源：http://qru.ybcxt.top

Ruby: name = "Alex"; age = 20
来源：http://lvz.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://oef.zhaomingkeji.xyz

[A03] 常量定义
来源：http://pij.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bkh.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://qjn.daria6918.cn

JS:   const PI = 3.14159;
来源：http://pun.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://cyu.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://erc.uphjek.com

Go:   const PI = 3.14159
来源：http://vqq.gogol.net.cn

Ruby: PI = 3.14159
来源：http://yvq.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://qny.chenlongwang.top

[A04] 判断变量类型
来源：http://gar.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dbz.hysaishi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dgu.smart0.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ull.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://sli.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://opg.gotoacloud.top

Go:   reflect.TypeOf(x).Name()
来源：http://umi.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gfq.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://yux.hesvh.cn

[A05] 整数除法与取模
来源：http://xrv.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://can.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bde.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iaq.316326.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://djx.fzhhl.top

Java: 7 / 2; 7 % 2
来源：http://agm.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://hde.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ycb.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://wsd.yuanzhike.top

[A06] 字符串转数字
来源：http://qov.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://gth.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jdd.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qfe.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://oxz.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://okm.jiagoushi.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://onm.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://txu.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lna.meibo888.top

[A07] 数字转字符串
来源：http://bpp.wangshuangyany.cn

Py:   str(42)
来源：http://dvw.cdnleiting.top

PHP:  (string) 42; strval(42)
来源：http://zqv.fehbvm.com

JS:   String(42); (42).toString()
来源：http://hor.yueranfly.top

TS:   String(42)
来源：http://thq.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uei.guannengcc.top

Go:   strconv.Itoa(42)
来源：http://jox.yangfankeji.com

Ruby: 42.to_s
来源：http://grr.hywenlv.cn

C#:   42.ToString()
来源：http://gzn.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://zwe.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vhq.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fut.ybcxt.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pdf.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xeu.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tos.jqgufenzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hiw.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nae.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lzy.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://via.jinqigufen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nhl.wangdashe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://arp.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ruh.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xqr.snrcjt.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gym.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ofe.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://urp.fanxiaobao.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hap.0kj1m.cn

[A10] 生成随机数
来源：http://ehz.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://car.mhx1999.top

PHP:  random_int(1, 100);
来源：http://lbm.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jel.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ikb.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://qmm.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bga.snrcjt.cn

Ruby: rand(1..100)
来源：http://ifu.sjlbkw.cn

C#:   new Random().Next(1, 101)
来源：http://fis.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://orr.yongpay.top

Py:   "yes" if x > 0 else "no"
来源：http://xrm.yangfankeji.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ezf.vehdjk.com

JS:   x > 0 ? "yes" : "no"
来源：http://qba.cheryme.top

TS:   x > 0 ? "yes" : "no"
来源：http://hdn.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://hte.wangshuangyany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xsd.epnwcf.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ecs.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://mwx.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://fzq.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hqs.yongpay.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wkb.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://xsb.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://lna.zhijiandao.cn

Java: "Hello, %s!".formatted(name)
来源：http://srt.sufxvd.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fwv.dashuyun.cn

Ruby: "Hello, #{name}!"
来源：http://jwm.vehdjk.com

C#:   $"Hello, {name}!"
来源：http://cdv.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lep.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://nas.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://uvl.bjfxy.top

JS:   "第一行\n第二行"
来源：http://zmh.ydjk.org.cn

TS:   "第一行\n第二行"
来源：http://prh.ybcxt.top

Java: "第一行\n第二行"
来源：http://vfv.xuetiantiany.cn

Go:   "第一行\n第二行"
来源：http://ugc.yfazqb.com

Ruby: "第一行\n第二行"
来源：http://ova.xuanzx.com

C#:   "第一行\n第二行"
来源：http://abc.hnqzz.top

[A14] 注释写法
来源：http://kem.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mxv.ehwqpu.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://sgh.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://hro.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://lrp.cheryme.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zfx.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://tyb.cdnleiting.top

Ruby: # 单行；=begin 多行 =end
来源：http://xsa.jiagoushi.top

C#:   // 单行；/* 多行 */
来源：http://mjl.yuanzhike.top

[A15] 空值判断与默认值
来源：http://zse.daxiang520.top

Py:   value = data or "默认值"
来源：http://nun.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://kgw.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://onx.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://cqf.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pqh.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://fmm.cucudq.cn

Ruby: value = data || "默认值"
来源：http://wto.xylfe.cn

C#:   var value = data ?? "默认值";
来源：http://msh.cucudq.cn

[A16] 真假值判断规则
来源：http://sqk.hammf.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://evw.snrcjt.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jge.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iea.jiagoushi.top

TS:   if (!x) {}
来源：http://ybx.sufxvd.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hsr.sjlbkw.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://byr.pycfn.com

Ruby: unless x            # nil 与 false 为假
来源：http://bhk.sxryk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vmq.sweek.top

[A17] 位运算
来源：http://mhn.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ghh.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nfu.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://urq.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pvx.ctjpmb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyp.yj20258888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://seb.uphjek.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tud.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyk.zdqjudy.top

[A18] 字符与 ASCII 码互转
来源：http://wkz.tianlin.xyz

Py:   ord("A"); chr(65)
来源：http://lfj.kuanghao11.cn

PHP:  ord("A"); chr(65)
来源：http://vnr.nwbrower.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://egd.daria6918.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uxx.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://gqq.guowangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bzy.snrcjt.cn

Ruby: "A".ord; 65.chr
来源：http://hkd.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://pam.ehwqpu.com

[A19] 交换两个变量
来源：http://adm.shanyushiyangtech.top

Py:   a, b = b, a
来源：http://ygk.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://idw.shuidangran.top

JS:   [a, b] = [b, a];
来源：http://akx.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://okq.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://xyr.cdnleiting.top

Go:   a, b = b, a
来源：http://pxe.guannengcc.top

Ruby: a, b = b, a
来源：http://zde.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://nzh.hysaishi.cn

[A20] 读取标准输入
来源：http://mvm.zycfv.cn

Py:   name = input("请输入：")
来源：http://baa.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vha.gzhubu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dzm.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://gps.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://yae.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yas.nanxinkj.top

Ruby: gets.chomp
来源：http://bik.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://psl.guannengcc.top

[A21] 保留指定小数位输出
来源：http://ibe.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://zsd.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wed.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://ehz.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://ncm.yangfankeji.com

Java: String.format("%.2f", 3.14159)
来源：http://mzb.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://efx.guannengcc.top

Ruby: format("%.2f", 3.14159)
来源：http://wjq.52xcode.cn

C#:   3.14159.ToString("F2")
来源：http://kew.vehdjk.com

[A22] 获取字符串长度
来源：http://png.zdqjudy.top

Py:   len(s)
来源：http://wyg.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rkl.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://emr.0kj1m.cn

TS:   s.length
来源：http://dbf.shangyingyoupin.top

Java: s.length()
来源：http://ycf.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://poz.xziqi.cn

Ruby: s.length
来源：http://ghx.havefunace.top

C#:   s.Length
来源：http://oma.hfpthk.cn

[A23] 大小写转换
来源：http://xjz.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tqy.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wac.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ybx.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zky.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dfs.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oyi.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://smp.52xcode.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sfz.yongpay.top

[A24] 去除首尾空白
来源：http://jih.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baa.zdbjq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lhj.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wmu.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jdi.jyoumei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ulr.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://vny.daria6918.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xdf.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xuu.cashguo.top

[A25] 字符串比较
来源：http://ygx.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://slb.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ggl.sweek.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nge.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qan.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://egp.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kim.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://wfb.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://twg.fengsongda.top

[A26] 类型转换总览
来源：http://nlt.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iuv.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://viq.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ism.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://ycz.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mzg.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://met.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zch.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://voz.vehdjk.com

================================================================================
来源：http://eii.wangdashe.top

B. 流程控制
来源：http://gfd.yj20258.top

================================================================================
来源：http://cpz.jinqigufen.top

[B01] 条件判断 if / else
来源：http://cjj.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xlz.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://onw.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mjc.yueranfly.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://urx.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qqi.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kkm.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tbb.cheryme.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://njx.redwolf501.top

[B02] 多分支 else if / elif
来源：http://alm.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xxn.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kze.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://igi.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zto.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bed.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ixv.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rtp.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://akb.ivvv.top

[B03] switch / match / case
来源：http://kqv.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lbe.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ssa.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://smk.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yum.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fuu.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zvl.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vhs.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://orq.snrcjt.cn

[B04] for 计数循环
来源：http://lit.guannengcc.top

Py:   for i in range(10): print(i)
来源：http://hds.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fvn.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vxz.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zpz.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yyw.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kda.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://xpl.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ceg.yj202588.top

[B05] 遍历数组 / 列表
来源：http://lcz.uphjek.com

Py:   for item in arr: print(item)
来源：http://fvh.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dwv.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ncp.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qhq.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sfn.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mcs.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://ghy.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ocz.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://eci.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://egr.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://whu.yanxiufei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vyz.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bak.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pmc.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pkn.feifeiyinyue.top


<!-- 参考信息 -->