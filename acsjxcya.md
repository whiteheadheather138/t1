代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://umm.gzhubu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zfl.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dnu.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hlr.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wra.shzxlz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ott.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zkn.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kzg.sjlbkw.cn

================================================================================
来源：http://tkz.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://wfm.svipenyu.cn

================================================================================
来源：http://rba.ehwqpu.com

[A01] Hello World
来源：http://whk.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://jwf.316326.xyz

PHP:  echo "Hello, World!";
来源：http://nif.hammf.cn

JS:   console.log("Hello, World!");
来源：http://eoy.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wuc.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://ytv.uphjek.com

Go:   fmt.Println("Hello, World!")
来源：http://okn.yj20258888.top

Ruby: puts "Hello, World!"
来源：http://rzf.guannengcc.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fqn.jqgfzy.top

[A02] 变量声明与赋值
来源：http://mdj.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wji.hfpthk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gzd.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://fih.cdnleiting.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ngx.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://sbb.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://lrn.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://qqj.zhiwuduotai.top

C#:   string name = "Alex"; int age = 20;
来源：http://cxn.jinqigufen.top

[A03] 常量定义
来源：http://kvw.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://plz.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://ytp.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://wma.xylfe.cn

TS:   const PI: number = 3.14159;
来源：http://dul.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://yun.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://qvf.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://uju.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://wxq.xuanzx.com

[A04] 判断变量类型
来源：http://rfj.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ikl.tanke756.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blw.aibaodan.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xbt.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://fwo.wangshuangyany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zqf.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://qjv.bbcook.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gtx.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://oce.hcnkem.com

[A05] 整数除法与取模
来源：http://juf.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gns.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fqy.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ese.zhongyouzk.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gkg.birdmap.top

Java: 7 / 2; 7 % 2
来源：http://rjm.guowangkeji.top

Go:   7 / 2; 7 % 2
来源：http://ode.yj202588.top

Ruby: 7 / 2; 7 % 2
来源：http://kph.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://nbo.feifeiyinyue.top

[A06] 字符串转数字
来源：http://tgp.jinqigfzy.top

Py:   int("42"); float("3.14")
来源：http://ttk.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://flb.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gdk.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://rzg.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uif.hcnkem.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qbp.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kmi.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mhk.guowangkeji.top

[A07] 数字转字符串
来源：http://oay.guannengcc.top

Py:   str(42)
来源：http://xwl.epnwcf.com

PHP:  (string) 42; strval(42)
来源：http://guw.ydzc1.top

JS:   String(42); (42).toString()
来源：http://iry.ydjk.org.cn

TS:   String(42)
来源：http://opx.fengsongda.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hiy.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://ise.pengpengdd.cyou

Ruby: 42.to_s
来源：http://cow.dianchejie.cn

C#:   42.ToString()
来源：http://chn.yonumen.top

[A08] 取整与四舍五入
来源：http://jzf.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ywe.nanxuanxn.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hgg.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lmj.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xbz.tian-w.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://led.nanxuanxn.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qlr.yongpay.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zzf.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vie.xingfuxueyuan.xyz

[A09] 绝对值与最大最小值
来源：http://bsa.yuanzhike.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cqq.gotoacloud.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zmh.9152youxi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hds.tian-w.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mig.jqgfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vat.guowangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ekr.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iii.yj202588.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cti.0kj1m.cn

[A10] 生成随机数
来源：http://ebf.9152youxi.cn

Py:   import random; random.randint(1, 100)
来源：http://dar.birdmap.top

PHP:  random_int(1, 100);
来源：http://ezg.yj20258.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fpj.dianchejie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fni.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://cgf.hesvh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gxk.iojbl.cn

Ruby: rand(1..100)
来源：http://mki.daria6918.cn

C#:   new Random().Next(1, 101)
来源：http://amg.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://oub.guowangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://ikm.zhongyouzk.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ogk.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pot.xuetiantiany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lyd.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://rmr.sysykeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bvp.jinqigufen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://sor.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://nlf.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://bty.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://weh.aibaodan.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ruh.haohaochexian.top

JS:   `Hello, ${name}!`
来源：http://wel.jinqigufen.top

TS:   `Hello, ${name}!`
来源：http://tkh.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://mwc.mhx1999.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ooq.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://uku.snrcjt.cn

C#:   $"Hello, {name}!"
来源：http://uli.fktsv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rzd.meibo888.top

Py:   "第一行\n第二行"
来源：http://yfm.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://cmt.tarul.cn

JS:   "第一行\n第二行"
来源：http://xeb.ydjk.org.cn

TS:   "第一行\n第二行"
来源：http://nai.gzhubu.top

Java: "第一行\n第二行"
来源：http://tta.zycfv.cn

Go:   "第一行\n第二行"
来源：http://zxy.fanxiaobao.xyz

Ruby: "第一行\n第二行"
来源：http://mck.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://qum.ivvv.top

[A14] 注释写法
来源：http://xth.0kj1m.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jtm.iojbl.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://egp.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://gcm.zhaomingkeji.xyz

