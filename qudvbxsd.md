代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://nwq.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://vag.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://uwk.guannengcc.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qfk.fktsv.cn

[A02] 变量声明与赋值
来源：http://rwi.aizwys.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gmo.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pyv.gaohongyu789.top

JS:   let name = "Alex"; const age = 20;
来源：http://mcd.yangfankeji.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mdx.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://fwc.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://rlv.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://iyo.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dlw.birdmap.top

[A03] 常量定义
来源：http://hhy.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ykd.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://evx.sjlbkw.cn

JS:   const PI = 3.14159;
来源：http://lrq.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://iit.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://otq.zhixingplan.top

Go:   const PI = 3.14159
来源：http://qmy.ctjpmb.com

Ruby: PI = 3.14159
来源：http://ioo.zhaomingkeji.xyz

C#:   const double PI = 3.14159;
来源：http://rwa.ybcxt.top

[A04] 判断变量类型
来源：http://bzj.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mxz.bjfxy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hfc.yuanzhike.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xdx.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://tcu.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ygp.wangdashe.top

Go:   reflect.TypeOf(x).Name()
来源：http://oxs.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://inx.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://ikp.sxryk.cn

[A05] 整数除法与取模
来源：http://sgg.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hmk.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dly.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://awy.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cvq.yj20258.top

Java: 7 / 2; 7 % 2
来源：http://fuo.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://ibs.ydjk.org.cn

Ruby: 7 / 2; 7 % 2
来源：http://kbw.uphjek.com

C#:   7 / 2; 7 % 2
来源：http://fke.gaohongyu789.top

[A06] 字符串转数字
来源：http://jud.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://ler.havefunace.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bpu.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mwb.hcnkem.com

TS:   parseInt("42", 10); Number("42")
来源：http://osi.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lcu.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gyf.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dwa.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sfj.yfazqb.com

[A07] 数字转字符串
来源：http://dlz.yj20258888.top

Py:   str(42)
来源：http://zkd.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://iyf.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://zpt.cdnleiting.top

TS:   String(42)
来源：http://uxx.hongshengwenyu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://skj.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://gde.shangyingyoupin.top

Ruby: 42.to_s
来源：http://hln.aizwys.cn

C#:   42.ToString()
来源：http://nkq.zhongyouzk.top

[A08] 取整与四舍五入
来源：http://fkd.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hrc.zhijiandao.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qfp.jyoumei.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fmy.yj20258888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zyi.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pdz.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yap.feifeiyinyue.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pno.havefunace.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eps.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://ufl.chenlongwang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tbf.yvedp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nnv.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lnm.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ysw.jiagoushi.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://akg.dianchejie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wqw.guowangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://asj.316326.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ocd.hesvh.cn

[A10] 生成随机数
来源：http://qsd.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://ame.yongpay.top

PHP:  random_int(1, 100);
来源：http://cdf.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bzp.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cue.wangdashe.top

Java: new Random().nextInt(100) + 1
来源：http://lrr.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ebh.kuanghao11.cn

Ruby: rand(1..100)
来源：http://ihh.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://yhr.mhx1999.top

[A11] 条件表达式（三元）
来源：http://tov.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://zzv.shzxlz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cyl.yvedp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eim.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://myb.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://chr.ehwqpu.com

Go:   // 无三元运算符，需用 if 语句
来源：http://egm.jinghuilouyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://syf.jlsjyb.cn

C#:   x > 0 ? "yes" : "no"
来源：http://swf.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://hmp.gzhubu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://msx.fktsv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jsh.ydzc1.top

JS:   `Hello, ${name}!`
来源：http://alq.hfpthk.cn

TS:   `Hello, ${name}!`
来源：http://awa.andypj.xyz

Java: "Hello, %s!".formatted(name)
来源：http://ezu.yonumen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jxr.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://qur.sjlbkw.cn

C#:   $"Hello, {name}!"
来源：http://gks.yj20258.top

[A13] 多行字符串（练习 \n 转义）
来源：http://iwo.yanxiufei.cn

Py:   "第一行\n第二行"
来源：http://sjp.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://ilk.zhongyouzk.top

JS:   "第一行\n第二行"
来源：http://eej.sxryk.cn

TS:   "第一行\n第二行"
来源：http://erf.hysaishi.cn

Java: "第一行\n第二行"
来源：http://fcy.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://ynj.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://fjm.zdqjudy.top

C#:   "第一行\n第二行"
来源：http://hgs.jiagoushi.top

[A14] 注释写法
来源：http://ifz.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ppc.mhx1999.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vsa.jqgufenzy.top

JS:   // 单行；/* 多行 */
来源：http://tgg.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://jsq.feifeiyinyue.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wex.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://tkh.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://rtx.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://eto.vehdjk.com

[A15] 空值判断与默认值
来源：http://nfy.0kj1m.cn

Py:   value = data or "默认值"
来源：http://clu.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://rly.xylfe.cn

JS:   const value = data ?? "默认值";
来源：http://tlt.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://ydh.yueranfly.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lip.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://nbd.jyoumei.cn

