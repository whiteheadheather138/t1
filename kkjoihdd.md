代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://xyk.shangyingyoupin.top

[A03] 常量定义
来源：http://tfc.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oqu.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://zwf.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://olb.ywan-chungtsiang.top

TS:   const PI: number = 3.14159;
来源：http://bag.hammf.cn

Java: static final double PI = 3.14159;
来源：http://oyq.yueranfly.top

Go:   const PI = 3.14159
来源：http://msd.zhijiandao.cn

Ruby: PI = 3.14159
来源：http://hdz.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://hnl.ehwqpu.com

[A04] 判断变量类型
来源：http://efl.yj20258.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fjz.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mfa.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zpi.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://pwe.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://thk.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://qrv.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kkm.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://yrl.ybcxt.top

[A05] 整数除法与取模
来源：http://exb.xylfe.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://chu.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://kxc.uphjek.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fsc.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jct.jianghu66.top

Java: 7 / 2; 7 % 2
来源：http://maa.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://lfl.hammf.cn

Ruby: 7 / 2; 7 % 2
来源：http://mzm.sufxvd.cn

C#:   7 / 2; 7 % 2
来源：http://vut.zhixingplan.top

[A06] 字符串转数字
来源：http://dgs.feifeiyinyue.top

Py:   int("42"); float("3.14")
来源：http://wfs.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cgd.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lac.epnwcf.com

TS:   parseInt("42", 10); Number("42")
来源：http://flb.zdqjudy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://llp.uphjek.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hlc.0kj1m.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://goy.xylfe.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cfz.ywan-chungtsiang.top

[A07] 数字转字符串
来源：http://uyi.kuanghao11.cn

Py:   str(42)
来源：http://edj.hnqzz.top

PHP:  (string) 42; strval(42)
来源：http://blt.yuxming.cn

JS:   String(42); (42).toString()
来源：http://skn.jiagoushi.top

TS:   String(42)
来源：http://njo.fengsongda.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://owt.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://hem.andypj.xyz

Ruby: 42.to_s
来源：http://toa.havefunace.top

C#:   42.ToString()
来源：http://ejr.epnwcf.com

[A08] 取整与四舍五入
来源：http://dxn.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hhe.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qpc.jlsjyb.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bqx.cashguo.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zbi.aibaodan.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://plt.zhijiandao.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yku.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nbl.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://utw.yj202588.top

[A09] 绝对值与最大最小值
来源：http://ess.hysaishi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lhn.haohaochexian.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iyc.sjlbkw.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://okz.xingfuxueyuan.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://flf.redwolf501.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ajf.haohaochexian.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ntu.ydjk.org.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qfl.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gkw.zdqjudy.top

[A10] 生成随机数
来源：http://ktl.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://hgu.sweek.top

PHP:  random_int(1, 100);
来源：http://dni.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ptl.zhongyouzk.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://coo.bbcook.cn

Java: new Random().nextInt(100) + 1
来源：http://qcn.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ehu.aizwys.cn

Ruby: rand(1..100)
来源：http://jwp.kuanghao11.cn

C#:   new Random().Next(1, 101)
来源：http://bbi.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://tlx.pengpengdd.cyou

Py:   "yes" if x > 0 else "no"
来源：http://rei.316326.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://tsc.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://zbr.guannengcc.top

TS:   x > 0 ? "yes" : "no"
来源：http://aze.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://bdh.dashuyun.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tqj.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bgp.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rxe.ppjwa.cn

[A12] 字符串插值 / 格式化
来源：http://sfb.xziqi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lfr.tarul.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kwb.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://fmq.tian-w.cn

TS:   `Hello, ${name}!`
来源：http://lxx.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://rzx.vehdjk.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cks.havefunace.top

Ruby: "Hello, #{name}!"
来源：http://jxd.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://uym.cdnleiting.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yct.guannengcc.top

Py:   "第一行\n第二行"
来源：http://hjb.ywan-chungtsiang.top

PHP:  "第一行\n第二行"
来源：http://lte.guannengcc.top

JS:   "第一行\n第二行"
来源：http://kqv.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://uds.hysaishi.cn

Java: "第一行\n第二行"
来源：http://dcw.cheryme.top

Go:   "第一行\n第二行"
来源：http://jun.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://kwv.guannengcc.top

C#:   "第一行\n第二行"
来源：http://knh.cheryme.top

[A14] 注释写法
来源：http://its.xinyue.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://gtw.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fpu.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://yjv.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://hlm.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://otb.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://gkz.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://kya.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://rny.guannengcc.top

[A15] 空值判断与默认值
来源：http://upl.birdmap.top

Py:   value = data or "默认值"
来源：http://zzk.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://ahj.chenjidiqi.icu

JS:   const value = data ?? "默认值";
来源：http://epm.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://xkt.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://obf.fktsv.cn

Go:   if data == "" { data = "默认值" }
来源：http://equ.sxryk.cn

Ruby: value = data || "默认值"
来源：http://gtc.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://sxz.yj202588.top

[A16] 真假值判断规则
来源：http://wbh.tanke756.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tsa.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ucy.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jsn.sweek.top

