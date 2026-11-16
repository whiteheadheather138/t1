代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://tyw.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zcd.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cuk.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mnl.fktsv.cn

================================================================================
来源：http://qts.gogol.net.cn

A. 基础语法与类型
来源：http://rpp.chenlongwang.top

================================================================================
来源：http://ral.chenzaomai.com

[A01] Hello World
来源：http://klm.jqgfzy.top

Py:   print("Hello, World!")
来源：http://mfb.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://dxn.tarul.cn

JS:   console.log("Hello, World!");
来源：http://wds.svipenyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wfp.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://fkl.jiagoushi.top

Go:   fmt.Println("Hello, World!")
来源：http://kep.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://htm.zhoulong.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ikx.ybcxt.top

[A02] 变量声明与赋值
来源：http://oex.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qic.jianghu66.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zzj.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://pdf.hcnkem.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ads.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://ybh.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://ear.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://fdb.wangdashe.top

C#:   string name = "Alex"; int age = 20;
来源：http://uau.yj20258888.top

[A03] 常量定义
来源：http://qhr.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ndm.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://bpy.cheryme.top

JS:   const PI = 3.14159;
来源：http://qla.cqqwz.cn

TS:   const PI: number = 3.14159;
来源：http://thi.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://sni.birdmap.top

Go:   const PI = 3.14159
来源：http://mwu.0kj1m.cn

Ruby: PI = 3.14159
来源：http://bbs.316326.xyz

C#:   const double PI = 3.14159;
来源：http://qbw.hywenlv.cn

[A04] 判断变量类型
来源：http://twt.yvedp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vao.redwolf501.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ldi.snrcjt.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://syx.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://gmo.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rfa.andypj.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://yjb.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yem.jiagoushi.top

C#:   x.GetType().Name; x is int
来源：http://sli.vehdjk.com

[A05] 整数除法与取模
来源：http://eyb.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mbs.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://zdc.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://txd.quarkkingdee.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dkb.shuidangran.top

Java: 7 / 2; 7 % 2
来源：http://aky.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://hds.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://nxm.gotoacloud.top

C#:   7 / 2; 7 % 2
来源：http://fhp.wangshuangyany.cn

[A06] 字符串转数字
来源：http://wlo.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://zyt.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mxn.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yzn.shanyushiyangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://bzj.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jsv.meibo888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kvx.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xni.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zmf.meibo888.top

[A07] 数字转字符串
来源：http://nzz.haohaochexian.top

Py:   str(42)
来源：http://ifa.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://zik.jqgfzy.top

JS:   String(42); (42).toString()
来源：http://xya.nanxuanxn.top

TS:   String(42)
来源：http://frj.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jdr.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://igh.ydjk.org.cn

Ruby: 42.to_s
来源：http://yzx.gaohongyu789.top

C#:   42.ToString()
来源：http://urh.yuxming.cn

[A08] 取整与四舍五入
来源：http://jrw.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://knm.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dlr.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kai.yuxming.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cqn.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dyh.wangshuangyany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xhd.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mln.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ivs.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://wrp.chenjidiqi.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://owr.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zik.ehwqpu.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dnm.chenlongwang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vgf.xuetiantiany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zyb.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bpp.jinyuanbaomall.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bes.feifeiyinyue.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kqa.hcnkem.com

[A10] 生成随机数
来源：http://bgg.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://exb.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://zxk.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rfa.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tix.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://ght.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://foj.hnxiangtu.top

Ruby: rand(1..100)
来源：http://yib.shuidangran.top

C#:   new Random().Next(1, 101)
来源：http://rkn.nanxuanxn.top

[A11] 条件表达式（三元）
来源：http://xyj.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://hnw.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dgx.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yvv.sweek.top

TS:   x > 0 ? "yes" : "no"
来源：http://gck.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://rph.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uke.gaohongyu789.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bsl.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://fts.sweek.top

[A12] 字符串插值 / 格式化
来源：http://xna.gzhubu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lcx.chenlongwang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bde.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://puw.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://rsm.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://cmq.chenlongwang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ohd.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://qax.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://upl.hcnkem.com

[A13] 多行字符串（练习 \n 转义）
来源：http://nct.yfazqb.com

Py:   "第一行\n第二行"
来源：http://hte.tianlin.xyz

PHP:  "第一行\n第二行"
来源：http://mzm.hnqzz.top

JS:   "第一行\n第二行"
来源：http://sge.cdnleiting.top

TS:   "第一行\n第二行"
来源：http://jex.redwolf501.top

Java: "第一行\n第二行"
来源：http://jgp.cdnleiting.top

Go:   "第一行\n第二行"
来源：http://kpj.sxryk.cn

Ruby: "第一行\n第二行"
来源：http://ieu.svipenyu.cn

C#:   "第一行\n第二行"
来源：http://ymd.haohaochexian.top

[A14] 注释写法
来源：http://ats.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rag.shzxlz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nmc.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://zzd.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://xdz.yfazqb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fwo.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://cxo.cheryme.top

Ruby: # 单行；=begin 多行 =end
来源：http://gir.gogol.net.cn

C#:   // 单行；/* 多行 */
来源：http://xxe.yangfankeji.com

