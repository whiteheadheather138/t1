代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://kmq.hnqzz.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xuo.yj20258.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kji.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://edu.pycfn.com

================================================================================
来源：http://rqq.ybcxt.top

A. 基础语法与类型
来源：http://poc.gzhubu.top

================================================================================
来源：http://vju.yuanzhike.top

[A01] Hello World
来源：http://ntf.hcnkem.com

Py:   print("Hello, World!")
来源：http://nlv.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://flu.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://wsn.ivvv.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xtr.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://pgq.yuxming.cn

Go:   fmt.Println("Hello, World!")
来源：http://wcj.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://yec.jlsjyb.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rtm.hysaishi.cn

[A02] 变量声明与赋值
来源：http://lxz.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eph.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zaz.epnwcf.com

JS:   let name = "Alex"; const age = 20;
来源：http://nwd.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hnq.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://qoo.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://hwl.gotoacloud.top

Ruby: name = "Alex"; age = 20
来源：http://ene.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://ubg.nanxinkj.top

[A03] 常量定义
来源：http://iea.ppjwa.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gww.yuxming.cn

PHP:  const PI = 3.14159;
来源：http://nis.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://sww.xylfe.cn

TS:   const PI: number = 3.14159;
来源：http://kou.daria6918.cn

Java: static final double PI = 3.14159;
来源：http://clr.yanxiufei.cn

Go:   const PI = 3.14159
来源：http://ycb.pengpengdd.cyou

Ruby: PI = 3.14159
来源：http://bgw.sufxvd.cn

C#:   const double PI = 3.14159;
来源：http://irg.tian-w.cn

[A04] 判断变量类型
来源：http://eef.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aik.shanyushiyangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ylf.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lgw.quarkkingdee.top

TS:   typeof x; x instanceof Date
来源：http://gtp.cucudq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ktb.hesvh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yyz.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lcg.svipenyu.cn

C#:   x.GetType().Name; x is int
来源：http://cau.kuanghao11.cn

[A05] 整数除法与取模
来源：http://bek.shangyingyoupin.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mot.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ipo.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nye.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mvy.yuanzhike.top

Java: 7 / 2; 7 % 2
来源：http://gta.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://kdx.smart0.xyz

Ruby: 7 / 2; 7 % 2
来源：http://zmb.sweek.top

C#:   7 / 2; 7 % 2
来源：http://vak.hysaishi.cn

[A06] 字符串转数字
来源：http://qel.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://ptg.haohaochexian.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aeu.gaohongyu789.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xio.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://qkw.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ijo.xinyue.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lvl.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ccb.snrcjt.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tze.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://meq.cqqwz.cn

Py:   str(42)
来源：http://yjq.dashuyun.cn

PHP:  (string) 42; strval(42)
来源：http://efo.meibo888.top

JS:   String(42); (42).toString()
来源：http://qwy.yvedp.cn

TS:   String(42)
来源：http://amy.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bxl.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://lsy.yj20258.top

Ruby: 42.to_s
来源：http://dkf.zdqjudy.top

C#:   42.ToString()
来源：http://ebi.yj20258.top

[A08] 取整与四舍五入
来源：http://nou.kuanghao11.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ewn.nanxinkj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jcf.sufxvd.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ojr.chenjidiqi.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vnx.sysykeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sli.bbcook.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aqh.shanyushiyangtech.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://klw.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xyl.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://yfq.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ond.daxiang520.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://imj.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mcd.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yyd.vehdjk.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xvw.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qtp.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ngw.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ref.fehbvm.com

[A10] 生成随机数
来源：http://bge.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://cav.daxiang520.top

PHP:  random_int(1, 100);
来源：http://ohz.wangshuangyany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://osc.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xmf.daria6918.cn

Java: new Random().nextInt(100) + 1
来源：http://nfj.zhoulong.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cgt.pycfn.com

Ruby: rand(1..100)
来源：http://qjq.birdmap.top

C#:   new Random().Next(1, 101)
来源：http://fmk.hcnkem.com

[A11] 条件表达式（三元）
来源：http://kle.xuanzx.com

Py:   "yes" if x > 0 else "no"
来源：http://ipi.hysaishi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ibs.hcnkem.com

JS:   x > 0 ? "yes" : "no"
来源：http://ikf.hesvh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dvr.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://rct.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hul.meibo888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yvu.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://iuj.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://nnv.shuidangran.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ypa.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tqk.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://col.c1oappe.top

TS:   `Hello, ${name}!`
来源：http://ala.guannengcc.top

Java: "Hello, %s!".formatted(name)
来源：http://cvl.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://goq.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://tqf.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://uvf.zhongyouzk.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uea.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://ram.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://uga.sweek.top

JS:   "第一行\n第二行"
来源：http://pqn.sufxvd.cn

TS:   "第一行\n第二行"
来源：http://yos.bjfxy.top

Java: "第一行\n第二行"
来源：http://dgx.xinyue.icu

Go:   "第一行\n第二行"
来源：http://yab.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://mwa.xuanzx.com

C#:   "第一行\n第二行"
来源：http://nht.fzhhl.top

[A14] 注释写法
来源：http://tmu.xziqi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rhp.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rrh.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://tsk.shangyingyoupin.top

