代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fdb.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://huz.cheryme.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cmn.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kjv.hongshengwenyu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ksj.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tpc.hammf.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zgx.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rhw.yangfankeji.com

================================================================================
来源：http://fqb.sweek.top

A. 基础语法与类型
来源：http://pgr.gaohongyu789.top

================================================================================
来源：http://dkl.shuidangran.top

[A01] Hello World
来源：http://lsb.yuxming.cn

Py:   print("Hello, World!")
来源：http://ffy.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://bob.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://dhe.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ksr.yj202588.top

Java: System.out.println("Hello, World!");
来源：http://hwk.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://fty.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://tuv.zhengqikj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vbw.ctjpmb.com

[A02] 变量声明与赋值
来源：http://zks.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gbd.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ozh.fehbvm.com

JS:   let name = "Alex"; const age = 20;
来源：http://sqe.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ndf.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://mow.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://tac.wangshuangyany.cn

Ruby: name = "Alex"; age = 20
来源：http://xxf.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lqf.yangfankeji.com

[A03] 常量定义
来源：http://dbl.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pzx.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://ebb.52xcode.cn

JS:   const PI = 3.14159;
来源：http://ncf.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://ems.cheryme.top

Java: static final double PI = 3.14159;
来源：http://low.daxiang520.top

Go:   const PI = 3.14159
来源：http://shy.ydjk.org.cn

Ruby: PI = 3.14159
来源：http://tnx.jinyuanbaomall.cn

C#:   const double PI = 3.14159;
来源：http://loo.ehwqpu.com

[A04] 判断变量类型
来源：http://tip.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://jsd.xuanzx.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://che.mhx1999.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zti.sweek.top

TS:   typeof x; x instanceof Date
来源：http://eox.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qdt.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iov.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://una.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://zes.yanxiufei.cn

[A05] 整数除法与取模
来源：http://nxh.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hxp.snrcjt.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fdi.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lal.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mlx.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://ysu.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://qqs.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://amd.sjlbkw.cn

C#:   7 / 2; 7 % 2
来源：http://fda.hcnkem.com

[A06] 字符串转数字
来源：http://rgk.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://jox.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tfg.nanxuanxn.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ikm.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://mdg.cqqwz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wwo.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://brf.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://pcw.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://etm.yonumen.top

[A07] 数字转字符串
来源：http://dcb.gotoacloud.top

Py:   str(42)
来源：http://bni.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://ivv.cucudq.cn

JS:   String(42); (42).toString()
来源：http://dbe.meibo888.top

TS:   String(42)
来源：http://fxo.cqqwz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://odm.ywan-chungtsiang.top

Go:   strconv.Itoa(42)
来源：http://fed.andypj.xyz

Ruby: 42.to_s
来源：http://rzz.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://kya.xingfuxueyuan.xyz

[A08] 取整与四舍五入
来源：http://suo.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dov.iojbl.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uhy.jyoumei.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vgo.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://swb.jqgufenzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://chx.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pqr.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uzi.nanxinkj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wzl.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://kjc.sufxvd.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wes.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qrx.haohaochexian.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://coo.shzxlz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://okj.hnqzz.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bts.yongpay.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yis.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gax.snrcjt.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zwi.jlsjyb.cn

[A10] 生成随机数
来源：http://gxx.xinyue.icu

Py:   import random; random.randint(1, 100)
来源：http://ujk.yfazqb.com

PHP:  random_int(1, 100);
来源：http://xmv.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pgm.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kcl.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://xyd.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xra.andypj.xyz

Ruby: rand(1..100)
来源：http://okc.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://jqn.mhx1999.top

[A11] 条件表达式（三元）
来源：http://prv.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://coq.daxiang520.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ftf.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://cma.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mcg.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://fzu.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tnn.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wdv.shzxlz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cox.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://jhi.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gsp.hysaishi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gfa.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://wlx.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://xmu.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://unh.yj20258.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rna.gogol.net.cn

Ruby: "Hello, #{name}!"
来源：http://iwp.yonumen.top

C#:   $"Hello, {name}!"
来源：http://jjc.hammf.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xhy.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://hch.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://tjf.yongpay.top

JS:   "第一行\n第二行"
来源：http://zff.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://jlo.dashuyun.cn

Java: "第一行\n第二行"
来源：http://uby.meibo888.top

Go:   "第一行\n第二行"
来源：http://lrx.shanyushiyangtech.top

Ruby: "第一行\n第二行"
来源：http://tyi.cdnleiting.top

C#:   "第一行\n第二行"
来源：http://cfu.jianghu66.top

[A14] 注释写法
来源：http://ffu.hysaishi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zat.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qph.jqgufenzy.top

