代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://uel.pengpengdd.cyou

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tzm.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hrz.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jhe.fktsv.cn

================================================================================
来源：http://bcq.yfazqb.com

A. 基础语法与类型
来源：http://fes.hfpthk.cn

================================================================================
来源：http://vww.wangdashe.top

[A01] Hello World
来源：http://iig.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://uvk.9152youxi.cn

PHP:  echo "Hello, World!";
来源：http://amz.yanxiufei.cn

JS:   console.log("Hello, World!");
来源：http://tlk.sufxvd.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fqh.tarul.cn

Java: System.out.println("Hello, World!");
来源：http://isw.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://fct.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://dqo.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vur.zdbjq.cn

[A02] 变量声明与赋值
来源：http://ngv.9152youxi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xsf.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://fmr.aibaodan.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qsu.9152youxi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ruq.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://okx.pycfn.com

Go:   name := "Alex"; age := 20
来源：http://gys.tarul.cn

Ruby: name = "Alex"; age = 20
来源：http://wca.9152youxi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vre.ybcxt.top

[A03] 常量定义
来源：http://aqz.jiagoushi.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uun.pycfn.com

PHP:  const PI = 3.14159;
来源：http://ljd.yj20258.top

JS:   const PI = 3.14159;
来源：http://ljv.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://llp.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://rsd.bbcook.cn

Go:   const PI = 3.14159
来源：http://vfd.chenjidiqi.icu

Ruby: PI = 3.14159
来源：http://arr.dashuyun.cn

C#:   const double PI = 3.14159;
来源：http://dbw.pengpengdd.cyou

[A04] 判断变量类型
来源：http://fea.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fyq.tanke756.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zdo.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qvm.fktsv.cn

TS:   typeof x; x instanceof Date
来源：http://qcy.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sik.cdnleiting.top

Go:   reflect.TypeOf(x).Name()
来源：http://jem.shangyingyoupin.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tls.zdbjq.cn

C#:   x.GetType().Name; x is int
来源：http://jyj.52xcode.cn

[A05] 整数除法与取模
来源：http://fgl.wangshuangyany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://phk.c1oappe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gmz.dianchejie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ohc.tarul.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vcp.yuxming.cn

Java: 7 / 2; 7 % 2
来源：http://fbf.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://tqu.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://jqu.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://dqz.yueranfly.top

[A06] 字符串转数字
来源：http://lqu.sxryk.cn

Py:   int("42"); float("3.14")
来源：http://ydl.quarkkingdee.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://esb.9152youxi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yfs.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vwp.guannengcc.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://guc.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lsy.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jgn.gzhubu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ohw.9152youxi.cn

[A07] 数字转字符串
来源：http://ggj.xinyue.icu

Py:   str(42)
来源：http://zsx.xuanzx.com

PHP:  (string) 42; strval(42)
来源：http://kbm.jqgufenzy.top

JS:   String(42); (42).toString()
来源：http://pxd.hongshengwenyu.top

TS:   String(42)
来源：http://lke.hcnkem.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://voc.daxiang520.top

Go:   strconv.Itoa(42)
来源：http://cvg.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://zgz.0kj1m.cn

C#:   42.ToString()
来源：http://mii.jinqigufen.top

[A08] 取整与四舍五入
来源：http://bjh.ydjk.org.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ehz.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xdr.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wmz.uphjek.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bnj.hysaishi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ppo.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fuf.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qui.shanyushiyangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://utn.yuanzhike.top

[A09] 绝对值与最大最小值
来源：http://qiu.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wrj.haohaochexian.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xaa.jyoumei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dco.hfpthk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oav.9152youxi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://llk.yuanzhike.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ntc.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lsj.zhijiandao.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mfw.xinyue.icu

[A10] 生成随机数
来源：http://ibb.zhengqikj.top

Py:   import random; random.randint(1, 100)
来源：http://ycb.dashuyun.cn

PHP:  random_int(1, 100);
来源：http://hkp.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ikq.c1oappe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dsq.xuetiantiany.cn

Java: new Random().nextInt(100) + 1
来源：http://gsx.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lzk.0kj1m.cn

Ruby: rand(1..100)
来源：http://msp.ybcxt.top

C#:   new Random().Next(1, 101)
来源：http://ogx.jinqigfzy.top

[A11] 条件表达式（三元）
来源：http://ylx.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://mxe.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://unt.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://nkd.shanyushiyangtech.top

TS:   x > 0 ? "yes" : "no"
来源：http://sjl.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://nmd.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gza.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dnx.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://ony.c1oappe.top

[A12] 字符串插值 / 格式化
来源：http://ryb.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://byt.hysaishi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vjo.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://shp.yuanzhike.top

TS:   `Hello, ${name}!`
来源：http://lvq.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://oyg.jinqigfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dqu.chenjidiqi.icu

Ruby: "Hello, #{name}!"
来源：http://kbe.dianchejie.cn

C#:   $"Hello, {name}!"
来源：http://fdu.chenzaomai.com

[A13] 多行字符串（练习 \n 转义）
来源：http://vjx.zhongyouzk.top

Py:   "第一行\n第二行"
来源：http://gjh.sysykeji.top

PHP:  "第一行\n第二行"
来源：http://dlv.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://fwb.vehdjk.com

TS:   "第一行\n第二行"
来源：http://ahu.chenlongwang.top

Java: "第一行\n第二行"
来源：http://ogl.vehdjk.com

Go:   "第一行\n第二行"
来源：http://dfz.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://rtt.redwolf501.top

C#:   "第一行\n第二行"
来源：http://fhd.sweek.top

