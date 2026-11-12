代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://ihe.zhoulong.xyz

[A03] 常量定义
来源：http://anf.shanyushiyangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://awq.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://dbr.tarul.cn

JS:   const PI = 3.14159;
来源：http://jjk.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://xhn.jlsjyb.cn

Java: static final double PI = 3.14159;
来源：http://hcw.fengsongda.top

Go:   const PI = 3.14159
来源：http://xzy.shanyushiyangkeji.top

Ruby: PI = 3.14159
来源：http://zri.zhoulong.xyz

C#:   const double PI = 3.14159;
来源：http://wui.tarul.cn

[A04] 判断变量类型
来源：http://gai.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://avg.jyoumei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lsc.dianchejie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nlc.zdqjudy.top

TS:   typeof x; x instanceof Date
来源：http://yga.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tid.hnxiangtu.top

Go:   reflect.TypeOf(x).Name()
来源：http://uic.wangshuangyany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lya.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://ags.haohaochexian.top

[A05] 整数除法与取模
来源：http://jbs.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cwa.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xpj.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uht.xuetiantiany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ilz.andypj.xyz

Java: 7 / 2; 7 % 2
来源：http://gok.tarul.cn

Go:   7 / 2; 7 % 2
来源：http://gvh.yongpay.top

Ruby: 7 / 2; 7 % 2
来源：http://yhz.jinghuilouyu.cn

C#:   7 / 2; 7 % 2
来源：http://xyk.xuanzx.com

[A06] 字符串转数字
来源：http://apu.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://gcj.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dmr.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iom.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://ahg.yueranfly.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ndz.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gsd.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ymn.zhijiandao.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yog.tarul.cn

[A07] 数字转字符串
来源：http://jao.hnqzz.top

Py:   str(42)
来源：http://aaf.yvedp.cn

PHP:  (string) 42; strval(42)
来源：http://tld.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://exv.jiagoushi.top

TS:   String(42)
来源：http://ilh.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://akl.jyoumei.cn

Go:   strconv.Itoa(42)
来源：http://mvf.ydjk.org.cn

Ruby: 42.to_s
来源：http://ukr.jinqigfzy.top

C#:   42.ToString()
来源：http://pfh.yj20258888.top

[A08] 取整与四舍五入
来源：http://sxt.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bfl.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xro.jlsjyb.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yup.fengsongda.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ngb.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sjv.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gba.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fqo.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kmn.cashguo.top

[A09] 绝对值与最大最小值
来源：http://xlh.meibo888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ccz.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nxe.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mqg.nwbrower.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tfs.fengsongda.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hqc.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nip.zhongyouzk.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xda.andypj.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ndn.yvedp.cn

[A10] 生成随机数
来源：http://cqq.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://cii.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://pdu.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kiz.tianlin.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wne.yuanzhike.top

Java: new Random().nextInt(100) + 1
来源：http://kdi.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vow.svipenyu.cn

Ruby: rand(1..100)
来源：http://fmq.ctjpmb.com

C#:   new Random().Next(1, 101)
来源：http://uth.vehdjk.com

[A11] 条件表达式（三元）
来源：http://ptf.hongshengwenyu.top

Py:   "yes" if x > 0 else "no"
来源：http://wug.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zas.shanyushiyangtech.top

JS:   x > 0 ? "yes" : "no"
来源：http://fyr.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://xdt.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://tmq.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ufc.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ysb.jyoumei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vzt.sweek.top

[A12] 字符串插值 / 格式化
来源：http://lkj.ctjpmb.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mdl.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kkk.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://hcz.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://fnv.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://asd.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ktr.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://kxc.cqqwz.cn

C#:   $"Hello, {name}!"
来源：http://new.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://noq.cheryme.top

Py:   "第一行\n第二行"
来源：http://boo.kuanghao11.cn

PHP:  "第一行\n第二行"
来源：http://ume.shuidangran.top

JS:   "第一行\n第二行"
来源：http://npf.snrcjt.cn

TS:   "第一行\n第二行"
来源：http://kdk.ywan-chungtsiang.top

Java: "第一行\n第二行"
来源：http://rso.kuanghao11.cn

Go:   "第一行\n第二行"
来源：http://xzs.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://ffa.birdmap.top

C#:   "第一行\n第二行"
来源：http://kug.sjlbkw.cn

[A14] 注释写法
来源：http://qbq.hnqzz.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kmd.jlsjyb.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://djx.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://oaw.zhengqikj.top

TS:   // 单行；/* 多行 */
来源：http://ihl.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ytf.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://ofq.daria6918.cn

Ruby: # 单行；=begin 多行 =end
来源：http://les.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://ult.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://dpc.chenjidiqi.icu

Py:   value = data or "默认值"
来源：http://kjm.hfpthk.cn

PHP:  $value = $data ?? "默认值";
来源：http://tzi.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://cdz.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://nsr.fanxiaobao.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dwq.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://lso.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://onn.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://hvs.redwolf501.top

[A16] 真假值判断规则
来源：http://zlq.zycfv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tcl.cashguo.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pio.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dqo.birdmap.top

