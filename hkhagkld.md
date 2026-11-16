代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lwy.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xff.guowangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zcc.ywan-chungtsiang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://obc.yuxming.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rec.shanyushiyangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dfe.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uyr.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qee.316326.xyz

================================================================================
来源：http://ffg.jianghu66.top

A. 基础语法与类型
来源：http://vyx.jinqigfzy.top

================================================================================
来源：http://flg.chenzaomai.com

[A01] Hello World
来源：http://hwh.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://cpl.xylfe.cn

PHP:  echo "Hello, World!";
来源：http://lwc.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://oyo.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tci.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://cpy.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://jyt.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://tgd.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nos.zhongyouzk.top

[A02] 变量声明与赋值
来源：http://zbh.quarkkingdee.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wfn.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://hhv.mhx1999.top

JS:   let name = "Alex"; const age = 20;
来源：http://tvq.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xtr.shuidangran.top

Java: String name = "Alex"; int age = 20;
来源：http://ttb.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://tvy.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://kmx.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vqy.yongpay.top

[A03] 常量定义
来源：http://iwl.wangshuangyany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lyo.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://jtc.daria6918.cn

JS:   const PI = 3.14159;
来源：http://fcp.ywan-chungtsiang.top

TS:   const PI: number = 3.14159;
来源：http://fiy.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://vkh.hfpthk.cn

Go:   const PI = 3.14159
来源：http://nlz.ivvv.top

Ruby: PI = 3.14159
来源：http://pnq.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://ydw.316326.xyz

[A04] 判断变量类型
来源：http://iyi.gaohongyu789.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vrp.ctjpmb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ycc.xylfe.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://euo.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://qlr.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wno.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://abf.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nus.andypj.xyz

C#:   x.GetType().Name; x is int
来源：http://okj.haohaochexian.top

[A05] 整数除法与取模
来源：http://iwl.snrcjt.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vry.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wmf.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xiu.meibo888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://izh.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://bjz.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://dch.yueranfly.top

Ruby: 7 / 2; 7 % 2
来源：http://hox.hammf.cn

C#:   7 / 2; 7 % 2
来源：http://yhl.daria6918.cn

[A06] 字符串转数字
来源：http://lkb.yongpay.top

Py:   int("42"); float("3.14")
来源：http://wru.yongpay.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tch.aibaodan.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yoh.0kj1m.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ohq.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ufq.gaohongyu789.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://haw.aibaodan.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mmk.cdnleiting.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ths.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://lbu.cqqwz.cn

Py:   str(42)
来源：http://myc.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://mft.jinyuanbaomall.cn

JS:   String(42); (42).toString()
来源：http://rov.ctjpmb.com

TS:   String(42)
来源：http://wiv.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ytx.jinqigufen.top

Go:   strconv.Itoa(42)
来源：http://tdc.cqqwz.cn

Ruby: 42.to_s
来源：http://opk.52xcode.cn

C#:   42.ToString()
来源：http://lwx.jinghuilouyu.cn

[A08] 取整与四舍五入
来源：http://kga.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gbp.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jip.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qcm.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qyb.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hxa.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nhe.fanxiaobao.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://obg.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ria.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://cii.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://llu.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gjx.shanyushiyangtech.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ojd.gaohongyu789.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://buh.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gtm.jlsjyb.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yht.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nci.xinyue.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uht.yangfankeji.com

[A10] 生成随机数
来源：http://dbz.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://qvf.sysykeji.top

PHP:  random_int(1, 100);
来源：http://qvp.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://axe.yuanzhike.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ntb.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://mxu.vqdsnc.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://atq.zhaomingkeji.xyz

Ruby: rand(1..100)
来源：http://fln.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://fbw.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://trn.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://yld.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://afn.daxiang520.top

JS:   x > 0 ? "yes" : "no"
来源：http://nyo.redwolf501.top

TS:   x > 0 ? "yes" : "no"
来源：http://qsf.yuxming.cn

Java: x > 0 ? "yes" : "no"
来源：http://olx.yueranfly.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tgi.feifeiyinyue.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jfq.smart0.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://vfe.yj202588.top

[A12] 字符串插值 / 格式化
来源：http://hka.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aco.bjfxy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kof.epnwcf.com

JS:   `Hello, ${name}!`
来源：http://ops.hcnkem.com

TS:   `Hello, ${name}!`
来源：http://xqs.sxryk.cn

Java: "Hello, %s!".formatted(name)
来源：http://jzc.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://arq.ctjpmb.com

Ruby: "Hello, #{name}!"
来源：http://hts.daria6918.cn

C#:   $"Hello, {name}!"
来源：http://gbn.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://she.sufxvd.cn

Py:   "第一行\n第二行"
来源：http://xaa.wangshuangyany.cn

PHP:  "第一行\n第二行"
来源：http://sxn.cheryme.top

JS:   "第一行\n第二行"
来源：http://gly.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://xnk.fktsv.cn

Java: "第一行\n第二行"
来源：http://fom.316326.xyz

Go:   "第一行\n第二行"
来源：http://nfv.tarul.cn

Ruby: "第一行\n第二行"
来源：http://lip.tian-w.cn

C#:   "第一行\n第二行"
来源：http://ikv.yj20258.top

[A14] 注释写法
来源：http://yzj.chenlongwang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://yip.tianlin.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://cnm.316326.xyz