[A14] 注释写法
来源：http://fgp.uphjek.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://lgk.daxiang520.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rgw.wangshuangyany.cn

JS:   // 单行；/* 多行 */
来源：http://xqo.bbcook.cn

TS:   // 单行；/* 多行 */
来源：http://ecl.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oef.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://bjp.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ica.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://qql.cdnleiting.top

[A15] 空值判断与默认值
来源：http://orm.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://vjq.xylfe.cn

PHP:  $value = $data ?? "默认值";
来源：http://gti.smart0.xyz

JS:   const value = data ?? "默认值";
来源：http://ois.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://yfc.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://srz.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://usw.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://bde.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://whn.yonumen.top

[A16] 真假值判断规则
来源：http://umn.sweek.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://izm.dianchejie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://haw.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iav.cheryme.top

TS:   if (!x) {}
来源：http://izo.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ply.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vhx.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dap.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pyx.fktsv.cn

[A17] 位运算
来源：http://gtq.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://spj.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tzn.daxiang520.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxg.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://erv.tianlin.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gxi.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dtz.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nwe.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjn.quarkkingdee.top

[A18] 字符与 ASCII 码互转
来源：http://fxd.feifeiyinyue.top

Py:   ord("A"); chr(65)
来源：http://nju.hongshengwenyu.top

PHP:  ord("A"); chr(65)
来源：http://wjg.sxryk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ikz.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wia.yanxiufei.cn

Java: (int) 'A'; (char) 65
来源：http://hfg.guowangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qoq.zhoulong.xyz

Ruby: "A".ord; 65.chr
来源：http://ype.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://vom.tarul.cn

[A19] 交换两个变量
来源：http://rym.52xcode.cn

Py:   a, b = b, a
来源：http://pbq.nwbrower.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dvq.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://kbj.hcnkem.com

TS:   [a, b] = [b, a];
来源：http://xsh.pengpengdd.cyou

Java: int t = a; a = b; b = t;
来源：http://cyj.sxryk.cn

Go:   a, b = b, a
来源：http://rew.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://xlb.9152youxi.cn

C#:   (a, b) = (b, a);
来源：http://vne.havefunace.top

[A20] 读取标准输入
来源：http://cdh.fengsongda.top

Py:   name = input("请输入：")
来源：http://arn.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://uqx.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zrg.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://zge.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://qzz.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://swj.yonumen.top

Ruby: gets.chomp
来源：http://doe.vehdjk.com

C#:   Console.ReadLine();
来源：http://kkd.yvedp.cn

[A21] 保留指定小数位输出
来源：http://gqg.sxryk.cn

Py:   f"{3.14159:.2f}"
来源：http://hxz.hongshengwenyu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://juv.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://ljp.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://ktu.yuanzhike.top

Java: String.format("%.2f", 3.14159)
来源：http://kua.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fvd.jinghuilouyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://kre.uphjek.com

C#:   3.14159.ToString("F2")
来源：http://jqn.svipenyu.cn

[A22] 获取字符串长度
来源：http://ycj.ydjk.org.cn

Py:   len(s)
来源：http://hwi.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ttn.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ogb.yueranfly.top

TS:   s.length
来源：http://nmd.c1oappe.top

Java: s.length()
来源：http://njk.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gzn.yj202588.top

Ruby: s.length
来源：http://bol.jinghuilouyu.cn

C#:   s.Length
来源：http://tpn.zhijiandao.cn

[A23] 大小写转换
来源：http://api.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://aim.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wju.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pkx.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fqc.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cso.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tci.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tqv.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bkr.haohaochexian.top

[A24] 去除首尾空白
来源：http://qme.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tbx.zdbjq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nih.yuxming.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iwv.yonumen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sem.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dmg.zhixingplan.top

Go:   strings.TrimSpace(s)
来源：http://xoy.gogol.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pln.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pmp.iojbl.cn

[A25] 字符串比较
来源：http://skz.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://znh.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://swg.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zga.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bpk.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qny.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://juj.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aee.yonumen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mzd.hongshengwenyu.top

[A26] 类型转换总览
来源：http://kql.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zwe.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eaj.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cgg.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://knn.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://osa.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qvx.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://tdb.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fbw.52xcode.cn

================================================================================
来源：http://udi.cdnleiting.top

B. 流程控制
来源：http://ldh.ywan-chungtsiang.top

================================================================================
来源：http://ipy.vehdjk.com

[B01] 条件判断 if / else
来源：http://ypa.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jgj.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://puq.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cmx.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cke.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cvn.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://diq.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ywe.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sop.sxryk.cn

[B02] 多分支 else if / elif
来源：http://djf.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mzm.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://quk.jyoumei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygd.havefunace.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyh.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltv.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://usp.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ecu.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ccq.fengsongda.top

[B03] switch / match / case
来源：http://alt.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lnf.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fzi.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kqn.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fny.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://far.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://czl.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mxj.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jlm.xuetiantiany.cn

[B04] for 计数循环
来源：http://jba.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://ceq.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cki.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://weh.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pxy.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://riq.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ntm.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://gsu.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nsl.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://zfl.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://eej.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lui.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fvv.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://hcf.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://leq.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://roc.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://lpc.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kqo.yj202588.top

[B06] 遍历字典 / 对象
来源：http://kmf.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mnq.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://itw.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pcg.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://krw.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aqy.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zhw.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lik.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tzl.wangdashe.top

[B07] while 循环
来源：http://ppo.hcnkem.com

Py:   while i < 10: i += 1
来源：http://iaq.shanyushiyangtech.top


<!-- 参考信息 -->