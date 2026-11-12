代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mqd.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ifs.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zqk.tanke756.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://khf.fktsv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yhx.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ucn.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vww.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qze.xylfe.cn

================================================================================
来源：http://kun.nwbrower.top

A. 基础语法与类型
来源：http://kwt.zhixingplan.top

================================================================================
来源：http://gsk.bjfxy.top

[A01] Hello World
来源：http://xdy.guannengcc.top

Py:   print("Hello, World!")
来源：http://ofe.zdbjq.cn

PHP:  echo "Hello, World!";
来源：http://ezm.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://dzq.zhiwuduotai.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kob.aizwys.cn

Java: System.out.println("Hello, World!");
来源：http://snn.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://wia.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://lkj.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tcv.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://hlc.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ddf.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dbf.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://qen.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hnt.xziqi.cn

Java: String name = "Alex"; int age = 20;
来源：http://hwk.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://clz.ybcxt.top

Ruby: name = "Alex"; age = 20
来源：http://bbz.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hqw.shangyingyoupin.top

[A03] 常量定义
来源：http://gco.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bvq.guowangkeji.top

PHP:  const PI = 3.14159;
来源：http://ddt.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://auh.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://lfk.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://mqy.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://yyo.dashuyun.cn

Ruby: PI = 3.14159
来源：http://swu.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://zod.shanyushiyangkeji.top

[A04] 判断变量类型
来源：http://dts.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://txn.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yaj.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aim.sufxvd.cn

TS:   typeof x; x instanceof Date
来源：http://bje.gogol.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hhi.iojbl.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yhq.wangdashe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jbt.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://rei.cashguo.top

[A05] 整数除法与取模
来源：http://zik.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vzg.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://knl.vqdsnc.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mqw.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pxb.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://dir.zdbjq.cn

Go:   7 / 2; 7 % 2
来源：http://yal.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://qmc.shzxlz.cn

C#:   7 / 2; 7 % 2
来源：http://xga.dashuyun.cn

[A06] 字符串转数字
来源：http://kkd.shanyushiyangkeji.top

Py:   int("42"); float("3.14")
来源：http://pau.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kuh.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sti.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ekt.zhongyouzk.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uru.zhijiandao.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gdk.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zjf.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fse.yongpay.top

[A07] 数字转字符串
来源：http://wkb.vehdjk.com

Py:   str(42)
来源：http://mtu.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://utf.yj20258888.top

JS:   String(42); (42).toString()
来源：http://sfw.sjlbkw.cn

TS:   String(42)
来源：http://nks.snrcjt.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pkt.ivvv.top

Go:   strconv.Itoa(42)
来源：http://xbi.wangdashe.top

Ruby: 42.to_s
来源：http://jsf.hfpthk.cn

C#:   42.ToString()
来源：http://ryr.chenlongwang.top

[A08] 取整与四舍五入
来源：http://nno.daria6918.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bbz.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ylu.iojbl.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iuv.fehbvm.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lmm.shzxlz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hwk.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ubt.hnqzz.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://otv.chenjidiqi.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bsi.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://bvb.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nie.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qsf.zdbjq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lsm.tarul.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vhu.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mnr.shanyushiyangtech.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pve.cqqwz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ahy.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://veo.sweek.top

[A10] 生成随机数
来源：http://smx.nanxinkj.top

Py:   import random; random.randint(1, 100)
来源：http://nuy.52xcode.cn

PHP:  random_int(1, 100);
来源：http://lmm.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bjm.zhijiandao.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cjo.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://xqr.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mix.dianchejie.cn

Ruby: rand(1..100)
来源：http://wro.yueranfly.top

C#:   new Random().Next(1, 101)
来源：http://fxc.yonumen.top

[A11] 条件表达式（三元）
来源：http://woy.snrcjt.cn

Py:   "yes" if x > 0 else "no"
来源：http://kin.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://rre.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://sey.vqdsnc.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rmq.yanxiufei.cn

Java: x > 0 ? "yes" : "no"
来源：http://cfc.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hbw.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jas.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://uzo.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://why.hnqzz.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nrw.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jas.xinyue.icu

JS:   `Hello, ${name}!`
来源：http://ebg.jinqigfzy.top

TS:   `Hello, ${name}!`
来源：http://gvv.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://ird.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cea.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://hyn.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://dyw.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fnt.nanxinkj.top

Py:   "第一行\n第二行"
来源：http://mzk.sweek.top

PHP:  "第一行\n第二行"
来源：http://iif.0kj1m.cn

JS:   "第一行\n第二行"
来源：http://sso.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://deo.yj202588.top

Java: "第一行\n第二行"
来源：http://ntw.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://dny.jqgufenzy.top

Ruby: "第一行\n第二行"
来源：http://xxx.sysykeji.top

C#:   "第一行\n第二行"
来源：http://cuu.zhoulong.xyz

[A14] 注释写法
来源：http://wit.vehdjk.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://cma.bbcook.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tgr.kuanghao11.cn

JS:   // 单行；/* 多行 */
来源：http://lvk.9152youxi.cn

TS:   // 单行；/* 多行 */
来源：http://iff.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rqi.redwolf501.top