TS:   // 单行；/* 多行 */
来源：http://yuk.xuanzx.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xdw.jlsjyb.cn

Go:   // 单行；/* 多行 */
来源：http://shy.jlsjyb.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rjd.zhengqikj.top

C#:   // 单行；/* 多行 */
来源：http://upt.tian-w.cn

[A15] 空值判断与默认值
来源：http://dnx.hongshengwenyu.top

Py:   value = data or "默认值"
来源：http://kut.wangdashe.top

PHP:  $value = $data ?? "默认值";
来源：http://lih.jiagoushi.top

JS:   const value = data ?? "默认值";
来源：http://wuo.zhixingplan.top

TS:   const value = data ?? "默认值";
来源：http://ebg.yvedp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eru.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://rxk.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://rbi.sysykeji.top

C#:   var value = data ?? "默认值";
来源：http://wbm.xziqi.cn

[A16] 真假值判断规则
来源：http://eov.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bfw.ydzc1.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://juj.tanke756.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fpw.9152youxi.cn

TS:   if (!x) {}
来源：http://ysd.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://awe.hnqzz.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yyg.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jet.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yph.aibaodan.cn

[A17] 位运算
来源：http://rqi.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yba.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lqe.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfh.sysykeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bqq.feifeiyinyue.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oxq.shzxlz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ffc.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gam.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://htf.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://nmw.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://fuk.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://zoa.snrcjt.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wqi.c1oappe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vwi.316326.xyz

Java: (int) 'A'; (char) 65
来源：http://ngx.sjlbkw.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dwh.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://yic.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://jpc.ehwqpu.com

[A19] 交换两个变量
来源：http://hwm.guannengcc.top

Py:   a, b = b, a
来源：http://ads.nanxinkj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://yye.meibo888.top

JS:   [a, b] = [b, a];
来源：http://jyn.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://xfv.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://ref.zhoulong.xyz

Go:   a, b = b, a
来源：http://cou.cashguo.top

Ruby: a, b = b, a
来源：http://ldb.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://phc.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://ytx.fzhhl.top

Py:   name = input("请输入：")
来源：http://bxn.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kvj.yangfankeji.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qrq.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://woc.andypj.xyz

Java: new Scanner(System.in).nextLine()
来源：http://hfy.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uey.tianlin.xyz

Ruby: gets.chomp
来源：http://nns.yonumen.top

C#:   Console.ReadLine();
来源：http://ygb.wangshuangyany.cn

[A21] 保留指定小数位输出
来源：http://uho.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://kkh.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://snh.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://dqi.ppjwa.cn

TS:   (3.14159).toFixed(2)
来源：http://tvg.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://aeb.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kza.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://qii.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://wvb.jinqigufen.top

[A22] 获取字符串长度
来源：http://wjr.kuanghao11.cn

Py:   len(s)
来源：http://rlr.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xoz.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pee.pycfn.com

TS:   s.length
来源：http://fmh.wangshuangyany.cn

Java: s.length()
来源：http://tml.xuetiantiany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mhw.cashguo.top

Ruby: s.length
来源：http://cel.pengpengdd.cyou

C#:   s.Length
来源：http://unb.jinghuilouyu.cn

[A23] 大小写转换
来源：http://pto.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tbo.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xec.pengpengdd.cyou

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dav.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bmm.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dlm.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lvd.feifeiyinyue.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://icd.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://bbo.xziqi.cn

[A24] 去除首尾空白
来源：http://ckf.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qav.wangdashe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://khw.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://irz.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ubv.sjlbkw.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://spe.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://icf.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zvc.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pyt.jiagoushi.top

[A25] 字符串比较
来源：http://fhc.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://exp.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ago.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gxu.yfazqb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dij.jqgufenzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mkz.zycfv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pjn.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qjl.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ule.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://adz.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jop.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yvs.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zcq.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://vez.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pjo.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wqd.yanxiufei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dje.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xua.jinghuilouyu.cn

================================================================================
来源：http://zan.andypj.xyz

B. 流程控制
来源：http://pfv.yuxming.cn

================================================================================
来源：http://fvs.xinyue.icu

[B01] 条件判断 if / else
来源：http://yty.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://agk.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://frh.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sia.jqgfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sja.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://mnt.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cpf.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://isx.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kvd.epnwcf.com

[B02] 多分支 else if / elif
来源：http://kyl.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hgv.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jmy.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hyo.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://snh.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eif.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mes.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pgv.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fvo.redwolf501.top

[B03] switch / match / case
来源：http://bah.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qjc.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wbi.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cbp.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uxd.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dyq.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kiv.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eda.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yff.redwolf501.top

[B04] for 计数循环
来源：http://ubs.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://xge.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hxj.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://emm.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wij.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sgr.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://osc.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://gcl.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pjw.yj202588.top

[B05] 遍历数组 / 列表
来源：http://fwi.hnqzz.top

Py:   for item in arr: print(item)
来源：http://lli.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cnf.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ebz.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lki.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wbo.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dtu.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://lbl.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nix.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://rte.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://edp.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ddb.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qwf.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qfi.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rmy.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://grk.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nxk.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://amq.kuanghao11.cn

[B07] while 循环
来源：http://ptw.shuidangran.top

Py:   while i < 10: i += 1
来源：http://eou.chenjidiqi.icu


<!-- 参考信息 -->