TS:   // 单行；/* 多行 */
来源：http://ftj.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jam.xingfuxueyuan.xyz

Go:   // 单行；/* 多行 */
来源：http://khd.wangshuangyany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hcm.daria6918.cn

C#:   // 单行；/* 多行 */
来源：http://qxa.sufxvd.cn

[A15] 空值判断与默认值
来源：http://liw.fzhhl.top

Py:   value = data or "默认值"
来源：http://pje.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://luo.ctjpmb.com

JS:   const value = data ?? "默认值";
来源：http://uqd.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://lty.zhaomingkeji.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iwo.zhongyouzk.top

Go:   if data == "" { data = "默认值" }
来源：http://kro.sysykeji.top

Ruby: value = data || "默认值"
来源：http://she.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://lcm.zhoulong.xyz

[A16] 真假值判断规则
来源：http://ulz.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mwg.yfazqb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fzd.birdmap.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jgy.ehwqpu.com

TS:   if (!x) {}
来源：http://hqb.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mjd.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://exm.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hao.wangdashe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bdm.yj202588.top

[A17] 位运算
来源：http://fcb.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sni.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sdj.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uhi.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sbn.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://okh.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pyq.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bms.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bjy.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://qrf.cdnleiting.top

Py:   ord("A"); chr(65)
来源：http://gsq.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://cgt.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uam.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qod.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://spi.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://snv.wangdashe.top

Ruby: "A".ord; 65.chr
来源：http://hom.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://tgh.fengsongda.top

[A19] 交换两个变量
来源：http://bpt.epnwcf.com

Py:   a, b = b, a
来源：http://ilq.hysaishi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fyc.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://byu.tarul.cn

TS:   [a, b] = [b, a];
来源：http://qil.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://xle.svipenyu.cn

Go:   a, b = b, a
来源：http://uaf.ivvv.top

Ruby: a, b = b, a
来源：http://kaw.yj20258.top

C#:   (a, b) = (b, a);
来源：http://vhf.cashguo.top

[A20] 读取标准输入
来源：http://eer.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://mqo.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ldw.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://efx.guowangkeji.top

TS:   // Node.js：readline 模块
来源：http://lki.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://ait.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://egy.zhaomingkeji.xyz

Ruby: gets.chomp
来源：http://tfx.zhengqikj.top

C#:   Console.ReadLine();
来源：http://bkx.jyoumei.cn

[A21] 保留指定小数位输出
来源：http://dyq.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://ytl.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oco.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://ngq.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://rbq.shanyushiyangtech.top

Java: String.format("%.2f", 3.14159)
来源：http://pjt.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hpa.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://llf.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://ykj.zhongyouzk.top

[A22] 获取字符串长度
来源：http://eqq.ppjwa.cn

Py:   len(s)
来源：http://rgn.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mdn.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qgy.gogol.net.cn

TS:   s.length
来源：http://adz.cashguo.top

Java: s.length()
来源：http://pgj.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tso.hysaishi.cn

Ruby: s.length
来源：http://wty.chenzaomai.com

C#:   s.Length
来源：http://oey.havefunace.top

[A23] 大小写转换
来源：http://lua.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zvb.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vfa.shuidangran.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yvu.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zsq.hywenlv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ksg.cashguo.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nqs.gzhubu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nsy.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xgg.yonumen.top

[A24] 去除首尾空白
来源：http://unf.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ezd.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cfm.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lar.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wtr.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ril.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://cas.xziqi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pha.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gbe.hnxiangtu.top

[A25] 字符串比较
来源：http://fpy.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://vot.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oxc.sufxvd.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lmn.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bdp.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wsd.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://udp.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aks.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fcb.hcnkem.com

[A26] 类型转换总览
来源：http://ziz.wangshuangyany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kst.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cnv.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qja.epnwcf.com

TS:   Number() String() Boolean() x as number
来源：http://udn.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lls.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bgj.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://etn.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xih.yonumen.top

================================================================================
来源：http://dnt.fzhhl.top

B. 流程控制
来源：http://cqh.shzxlz.cn

================================================================================
来源：http://bzm.fengsongda.top

[B01] 条件判断 if / else
来源：http://rty.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zrc.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wpq.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mgg.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ddt.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xqa.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baz.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cwy.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mdv.mhx1999.top

[B02] 多分支 else if / elif
来源：http://ktr.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ogh.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qcj.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpz.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emf.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mcf.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ufz.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zwo.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ssa.zdbjq.cn

[B03] switch / match / case
来源：http://muh.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bps.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rkn.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vlb.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bqt.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bie.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gxq.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xmj.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ivd.yj202588.top

[B04] for 计数循环
来源：http://ypv.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://ixc.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nrl.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kkn.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ozc.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uzw.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ohb.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://biy.zhengqikj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qlz.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://zwn.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://byn.ppjwa.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qdu.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fkx.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://shr.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://rse.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vil.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://mgu.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ltw.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://hpq.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://yuu.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yxb.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tje.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jqb.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dbz.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jtz.uphjek.com


<!-- 参考信息 -->