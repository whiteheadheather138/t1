代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://kgq.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gmc.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gvd.sufxvd.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bkx.wangshuangyany.cn

================================================================================
来源：http://dev.vehdjk.com

A. 基础语法与类型
来源：http://oax.cqqwz.cn

================================================================================
来源：http://aph.tian-w.cn

[A01] Hello World
来源：http://tql.yj20258888.top

Py:   print("Hello, World!")
来源：http://jvt.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://asf.yanxiufei.cn

JS:   console.log("Hello, World!");
来源：http://svq.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vmj.dashuyun.cn

Java: System.out.println("Hello, World!");
来源：http://equ.zhijiandao.cn

Go:   fmt.Println("Hello, World!")
来源：http://vyn.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://nop.jqgufenzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kmq.ivvv.top

[A02] 变量声明与赋值
来源：http://omn.yj202588.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tmg.xuanzx.com

PHP:  $name = "Alex"; $age = 20;
来源：http://lkx.ppjwa.cn

JS:   let name = "Alex"; const age = 20;
来源：http://aaw.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zlk.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://rcd.cashguo.top

Go:   name := "Alex"; age := 20
来源：http://eba.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://khu.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://yvi.yuxming.cn

[A03] 常量定义
来源：http://xvw.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ccc.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://vwy.xylfe.cn

JS:   const PI = 3.14159;
来源：http://gbe.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://vfg.cheryme.top

Java: static final double PI = 3.14159;
来源：http://xlu.hammf.cn

Go:   const PI = 3.14159
来源：http://rxr.guannengcc.top

Ruby: PI = 3.14159
来源：http://mzh.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://fsg.316326.xyz

[A04] 判断变量类型
来源：http://axb.iojbl.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jdf.shuidangran.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://llv.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://edl.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://oxi.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nqo.c1oappe.top

Go:   reflect.TypeOf(x).Name()
来源：http://ure.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ogj.xylfe.cn

C#:   x.GetType().Name; x is int
来源：http://phz.epnwcf.com

[A05] 整数除法与取模
来源：http://bzm.yuanzhike.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pum.snrcjt.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://txo.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://swm.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ila.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://cqp.ppjwa.cn

Go:   7 / 2; 7 % 2
来源：http://pic.iojbl.cn

Ruby: 7 / 2; 7 % 2
来源：http://bbl.yangfankeji.com

C#:   7 / 2; 7 % 2
来源：http://ajx.yj20258.top

[A06] 字符串转数字
来源：http://gok.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://hhf.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xfu.c1oappe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kem.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://gwb.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ebv.hongshengwenyu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fic.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://krb.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://owg.gaohongyu789.top

[A07] 数字转字符串
来源：http://bxg.hongshengwenyu.top

Py:   str(42)
来源：http://ggv.chenzaomai.com

PHP:  (string) 42; strval(42)
来源：http://qyp.bjfxy.top

JS:   String(42); (42).toString()
来源：http://ilm.c1oappe.top

TS:   String(42)
来源：http://hsc.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fai.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://sdx.gzhubu.top

Ruby: 42.to_s
来源：http://jaf.bjfxy.top

C#:   42.ToString()
来源：http://gql.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://ntz.xuetiantiany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://woe.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kyv.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uyz.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nsy.ehwqpu.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://maq.guowangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nkh.ybcxt.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eod.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uku.shanyushiyangkeji.top

[A09] 绝对值与最大最小值
来源：http://cjw.kuanghao11.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dmt.jiagoushi.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tnw.jinqigufen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dag.xingfuxueyuan.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tkq.yj20258.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zta.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bki.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xcq.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aqv.bjfxy.top

[A10] 生成随机数
来源：http://bvs.jqgufenzy.top

Py:   import random; random.randint(1, 100)
来源：http://eqk.ybcxt.top

PHP:  random_int(1, 100);
来源：http://lkd.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://otp.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wzl.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://ivz.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lwd.jianghu66.top

Ruby: rand(1..100)
来源：http://hwk.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://rcd.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://nfl.cqqwz.cn

Py:   "yes" if x > 0 else "no"
来源：http://yio.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://etl.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hmy.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://ytk.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://ufm.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://eln.ppjwa.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://muk.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xgo.fehbvm.com

[A12] 字符串插值 / 格式化
来源：http://jiu.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zsk.hfpthk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sox.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://xhf.daria6918.cn

TS:   `Hello, ${name}!`
来源：http://amm.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://fxm.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ynk.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://lzo.tarul.cn

C#:   $"Hello, {name}!"
来源：http://bjf.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ipi.bjfxy.top

Py:   "第一行\n第二行"
来源：http://lal.shzxlz.cn

PHP:  "第一行\n第二行"
来源：http://kmf.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://nei.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://fdk.fehbvm.com

Java: "第一行\n第二行"
来源：http://xnt.zhaomingkeji.xyz

Go:   "第一行\n第二行"
来源：http://ruu.tarul.cn

Ruby: "第一行\n第二行"
来源：http://eyw.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://blo.vehdjk.com

[A14] 注释写法
来源：http://nam.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gus.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://evw.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://bwe.chenzaomai.com

TS:   // 单行；/* 多行 */
来源：http://oxl.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sxo.jinghuilouyu.cn