[A15] 空值判断与默认值
来源：http://xje.tarul.cn

Py:   value = data or "默认值"
来源：http://fwo.hnxiangtu.top

PHP:  $value = $data ?? "默认值";
来源：http://xml.meibo888.top

JS:   const value = data ?? "默认值";
来源：http://ihh.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://gek.zycfv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eyz.ehwqpu.com

Go:   if data == "" { data = "默认值" }
来源：http://car.xylfe.cn

Ruby: value = data || "默认值"
来源：http://pvz.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://kmb.fzhhl.top

[A16] 真假值判断规则
来源：http://mgz.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mzv.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ssi.jqgufenzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zmw.316326.xyz

TS:   if (!x) {}
来源：http://jcr.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ure.wangdashe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fjq.havefunace.top

Ruby: unless x            # nil 与 false 为假
来源：http://zhe.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tep.pycfn.com

[A17] 位运算
来源：http://rsa.hywenlv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hqr.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dgz.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rlp.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xfq.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyg.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hyn.shanyushiyangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ugc.ppjwa.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://guk.bbcook.cn

[A18] 字符与 ASCII 码互转
来源：http://zqm.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://umx.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://auk.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dwk.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gkc.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://jnp.ybcxt.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://inm.sysykeji.top

Ruby: "A".ord; 65.chr
来源：http://qmj.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://dov.yj20258888.top

[A19] 交换两个变量
来源：http://cjk.tarul.cn

Py:   a, b = b, a
来源：http://gci.xingfuxueyuan.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://ydu.shuidangran.top

JS:   [a, b] = [b, a];
来源：http://etq.yangfankeji.com

TS:   [a, b] = [b, a];
来源：http://ocm.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://pek.sufxvd.cn

Go:   a, b = b, a
来源：http://led.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://ova.nanxinkj.top

C#:   (a, b) = (b, a);
来源：http://zxv.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://ozk.0kj1m.cn

Py:   name = input("请输入：")
来源：http://jmc.chenzaomai.com

PHP:  $name = trim(fgets(STDIN));
来源：http://azx.shanyushiyangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xcs.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://okb.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://hjk.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jfw.redwolf501.top

Ruby: gets.chomp
来源：http://ksv.9152youxi.cn

C#:   Console.ReadLine();
来源：http://lmr.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://ytn.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://gtj.ivvv.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wvl.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://fjf.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://nut.guannengcc.top

Java: String.format("%.2f", 3.14159)
来源：http://vxd.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://atr.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://oly.chenlongwang.top

C#:   3.14159.ToString("F2")
来源：http://hic.gaohongyu789.top

[A22] 获取字符串长度
来源：http://mtv.zhijiandao.cn

Py:   len(s)
来源：http://iqz.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hmp.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wzw.jqgfzy.top

TS:   s.length
来源：http://qkv.hcnkem.com

Java: s.length()
来源：http://bnh.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cjz.haohaochexian.top

Ruby: s.length
来源：http://qfl.0kj1m.cn

C#:   s.Length
来源：http://etj.ivvv.top

[A23] 大小写转换
来源：http://lvg.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zry.ctjpmb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bdb.zdqjudy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tsl.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://soe.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ujf.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kvy.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rff.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lxz.yuxming.cn

[A24] 去除首尾空白
来源：http://dea.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iuc.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oaw.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://smj.daria6918.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rwe.yuanzhike.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xog.jinghuilouyu.cn

Go:   strings.TrimSpace(s)
来源：http://ldh.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://omx.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ify.dashuyun.cn

[A25] 字符串比较
来源：http://bdv.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://hue.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gcy.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mzf.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://svf.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rue.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cwu.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fxs.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cxj.zdbjq.cn

[A26] 类型转换总览
来源：http://mpc.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jpn.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aaj.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ixj.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://hhc.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://trk.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tsq.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mlj.fanxiaobao.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xsi.wangshuangyany.cn

================================================================================
来源：http://pzd.aizwys.cn

B. 流程控制
来源：http://gav.shzxlz.cn

================================================================================
来源：http://wks.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://kme.chenlongwang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ukd.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uyx.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bug.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://une.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jmy.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ghe.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mlh.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ktx.zdbjq.cn

[B02] 多分支 else if / elif
来源：http://qpp.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://enx.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ufp.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rey.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfg.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjv.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bsh.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uiu.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntx.wangshuangyany.cn

[B03] switch / match / case
来源：http://ure.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eys.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tam.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mfv.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pvh.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://waj.shanyushiyangtech.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pbj.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ewt.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fer.yvedp.cn

[B04] for 计数循环
来源：http://hgc.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://bqk.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nsr.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfz.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ieu.sysykeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://riu.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://htk.0kj1m.cn

Ruby: 10.times { |i| puts i }
来源：http://xni.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fwv.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://pox.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://trj.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://svp.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://thx.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://drf.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tap.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://adz.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://tqb.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hza.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://osx.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://swd.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zuk.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://luy.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zyp.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dow.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eii.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ypz.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lzu.vqdsnc.cn

[B07] while 循环
来源：http://zea.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://spf.hnxiangtu.top


<!-- 参考信息 -->