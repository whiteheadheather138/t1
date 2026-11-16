代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://kmo.c1oappe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cht.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xen.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lsf.zhixingplan.top

================================================================================
来源：http://xae.daria6918.cn

A. 基础语法与类型
来源：http://xrr.yangfankeji.com

================================================================================
来源：http://sze.sysykeji.top

[A01] Hello World
来源：http://vsm.birdmap.top

Py:   print("Hello, World!")
来源：http://qne.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://rby.c1oappe.top

JS:   console.log("Hello, World!");
来源：http://nmm.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rbg.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://szn.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://ixo.fehbvm.com

Ruby: puts "Hello, World!"
来源：http://vrx.jinyuanbaomall.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bnm.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://zyb.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://voc.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gsv.yanxiufei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ben.andypj.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nin.sysykeji.top

Java: String name = "Alex"; int age = 20;
来源：http://dyv.cheryme.top

Go:   name := "Alex"; age := 20
来源：http://kat.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://kbm.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://qge.tianlin.xyz

[A03] 常量定义
来源：http://wec.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tit.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://hqm.sxryk.cn

JS:   const PI = 3.14159;
来源：http://ixx.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://twn.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://xnq.c1oappe.top

Go:   const PI = 3.14159
来源：http://aui.yj20258.top

Ruby: PI = 3.14159
来源：http://ylz.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://gag.andypj.xyz

[A04] 判断变量类型
来源：http://rte.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cbz.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://skw.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://axu.yangfankeji.com

TS:   typeof x; x instanceof Date
来源：http://buk.xuetiantiany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vqk.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://imz.cdnleiting.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bjr.xylfe.cn

C#:   x.GetType().Name; x is int
来源：http://qrw.jyoumei.cn

[A05] 整数除法与取模
来源：http://zdi.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fwc.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xvy.dashuyun.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dlu.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://adn.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://yjt.pengpengdd.cyou

Go:   7 / 2; 7 % 2
来源：http://ldj.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://gsi.nanxinkj.top

C#:   7 / 2; 7 % 2
来源：http://yxa.jinyuanbaomall.cn

[A06] 字符串转数字
来源：http://fmu.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://hlz.epnwcf.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wfa.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://inm.guowangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://sqy.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vud.pycfn.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nhj.gzhubu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hjt.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wfx.jinqigfzy.top

[A07] 数字转字符串
来源：http://vzt.dashuyun.cn

Py:   str(42)
来源：http://usp.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://pvz.ivvv.top

JS:   String(42); (42).toString()
来源：http://rwf.wangdashe.top

TS:   String(42)
来源：http://gia.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rji.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://iyf.cucudq.cn

Ruby: 42.to_s
来源：http://uda.hongshengwenyu.top

C#:   42.ToString()
来源：http://pww.sjlbkw.cn

[A08] 取整与四舍五入
来源：http://rnw.zhixingplan.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://man.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jeu.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yrw.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zpt.zhengqikj.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bkj.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kst.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qcb.dianchejie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nqu.yj202588.top

[A09] 绝对值与最大最小值
来源：http://ter.ydjk.org.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nkn.cdnleiting.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://diz.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://deo.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kjk.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rqy.aibaodan.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://irb.c1oappe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mgp.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://acl.andypj.xyz

[A10] 生成随机数
来源：http://rrk.jqgufenzy.top

Py:   import random; random.randint(1, 100)
来源：http://hvm.cashguo.top

PHP:  random_int(1, 100);
来源：http://gti.gotoacloud.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eba.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bsn.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://ary.ywan-chungtsiang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mik.cdnleiting.top

Ruby: rand(1..100)
来源：http://skh.sysykeji.top

C#:   new Random().Next(1, 101)
来源：http://thl.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://woy.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://rav.zhiwuduotai.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vrx.iojbl.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oxa.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://beo.svipenyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://rxl.shangyingyoupin.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gol.ivvv.top

Ruby: x > 0 ? "yes" : "no"
来源：http://chz.zhongyouzk.top

C#:   x > 0 ? "yes" : "no"
来源：http://lkg.sysykeji.top

[A12] 字符串插值 / 格式化
来源：http://rdq.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rcf.mhx1999.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ffo.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://osx.gaohongyu789.top

TS:   `Hello, ${name}!`
来源：http://isq.bbcook.cn

Java: "Hello, %s!".formatted(name)
来源：http://azy.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vxq.tian-w.cn

Ruby: "Hello, #{name}!"
来源：http://vrb.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://nae.sufxvd.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xvw.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://xou.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://hrm.tian-w.cn

JS:   "第一行\n第二行"
来源：http://gyk.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://wtw.yueranfly.top

Java: "第一行\n第二行"
来源：http://uiw.ctjpmb.com

Go:   "第一行\n第二行"
来源：http://eje.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://xsl.fktsv.cn

C#:   "第一行\n第二行"
来源：http://jcn.hysaishi.cn

[A14] 注释写法
来源：http://tol.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kqr.shanyushiyangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lmy.quarkkingdee.top

JS:   // 单行；/* 多行 */
来源：http://trn.chenlongwang.top

TS:   // 单行；/* 多行 */
来源：http://uxb.gzhubu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ykj.xylfe.cn

Go:   // 单行；/* 多行 */
来源：http://ppi.havefunace.top