JS:   // 单行；/* 多行 */
来源：http://zym.shanyushiyangkeji.top

TS:   // 单行；/* 多行 */
来源：http://ejy.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://elw.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://gle.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://eru.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://ggd.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://mdu.hammf.cn

Py:   value = data or "默认值"
来源：http://ttl.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://feh.chenlongwang.top

JS:   const value = data ?? "默认值";
来源：http://cph.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://gqo.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://njx.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://tmd.vehdjk.com

Ruby: value = data || "默认值"
来源：http://uas.kuanghao11.cn

C#:   var value = data ?? "默认值";
来源：http://bbf.sufxvd.cn

[A16] 真假值判断规则
来源：http://wai.0kj1m.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ncx.fzhhl.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hxa.gotoacloud.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tlo.gotoacloud.top

TS:   if (!x) {}
来源：http://rii.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dbx.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jbe.pycfn.com

Ruby: unless x            # nil 与 false 为假
来源：http://cmg.wangdashe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ebf.xziqi.cn

[A17] 位运算
来源：http://kmk.wangdashe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yhi.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aev.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnt.gogol.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fcy.daria6918.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xct.andypj.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://umk.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrz.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vpq.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://dmr.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://zdl.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://oin.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kvb.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ngy.vqdsnc.cn

Java: (int) 'A'; (char) 65
来源：http://dmh.zhiwuduotai.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kzr.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://zfo.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://qwu.jinghuilouyu.cn

[A19] 交换两个变量
来源：http://opz.jqgufenzy.top

Py:   a, b = b, a
来源：http://mob.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://obf.shanyushiyangtech.top

JS:   [a, b] = [b, a];
来源：http://sfj.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://icp.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://ixq.cucudq.cn

Go:   a, b = b, a
来源：http://ulr.andypj.xyz

Ruby: a, b = b, a
来源：http://ghg.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://baz.hysaishi.cn

[A20] 读取标准输入
来源：http://olc.andypj.xyz

Py:   name = input("请输入：")
来源：http://scv.tanke756.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tnu.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://juh.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://ual.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://jvh.xinyue.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kmw.jlsjyb.cn

Ruby: gets.chomp
来源：http://pgh.xinyue.icu

C#:   Console.ReadLine();
来源：http://nhr.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://uee.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://qxm.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qgc.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://rbc.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://rzl.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://dvn.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pzc.sweek.top

Ruby: format("%.2f", 3.14159)
来源：http://jit.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://vme.yongpay.top

[A22] 获取字符串长度
来源：http://seq.fehbvm.com

Py:   len(s)
来源：http://pgs.pycfn.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://neu.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mir.guannengcc.top

TS:   s.length
来源：http://pfg.tianlin.xyz

Java: s.length()
来源：http://juq.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lwu.jinqigufen.top

Ruby: s.length
来源：http://mvx.zhijiandao.cn

C#:   s.Length
来源：http://eog.haohaochexian.top

[A23] 大小写转换
来源：http://yqk.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://uoq.bbcook.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://adh.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wls.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://avl.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oik.ivvv.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://trf.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vrb.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nmj.dianchejie.cn

[A24] 去除首尾空白
来源：http://bca.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mla.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qok.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mhq.zhoulong.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rfw.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xle.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://fjp.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ewo.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kos.haohaochexian.top

[A25] 字符串比较
来源：http://stn.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://lwq.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oro.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dbn.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hcc.jqgfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oum.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lyh.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mlp.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yxo.bjfxy.top

[A26] 类型转换总览
来源：http://ish.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yax.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vae.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iet.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://bfp.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xfn.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://abc.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ghy.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zji.dashuyun.cn

================================================================================
来源：http://vpf.316326.xyz

B. 流程控制
来源：http://sid.sjlbkw.cn

================================================================================
来源：http://idr.mhx1999.top

[B01] 条件判断 if / else
来源：http://zsv.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nzm.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vay.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://btb.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hhi.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://aha.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rol.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gon.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://div.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://qwg.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ock.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tlz.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xjq.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qrr.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpw.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kkb.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ubb.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://keb.pengpengdd.cyou

[B03] switch / match / case
来源：http://hif.dianchejie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dsf.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nlh.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://glk.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dlk.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ysa.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ply.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hit.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://edw.aibaodan.cn

[B04] for 计数循环
来源：http://fxi.tarul.cn

Py:   for i in range(10): print(i)
来源：http://htr.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ddz.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dma.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qfi.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xor.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pos.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://rei.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ggv.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://wyu.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://qcu.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qtp.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://oob.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://okk.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yse.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ytt.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://wrk.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sle.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://tnt.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fop.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gsq.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://upv.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ine.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yip.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ffc.ppjwa.cn


<!-- 参考信息 -->