TS:   if (!x) {}
来源：http://rak.yuanzhike.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oiv.zhongyouzk.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aqb.gotoacloud.top

Ruby: unless x            # nil 与 false 为假
来源：http://yvn.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://anx.nwbrower.top

[A17] 位运算
来源：http://ihu.jlsjyb.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzr.nanxuanxn.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cxj.dashuyun.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovy.jyoumei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://erb.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://emj.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xmj.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cnd.ydjk.org.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssv.pengpengdd.cyou

[A18] 字符与 ASCII 码互转
来源：http://nkr.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://mko.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://zah.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ebd.zdqjudy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ubl.cashguo.top

Java: (int) 'A'; (char) 65
来源：http://aay.quarkkingdee.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nmq.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://ahp.yj20258888.top

C#:   (int)'A'; (char)65
来源：http://dfu.vehdjk.com

[A19] 交换两个变量
来源：http://tpf.shzxlz.cn

Py:   a, b = b, a
来源：http://oyf.fengsongda.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nan.zdqjudy.top

JS:   [a, b] = [b, a];
来源：http://vyl.sweek.top

TS:   [a, b] = [b, a];
来源：http://wgh.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://req.fzhhl.top

Go:   a, b = b, a
来源：http://srl.aizwys.cn

Ruby: a, b = b, a
来源：http://amm.316326.xyz

C#:   (a, b) = (b, a);
来源：http://cni.wangshuangyany.cn

[A20] 读取标准输入
来源：http://swy.birdmap.top

Py:   name = input("请输入：")
来源：http://dqn.sweek.top

PHP:  $name = trim(fgets(STDIN));
来源：http://agi.nwbrower.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xrz.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://asa.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://nuy.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tll.snrcjt.cn

Ruby: gets.chomp
来源：http://ldy.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://eeu.52xcode.cn

[A21] 保留指定小数位输出
来源：http://tud.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://qog.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kyg.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://epq.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://buu.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://hgy.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nbc.xziqi.cn

Ruby: format("%.2f", 3.14159)
来源：http://aqt.chenlongwang.top

C#:   3.14159.ToString("F2")
来源：http://lfi.sxryk.cn

[A22] 获取字符串长度
来源：http://jwj.gogol.net.cn

Py:   len(s)
来源：http://gxl.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zxt.ydzc1.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://laz.zhijiandao.cn

TS:   s.length
来源：http://jnr.xingfuxueyuan.xyz

Java: s.length()
来源：http://ohz.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kjo.jiagoushi.top

Ruby: s.length
来源：http://uys.cheryme.top

C#:   s.Length
来源：http://apd.0kj1m.cn

[A23] 大小写转换
来源：http://scl.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://byu.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ciu.shuidangran.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xof.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bpz.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dtd.hnqzz.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iry.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wcd.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xkx.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://orh.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bxu.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tag.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lrk.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://syw.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xzh.gaohongyu789.top

Go:   strings.TrimSpace(s)
来源：http://erm.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uxp.jinqigufen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nss.zhiwuduotai.top

[A25] 字符串比较
来源：http://lpu.yuanzhike.top

Py:   s1 == s2; s1 != s2
来源：http://duw.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://loo.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://etq.iojbl.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kov.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vbv.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ibi.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vlp.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hsp.yangfankeji.com

[A26] 类型转换总览
来源：http://qsg.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hwx.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://czg.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kpm.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://wox.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oig.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://obt.epnwcf.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xto.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hfq.daxiang520.top

================================================================================
来源：http://osc.xylfe.cn

B. 流程控制
来源：http://ols.ydjk.org.cn

================================================================================
来源：http://mcr.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://uim.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://akt.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mau.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://idc.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wil.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uhn.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gzp.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mhv.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://prc.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://ocf.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://obn.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://esn.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lii.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwl.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkl.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kwe.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xkc.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kgz.xuetiantiany.cn

[B03] switch / match / case
来源：http://yxo.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qra.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xhb.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ldq.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://atd.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ooy.316326.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oye.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xxl.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rnt.cheryme.top

[B04] for 计数循环
来源：http://twz.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://kwk.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tfm.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zws.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xpp.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://drz.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mwe.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://elb.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wag.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://hey.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://swc.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cpy.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rpb.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://lzs.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mdq.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eme.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://tkt.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jgc.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://ysd.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yzm.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xnt.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rmo.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rfj.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lig.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wfc.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mrq.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dpc.birdmap.top

[B07] while 循环
来源：http://tzc.bjfxy.top

Py:   while i < 10: i += 1
来源：http://gyd.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kdm.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://ghz.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://lsy.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://zot.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vsl.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://nim.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://fqe.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://ntx.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://lfa.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tkd.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://gtl.jinghuilouyu.cn

TS:   do { i++; } while (i < 10);
来源：http://clm.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://unp.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mzy.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://whz.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://zvt.fengsongda.top

[B09] break 与 continue
来源：http://hwy.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kco.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cco.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tfq.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hat.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrd.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ita.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://toz.zhaomingkeji.xyz


<!-- 参考信息 -->