Ruby: # 单行；=begin 多行 =end
来源：http://qxw.kuanghao11.cn

C#:   // 单行；/* 多行 */
来源：http://tcu.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://tqb.ctjpmb.com

Py:   value = data or "默认值"
来源：http://rfa.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://etp.zhaomingkeji.xyz

JS:   const value = data ?? "默认值";
来源：http://utu.shuidangran.top

TS:   const value = data ?? "默认值";
来源：http://wio.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dpv.zhaomingkeji.xyz

Go:   if data == "" { data = "默认值" }
来源：http://lrb.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://zlg.316326.xyz

C#:   var value = data ?? "默认值";
来源：http://rxd.fengsongda.top

[A16] 真假值判断规则
来源：http://xsz.zhiwuduotai.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rvb.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wcb.c1oappe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dnr.xylfe.cn

TS:   if (!x) {}
来源：http://sqt.316326.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://und.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mag.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://drg.tanke756.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jyg.52xcode.cn

[A17] 位运算
来源：http://pft.hammf.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fwp.tian-w.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ryi.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dzw.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://seu.daxiang520.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wlb.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zqs.hnxiangtu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vmo.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzs.hfpthk.cn

[A18] 字符与 ASCII 码互转
来源：http://cjx.jianghu66.top

Py:   ord("A"); chr(65)
来源：http://ymd.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://lrv.zhijiandao.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bgp.ctjpmb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lid.gzhubu.top

Java: (int) 'A'; (char) 65
来源：http://hkd.vehdjk.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://luv.jinghuilouyu.cn

Ruby: "A".ord; 65.chr
来源：http://fbr.zycfv.cn

C#:   (int)'A'; (char)65
来源：http://lnv.birdmap.top

[A19] 交换两个变量
来源：http://ybo.nanxinkj.top

Py:   a, b = b, a
来源：http://ftc.jlsjyb.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://may.yueranfly.top

JS:   [a, b] = [b, a];
来源：http://njp.shangyingyoupin.top

TS:   [a, b] = [b, a];
来源：http://fuk.zhongyouzk.top

Java: int t = a; a = b; b = t;
来源：http://una.nanxinkj.top

Go:   a, b = b, a
来源：http://shq.jlsjyb.cn

Ruby: a, b = b, a
来源：http://cir.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://dmq.birdmap.top

[A20] 读取标准输入
来源：http://riv.hysaishi.cn

Py:   name = input("请输入：")
来源：http://zkn.meibo888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kzj.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yme.fehbvm.com

TS:   // Node.js：readline 模块
来源：http://qhx.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://cft.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ntd.fengsongda.top

Ruby: gets.chomp
来源：http://gvz.hesvh.cn

C#:   Console.ReadLine();
来源：http://qpc.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://afg.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://lth.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pkk.zhiwuduotai.top

JS:   (3.14159).toFixed(2)
来源：http://phw.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://plh.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://pgf.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xul.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://ced.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://ccv.quarkkingdee.top

[A22] 获取字符串长度
来源：http://gem.zdqjudy.top

Py:   len(s)
来源：http://ert.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dzd.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://new.tian-w.cn

TS:   s.length
来源：http://qoc.tanke756.top

Java: s.length()
来源：http://ljy.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jiw.bjfxy.top

Ruby: s.length
来源：http://hvp.yj20258.top

C#:   s.Length
来源：http://zic.zhiwuduotai.top

[A23] 大小写转换
来源：http://qts.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mgu.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mkk.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lba.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ngs.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ory.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mpi.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://llf.sufxvd.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uxe.zhengqikj.top

[A24] 去除首尾空白
来源：http://fhz.vqdsnc.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oou.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lqk.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ipt.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ago.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hoe.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://pae.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pxn.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fmx.jinqigufen.top

[A25] 字符串比较
来源：http://xhu.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://jwi.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ckk.xuanzx.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rao.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mql.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://web.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://peo.gotoacloud.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vpq.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cfs.aizwys.cn

[A26] 类型转换总览
来源：http://ofy.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wkw.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://air.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jal.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://wrh.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pnj.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tpb.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iuz.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ofp.hcnkem.com

================================================================================
来源：http://vbj.xinyue.icu

B. 流程控制
来源：http://caw.jqgfzy.top

================================================================================
来源：http://rco.9152youxi.cn

[B01] 条件判断 if / else
来源：http://odu.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://xhq.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zuy.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nbq.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nfa.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://egp.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ygf.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://axb.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://upw.tarul.cn

[B02] 多分支 else if / elif
来源：http://gef.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mfb.birdmap.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cku.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqw.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nfj.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nvg.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kid.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xov.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fll.sufxvd.cn

[B03] switch / match / case
来源：http://kwr.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hop.jqgufenzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://apb.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bwh.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ael.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zdo.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mpz.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bbv.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qcu.fktsv.cn

[B04] for 计数循环
来源：http://lnz.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://pku.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vdm.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ujc.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fzw.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lzj.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pzs.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://aer.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zsx.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://sen.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://tak.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eny.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aia.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://unt.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://got.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ewm.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://nik.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tqp.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://ddk.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ruf.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wny.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhq.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://upx.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://orz.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cyc.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://atx.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nun.mhx1999.top

[B07] while 循环
来源：http://mrh.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://lzj.hywenlv.cn


<!-- 参考信息 -->