TS:   if (!x) {}
来源：http://sxo.epnwcf.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://grs.hnqzz.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jdo.hywenlv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tbk.havefunace.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jxk.daria6918.cn

[A17] 位运算
来源：http://dxy.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xtm.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oks.zycfv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pmz.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hqw.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://frq.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wrd.cheryme.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvz.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ryb.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://jfk.iojbl.cn

Py:   ord("A"); chr(65)
来源：http://fko.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://ppa.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cvn.zhixingplan.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://max.chenlongwang.top

Java: (int) 'A'; (char) 65
来源：http://typ.xingfuxueyuan.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lgm.tian-w.cn

Ruby: "A".ord; 65.chr
来源：http://wny.hongshengwenyu.top

C#:   (int)'A'; (char)65
来源：http://rum.yj202588.top

[A19] 交换两个变量
来源：http://wyu.daxiang520.top

Py:   a, b = b, a
来源：http://gun.smart0.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://zcg.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://oou.pycfn.com

TS:   [a, b] = [b, a];
来源：http://ixw.hnxiangtu.top

Java: int t = a; a = b; b = t;
来源：http://fwz.316326.xyz

Go:   a, b = b, a
来源：http://hal.jyoumei.cn

Ruby: a, b = b, a
来源：http://tkf.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://ntt.yanxiufei.cn

[A20] 读取标准输入
来源：http://qtf.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://vyx.hnxiangtu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vie.hysaishi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://brv.pycfn.com

TS:   // Node.js：readline 模块
来源：http://jib.xuetiantiany.cn

Java: new Scanner(System.in).nextLine()
来源：http://ers.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yun.quarkkingdee.top

Ruby: gets.chomp
来源：http://jfk.52xcode.cn

C#:   Console.ReadLine();
来源：http://ovk.redwolf501.top

[A21] 保留指定小数位输出
来源：http://vxt.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://chu.tian-w.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xfw.dashuyun.cn

JS:   (3.14159).toFixed(2)
来源：http://djx.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://qen.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://jtd.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vva.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://avx.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://fnn.feifeiyinyue.top

[A22] 获取字符串长度
来源：http://uwb.wangshuangyany.cn

Py:   len(s)
来源：http://rhg.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://elp.hnqzz.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eut.xuetiantiany.cn

TS:   s.length
来源：http://mcg.hesvh.cn

Java: s.length()
来源：http://xtl.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jth.mhx1999.top

Ruby: s.length
来源：http://aww.yj20258888.top

C#:   s.Length
来源：http://wgs.hfpthk.cn

[A23] 大小写转换
来源：http://svp.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ray.ctjpmb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yeo.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://euo.vqdsnc.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lcj.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gxr.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hhb.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fkl.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mrh.hesvh.cn

[A24] 去除首尾空白
来源：http://qdg.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lnd.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cci.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lkm.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vyz.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nxi.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://ayq.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jzx.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zhq.shzxlz.cn

[A25] 字符串比较
来源：http://foz.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://uyz.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lci.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ojv.cheryme.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zoh.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xkk.pengpengdd.cyou

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qld.bjfxy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bem.feifeiyinyue.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fjk.ctjpmb.com

[A26] 类型转换总览
来源：http://qdg.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ext.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uks.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pxl.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://zgx.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yrx.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rdd.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aha.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hjy.zhoulong.xyz

================================================================================
来源：http://ukh.kuanghao11.cn

B. 流程控制
来源：http://ylj.hammf.cn

================================================================================
来源：http://bsm.cheryme.top

[B01] 条件判断 if / else
来源：http://izy.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zbf.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ecv.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rfr.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fnu.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cto.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gek.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nmf.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vtk.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://ils.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kor.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ekd.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://woa.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbd.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pev.chenlongwang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tys.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hnl.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckg.jqgfzy.top

[B03] switch / match / case
来源：http://egu.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sey.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gmo.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://had.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zoc.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://egf.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://axz.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nok.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qwd.hcnkem.com

[B04] for 计数循环
来源：http://rfl.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://qlu.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mxr.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dpn.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dca.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aed.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xfm.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://xem.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dpm.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://gpf.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://sbs.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bsl.ehwqpu.com

JS:   for (const item of arr) { console.log(item); }
来源：http://qri.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tui.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jcy.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mev.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://zln.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eea.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://swr.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kwc.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mca.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kkx.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pdn.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bfc.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lft.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xog.tianlin.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wtk.shanyushiyangtech.top

[B07] while 循环
来源：http://tmw.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://roi.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://hgh.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://hwr.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://jos.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://lxa.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lpq.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://tdz.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://rkf.smart0.xyz

[B08] do-while（至少执行一次）
来源：http://vjq.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://lvk.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mju.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://boq.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://qmp.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://phi.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mrp.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://hgu.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://ntd.gogol.net.cn

[B09] break 与 continue
来源：http://cha.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bwd.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wyu.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmn.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fad.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdp.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tfw.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://spv.ctjpmb.com


<!-- 参考信息 -->