Go:   // 单行；/* 多行 */
来源：http://nmd.nwbrower.top

Ruby: # 单行；=begin 多行 =end
来源：http://qpy.cdnleiting.top

C#:   // 单行；/* 多行 */
来源：http://ewh.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://wci.guowangkeji.top

Py:   value = data or "默认值"
来源：http://qbd.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://bhr.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://bsa.zhixingplan.top

TS:   const value = data ?? "默认值";
来源：http://fkc.nanxinkj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ezp.hongshengwenyu.top

Go:   if data == "" { data = "默认值" }
来源：http://sza.andypj.xyz

Ruby: value = data || "默认值"
来源：http://zrg.zhaomingkeji.xyz

C#:   var value = data ?? "默认值";
来源：http://zqm.snrcjt.cn

[A16] 真假值判断规则
来源：http://zzn.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jfy.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sfn.jinghuilouyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kqm.fehbvm.com

TS:   if (!x) {}
来源：http://pon.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ctq.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xsq.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://txf.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eng.xuetiantiany.cn

[A17] 位运算
来源：http://srt.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vmi.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cpi.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://psi.316326.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dio.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xln.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gho.ydzc1.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txx.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lxh.wangdashe.top

[A18] 字符与 ASCII 码互转
来源：http://tau.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://xhm.yj20258.top

PHP:  ord("A"); chr(65)
来源：http://xds.xingfuxueyuan.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://adm.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nyr.guowangkeji.top

Java: (int) 'A'; (char) 65
来源：http://xcm.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tdc.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://vpd.guowangkeji.top

C#:   (int)'A'; (char)65
来源：http://xyc.cashguo.top

[A19] 交换两个变量
来源：http://ccg.nwbrower.top

Py:   a, b = b, a
来源：http://nnr.zhiwuduotai.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wco.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://pdx.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://xgs.zycfv.cn

Java: int t = a; a = b; b = t;
来源：http://bht.gotoacloud.top

Go:   a, b = b, a
来源：http://rtg.shzxlz.cn

Ruby: a, b = b, a
来源：http://ekq.gzhubu.top

C#:   (a, b) = (b, a);
来源：http://nph.shzxlz.cn

[A20] 读取标准输入
来源：http://iri.tarul.cn

Py:   name = input("请输入：")
来源：http://qfb.sysykeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://thi.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://htx.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://hyf.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://iqn.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ice.nanxuanxn.top

Ruby: gets.chomp
来源：http://wyq.cheryme.top

C#:   Console.ReadLine();
来源：http://xen.yanxiufei.cn

[A21] 保留指定小数位输出
来源：http://wot.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://prs.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eed.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://tbv.ppjwa.cn

TS:   (3.14159).toFixed(2)
来源：http://dle.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://rcu.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fyt.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://pwu.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://sdx.daxiang520.top

[A22] 获取字符串长度
来源：http://lqw.zhoulong.xyz

Py:   len(s)
来源：http://dfx.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zss.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://riy.shangyingyoupin.top

TS:   s.length
来源：http://ugz.snrcjt.cn

Java: s.length()
来源：http://zve.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uaj.zhijiandao.cn

Ruby: s.length
来源：http://elv.yangfankeji.com

C#:   s.Length
来源：http://xwi.tian-w.cn

[A23] 大小写转换
来源：http://klt.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xaa.cucudq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xba.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zda.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tjf.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cum.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vvm.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ynv.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://han.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://waa.epnwcf.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ojk.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fky.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ydc.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pdi.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://liy.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://vwq.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pak.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zxe.zhengqikj.top

[A25] 字符串比较
来源：http://pux.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://efv.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://omk.tianlin.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lhk.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bhe.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xvs.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aax.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kwk.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kqb.xylfe.cn

[A26] 类型转换总览
来源：http://ihe.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nnk.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mga.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dea.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://dcm.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cyu.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ddk.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://swa.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hrn.fehbvm.com

================================================================================
来源：http://ojs.fehbvm.com

B. 流程控制
来源：http://rvh.sufxvd.cn

================================================================================
来源：http://gku.zhengqikj.top

[B01] 条件判断 if / else
来源：http://uhj.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://bme.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ojr.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gep.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://csy.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xik.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qbc.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uph.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qas.tarul.cn

[B02] 多分支 else if / elif
来源：http://pic.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://slf.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qfh.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zld.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcx.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sul.hnqzz.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zfd.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gny.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yrp.aizwys.cn

[B03] switch / match / case
来源：http://klg.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kdh.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uzj.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://srp.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xwl.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mya.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mhs.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://izl.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xss.52xcode.cn

[B04] for 计数循环
来源：http://gxk.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://kzr.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fcg.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rwd.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ect.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fxv.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://swv.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://ebj.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bzl.tarul.cn

[B05] 遍历数组 / 列表
来源：http://aeg.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://vxz.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qxh.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zks.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bes.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yem.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wks.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://wwx.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oym.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://ktr.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qjv.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pyq.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pyb.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fhp.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cgr.bbcook.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sbb.cqqwz.cn


<!-- 参考信息 -->