JS:   // 单行；/* 多行 */
来源：http://wsg.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://tre.ywan-chungtsiang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aox.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://guc.haohaochexian.top

Ruby: # 单行；=begin 多行 =end
来源：http://xpt.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://qjk.daxiang520.top

[A15] 空值判断与默认值
来源：http://ovq.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://odh.ydzc1.top

PHP:  $value = $data ?? "默认值";
来源：http://ahv.nanxinkj.top

JS:   const value = data ?? "默认值";
来源：http://efu.tianlin.xyz

TS:   const value = data ?? "默认值";
来源：http://zkg.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tuk.zhengqikj.top

Go:   if data == "" { data = "默认值" }
来源：http://hfp.ywan-chungtsiang.top

Ruby: value = data || "默认值"
来源：http://rdi.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://qpt.tarul.cn

[A16] 真假值判断规则
来源：http://ubl.cdnleiting.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://prx.quarkkingdee.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wxx.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ouz.haohaochexian.top

TS:   if (!x) {}
来源：http://omq.nanxuanxn.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hwc.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aze.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ita.dianchejie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aos.cucudq.cn

[A17] 位运算
来源：http://han.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cod.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bfe.hcnkem.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxq.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rom.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rkk.cqqwz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ilp.zhiwuduotai.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufb.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rvq.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://vyp.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://zlh.316326.xyz

PHP:  ord("A"); chr(65)
来源：http://fnc.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zlz.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zov.yuanzhike.top

Java: (int) 'A'; (char) 65
来源：http://xqo.nanxuanxn.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xas.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://ovc.jinghuilouyu.cn

C#:   (int)'A'; (char)65
来源：http://wzv.fengsongda.top

[A19] 交换两个变量
来源：http://rqv.hongshengwenyu.top

Py:   a, b = b, a
来源：http://qdl.fengsongda.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dpf.vqdsnc.cn

JS:   [a, b] = [b, a];
来源：http://mom.yj20258.top

TS:   [a, b] = [b, a];
来源：http://yrv.daria6918.cn

Java: int t = a; a = b; b = t;
来源：http://zdh.mhx1999.top

Go:   a, b = b, a
来源：http://abk.ydzc1.top

Ruby: a, b = b, a
来源：http://tvp.cashguo.top

C#:   (a, b) = (b, a);
来源：http://cci.snrcjt.cn

[A20] 读取标准输入
来源：http://ivh.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://oog.sjlbkw.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://luy.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://afm.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://jvn.aibaodan.cn

Java: new Scanner(System.in).nextLine()
来源：http://bpq.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zzi.yvedp.cn

Ruby: gets.chomp
来源：http://ocp.kuanghao11.cn

C#:   Console.ReadLine();
来源：http://mpj.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://dsh.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://rbi.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ejs.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://dqk.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://cmr.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://koi.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jwd.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://lln.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://rbu.tanke756.top

[A22] 获取字符串长度
来源：http://hhe.xuanzx.com

Py:   len(s)
来源：http://nrk.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://syw.9152youxi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xil.zycfv.cn

TS:   s.length
来源：http://koc.zhixingplan.top

Java: s.length()
来源：http://grp.feifeiyinyue.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://juz.shuidangran.top

Ruby: s.length
来源：http://eck.jinqigfzy.top

C#:   s.Length
来源：http://mqy.hongshengwenyu.top

[A23] 大小写转换
来源：http://kkn.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://gij.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cfy.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bmf.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://opb.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kng.chenzaomai.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ivg.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ehj.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vyr.quarkkingdee.top

[A24] 去除首尾空白
来源：http://drr.bbcook.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://abw.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lop.pycfn.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aui.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sys.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jtm.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://sda.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tbl.daxiang520.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mon.gaohongyu789.top

[A25] 字符串比较
来源：http://bjr.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://vyz.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qll.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nqs.quarkkingdee.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jcb.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fzx.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wec.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kep.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zpm.aibaodan.cn

[A26] 类型转换总览
来源：http://vsh.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zti.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tnf.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bvm.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://nuf.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eno.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dji.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kxn.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wtm.cqqwz.cn

================================================================================
来源：http://bqy.daxiang520.top

B. 流程控制
来源：http://wiu.zhixingplan.top

================================================================================
来源：http://aie.xziqi.cn

[B01] 条件判断 if / else
来源：http://xit.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lbf.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pys.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gjy.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xkq.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zvb.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hsa.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nug.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://man.xziqi.cn

[B02] 多分支 else if / elif
来源：http://epy.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gmy.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cne.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ass.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://naz.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxy.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xsg.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xme.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sel.nanxinkj.top

[B03] switch / match / case
来源：http://rwv.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rxc.feifeiyinyue.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kyx.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jwp.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yns.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://amu.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lzo.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uky.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pju.hfpthk.cn

[B04] for 计数循环
来源：http://jlv.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://tuc.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vyv.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bok.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxq.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aor.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fux.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://wzu.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oze.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://qmj.hcnkem.com

Py:   for item in arr: print(item)
来源：http://lha.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xks.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bwo.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lvp.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qnh.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gne.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://dtr.pycfn.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ufz.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://ffv.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dxd.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://set.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kxy.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qvg.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://siq.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://esk.dianchejie.cn


<!-- 参考信息 -->