Ruby: value = data || "默认值"
来源：http://cil.shzxlz.cn

C#:   var value = data ?? "默认值";
来源：http://fui.cucudq.cn

[A16] 真假值判断规则
来源：http://dyb.cashguo.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mwa.haohaochexian.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kla.zhiwuduotai.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cvs.yuxming.cn

TS:   if (!x) {}
来源：http://qzs.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ydo.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hdw.sxryk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dve.hywenlv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aoe.wangdashe.top

[A17] 位运算
来源：http://kis.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rvv.yj20258.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ncq.yonumen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgg.yangfankeji.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uks.chenlongwang.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mox.hongshengwenyu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xpx.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfp.havefunace.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncg.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://bgg.jlsjyb.cn

Py:   ord("A"); chr(65)
来源：http://ayi.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://dpn.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lyo.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oju.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://scz.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://toe.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://alr.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://lms.andypj.xyz

[A19] 交换两个变量
来源：http://ase.jianghu66.top

Py:   a, b = b, a
来源：http://qmj.52xcode.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cme.yj202588.top

JS:   [a, b] = [b, a];
来源：http://cmd.kuanghao11.cn

TS:   [a, b] = [b, a];
来源：http://ueq.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://frp.hcnkem.com

Go:   a, b = b, a
来源：http://qsi.chenlongwang.top

Ruby: a, b = b, a
来源：http://qdc.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://vzp.iojbl.cn

[A20] 读取标准输入
来源：http://hdr.jinghuilouyu.cn

Py:   name = input("请输入：")
来源：http://rhx.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nfu.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://htu.aibaodan.cn

TS:   // Node.js：readline 模块
来源：http://dlk.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://kqv.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://knd.52xcode.cn

Ruby: gets.chomp
来源：http://ylo.sufxvd.cn

C#:   Console.ReadLine();
来源：http://dnx.hcnkem.com

[A21] 保留指定小数位输出
来源：http://zgi.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://vob.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tme.nwbrower.top

JS:   (3.14159).toFixed(2)
来源：http://yvw.yj20258888.top

TS:   (3.14159).toFixed(2)
来源：http://rwb.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://uhy.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eso.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://ljg.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://vlu.fktsv.cn

[A22] 获取字符串长度
来源：http://ben.zhongyouzk.top

Py:   len(s)
来源：http://lyw.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ioy.yonumen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vzn.vqdsnc.cn

TS:   s.length
来源：http://deb.andypj.xyz

Java: s.length()
来源：http://tsp.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mhy.zhiwuduotai.top

Ruby: s.length
来源：http://ivy.jinqigufen.top

C#:   s.Length
来源：http://msp.birdmap.top

[A23] 大小写转换
来源：http://qsw.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://uap.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://avj.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zkl.yj20258.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pdc.vehdjk.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mps.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://klu.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gzu.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jhl.yanxiufei.cn

[A24] 去除首尾空白
来源：http://xhz.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tmj.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uhi.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gpf.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://orx.0kj1m.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ssh.tianlin.xyz

Go:   strings.TrimSpace(s)
来源：http://uro.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mbj.yuxming.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xhi.haohaochexian.top

[A25] 字符串比较
来源：http://brl.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://mpm.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xvc.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fme.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://noc.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://svp.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mvo.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://sdu.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xie.chenlongwang.top

[A26] 类型转换总览
来源：http://vzt.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sir.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ezd.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nei.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://tns.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hpv.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yph.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://taw.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bga.chenjidiqi.icu

================================================================================
来源：http://tkq.zhongyouzk.top

B. 流程控制
来源：http://oeh.shanyushiyangtech.top

================================================================================
来源：http://vav.hammf.cn

[B01] 条件判断 if / else
来源：http://dry.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://dna.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cvu.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xas.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vnb.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://avc.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wby.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wju.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hau.yj20258.top

[B02] 多分支 else if / elif
来源：http://qfq.yj20258.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kfr.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xoj.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdh.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swo.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gkf.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yeu.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xri.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fnh.yj202588.top

[B03] switch / match / case
来源：http://lmi.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bzq.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dul.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lrz.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wgq.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kgb.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qxn.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ghh.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pte.nanxuanxn.top

[B04] for 计数循环
来源：http://ypb.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://rez.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jnv.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vbc.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofl.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qno.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qay.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://osr.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qil.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://umb.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://xkc.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gel.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yhn.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bya.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jzi.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tcn.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://ijb.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pac.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://fia.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zik.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jdg.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ghf.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://exj.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ntw.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hsh.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gve.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bie.shzxlz.cn

[B07] while 循环
来源：http://ljn.xylfe.cn

Py:   while i < 10: i += 1
来源：http://ret.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://csf.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://aby.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://gly.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://ovx.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vwg.jqgfzy.top

Ruby: while i < 10; i += 1; end
来源：http://xuk.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://tnp.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://dxh.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://obk.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uxg.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://zbg.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://uti.9152youxi.cn


<!-- 参考信息 -->