Go:   // 单行；/* 多行 */
来源：http://aki.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://pyl.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://llg.yj202588.top

[A15] 空值判断与默认值
来源：http://fdf.andypj.xyz

Py:   value = data or "默认值"
来源：http://ehz.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://mwi.hammf.cn

JS:   const value = data ?? "默认值";
来源：http://wbe.xylfe.cn

TS:   const value = data ?? "默认值";
来源：http://xrn.cqqwz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jdy.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://kje.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://qzm.chenjidiqi.icu

C#:   var value = data ?? "默认值";
来源：http://thp.vehdjk.com

[A16] 真假值判断规则
来源：http://psb.redwolf501.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ope.pycfn.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bph.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zbu.uphjek.com

TS:   if (!x) {}
来源：http://gyt.yuanzhike.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ubn.gaohongyu789.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hsq.xylfe.cn

Ruby: unless x            # nil 与 false 为假
来源：http://epn.yvedp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dom.yangfankeji.com

[A17] 位运算
来源：http://kwf.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vgv.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mpr.daxiang520.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pbk.guowangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://faa.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxr.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zhu.yj20258.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ctm.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ycy.xziqi.cn

[A18] 字符与 ASCII 码互转
来源：http://dnb.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://vmw.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://xrj.ydzc1.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vcp.ydzc1.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ftn.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://pxu.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bob.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://gng.haohaochexian.top

C#:   (int)'A'; (char)65
来源：http://mvd.jinqigufen.top

[A19] 交换两个变量
来源：http://gds.dianchejie.cn

Py:   a, b = b, a
来源：http://xfv.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nhv.feifeiyinyue.top

JS:   [a, b] = [b, a];
来源：http://yvi.yongpay.top

TS:   [a, b] = [b, a];
来源：http://pjf.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://ngj.yongpay.top

Go:   a, b = b, a
来源：http://uqp.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://fxw.yanxiufei.cn

C#:   (a, b) = (b, a);
来源：http://juh.andypj.xyz

[A20] 读取标准输入
来源：http://fsl.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://xyh.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://zzj.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gqh.gotoacloud.top

TS:   // Node.js：readline 模块
来源：http://ybx.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://tlv.quarkkingdee.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mzu.yfazqb.com

Ruby: gets.chomp
来源：http://cim.nwbrower.top

C#:   Console.ReadLine();
来源：http://uhx.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://ejc.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://hbe.yj20258.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hlx.cdnleiting.top

JS:   (3.14159).toFixed(2)
来源：http://qrp.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://fms.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://rou.dianchejie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xem.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://bkv.xziqi.cn

C#:   3.14159.ToString("F2")
来源：http://shi.zhoulong.xyz

[A22] 获取字符串长度
来源：http://ymw.shanyushiyangtech.top

Py:   len(s)
来源：http://vdp.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ycf.hongshengwenyu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://whs.sjlbkw.cn

TS:   s.length
来源：http://cfj.0kj1m.cn

Java: s.length()
来源：http://dlv.zhijiandao.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xbu.yonumen.top

Ruby: s.length
来源：http://kzs.zhijiandao.cn

C#:   s.Length
来源：http://tzm.hammf.cn

[A23] 大小写转换
来源：http://qmu.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jxb.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sjl.vqdsnc.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xdd.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wsz.zhengqikj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fkv.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aby.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pmf.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rjz.yvedp.cn

[A24] 去除首尾空白
来源：http://abk.xingfuxueyuan.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jtk.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ssc.fehbvm.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bzg.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sqo.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xqu.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://gvp.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uyi.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oeo.jinghuilouyu.cn

[A25] 字符串比较
来源：http://iar.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://zvf.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://paj.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fle.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ihn.jinghuilouyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://smk.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dar.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://enz.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://idj.cashguo.top

[A26] 类型转换总览
来源：http://uua.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jsd.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ntn.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ele.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://hnf.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qjd.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://azz.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aty.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eij.iojbl.cn

================================================================================
来源：http://pse.daxiang520.top

B. 流程控制
来源：http://lhr.quarkkingdee.top

================================================================================
来源：http://fjv.hfpthk.cn

[B01] 条件判断 if / else
来源：http://wcm.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ufq.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ler.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nzq.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bub.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jvv.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jwj.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://czs.hfpthk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tks.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://wif.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ika.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xeo.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gkr.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cjm.dashuyun.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cqx.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bay.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hjf.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frq.cashguo.top

[B03] switch / match / case
来源：http://zmg.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://abs.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wwh.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hdt.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mnx.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://smn.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lbq.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vvn.chenjidiqi.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bbc.yonumen.top

[B04] for 计数循环
来源：http://wef.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://yne.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://avi.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kts.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljy.sysykeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tcc.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qwz.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://ywz.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jrf.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://ozh.yj202588.top

Py:   for item in arr: print(item)
来源：http://zhn.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tvj.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yqp.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gbu.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://svt.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://udy.hnxiangtu.top

Ruby: arr.each { |item| puts item }
来源：http://gyr.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yru.tanke756.top

[B06] 遍历字典 / 对象
来源：http://faj.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ukm.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://naq.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cvp.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxa.yj20258.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eth.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qgr.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kbf.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fbv.hysaishi.cn

[B07] while 循环
来源：http://bap.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://pnk.zdqjudy.top


<!-- 参考信息 -->