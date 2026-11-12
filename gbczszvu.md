代发 wailian999

================================================================================
来源：http://cyp.uphjek.com

A. 基础语法与类型
来源：http://koj.yueranfly.top

================================================================================
来源：http://btc.pycfn.com

[A01] Hello World
来源：http://mpv.tianlin.xyz

Py:   print("Hello, World!")
来源：http://msy.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://blk.cheryme.top

JS:   console.log("Hello, World!");
来源：http://tsi.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eop.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://qep.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://inb.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://aej.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ogs.zdbjq.cn

[A02] 变量声明与赋值
来源：http://nfd.sjlbkw.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://elj.9152youxi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wxa.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://llk.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yjg.redwolf501.top

Java: String name = "Alex"; int age = 20;
来源：http://inm.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://xiv.yuxming.cn

Ruby: name = "Alex"; age = 20
来源：http://bjt.c1oappe.top

C#:   string name = "Alex"; int age = 20;
来源：http://rqf.fzhhl.top

[A03] 常量定义
来源：http://sht.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yyt.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://jrv.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://jpu.zycfv.cn

TS:   const PI: number = 3.14159;
来源：http://xjn.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://lyf.svipenyu.cn

Go:   const PI = 3.14159
来源：http://rbt.hcnkem.com

Ruby: PI = 3.14159
来源：http://jly.tanke756.top

C#:   const double PI = 3.14159;
来源：http://grc.gogol.net.cn

[A04] 判断变量类型
来源：http://sew.cucudq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tnv.chenjidiqi.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kjz.sjlbkw.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pal.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://xes.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://paf.zhongyouzk.top

Go:   reflect.TypeOf(x).Name()
来源：http://gsu.hywenlv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kez.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://fns.gzhubu.top

[A05] 整数除法与取模
来源：http://exw.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ypf.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mbo.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yku.jqgfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://znp.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://onq.9152youxi.cn

Go:   7 / 2; 7 % 2
来源：http://zzr.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://gyu.hesvh.cn

C#:   7 / 2; 7 % 2
来源：http://snp.nanxinkj.top

[A06] 字符串转数字
来源：http://azr.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://dbr.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vqj.hcnkem.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uho.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://caj.hfpthk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://peu.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rey.chenlongwang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ozp.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cby.fengsongda.top

[A07] 数字转字符串
来源：http://xho.jinyuanbaomall.cn

Py:   str(42)
来源：http://bqs.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://sqw.svipenyu.cn

JS:   String(42); (42).toString()
来源：http://gvh.hammf.cn

TS:   String(42)
来源：http://onr.hnxiangtu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vfo.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://ans.tanke756.top

Ruby: 42.to_s
来源：http://xwq.jqgufenzy.top

C#:   42.ToString()
来源：http://kmu.ydjk.org.cn

[A08] 取整与四舍五入
来源：http://pgf.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yvb.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hne.smart0.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gmh.tarul.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gyo.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://szw.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dek.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://evq.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mql.ybcxt.top

[A09] 绝对值与最大最小值
来源：http://ucj.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gre.shangyingyoupin.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cyn.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qkz.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://erb.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hwm.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://agz.ehwqpu.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zbz.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://skf.wangdashe.top

[A10] 生成随机数
来源：http://epa.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://ybt.sweek.top

PHP:  random_int(1, 100);
来源：http://cha.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://piv.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xqe.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://crb.jiagoushi.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qlc.gotoacloud.top

Ruby: rand(1..100)
来源：http://ldf.shuidangran.top

C#:   new Random().Next(1, 101)
来源：http://foa.kuanghao11.cn

[A11] 条件表达式（三元）
来源：http://xic.pengpengdd.cyou

Py:   "yes" if x > 0 else "no"
来源：http://lva.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jiq.xuanzx.com

JS:   x > 0 ? "yes" : "no"
来源：http://eli.yuanzhike.top

TS:   x > 0 ? "yes" : "no"
来源：http://wid.sxryk.cn

Java: x > 0 ? "yes" : "no"
来源：http://njp.zhaomingkeji.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://vpg.nwbrower.top

Ruby: x > 0 ? "yes" : "no"
来源：http://til.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://xhm.cheryme.top

[A12] 字符串插值 / 格式化
来源：http://jvj.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ddk.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tys.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://rym.nanxuanxn.top

TS:   `Hello, ${name}!`
来源：http://ehf.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://ypa.cucudq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://unj.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://tmv.xylfe.cn

C#:   $"Hello, {name}!"
来源：http://ezw.cqqwz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oef.yanxiufei.cn

Py:   "第一行\n第二行"
来源：http://nnf.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://qla.316326.xyz

JS:   "第一行\n第二行"
来源：http://xko.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://utx.zycfv.cn

Java: "第一行\n第二行"
来源：http://ibf.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://uvf.chenlongwang.top

Ruby: "第一行\n第二行"
来源：http://qqo.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://gmo.nanxuanxn.top

[A14] 注释写法
来源：http://gxs.ctjpmb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://fvu.yongpay.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fjv.0kj1m.cn

JS:   // 单行；/* 多行 */
来源：http://nqo.daria6918.cn

TS:   // 单行；/* 多行 */
来源：http://srd.smart0.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jir.sxryk.cn

Go:   // 单行；/* 多行 */
来源：http://stk.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://gkr.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://ggz.xuanzx.com

[A15] 空值判断与默认值
来源：http://toh.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://csx.ctjpmb.com

PHP:  $value = $data ?? "默认值";
来源：http://vvr.svipenyu.cn

JS:   const value = data ?? "默认值";
来源：http://aoe.vqdsnc.cn

TS:   const value = data ?? "默认值";
来源：http://liq.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ntd.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://mer.cdnleiting.top

Ruby: value = data || "默认值"
来源：http://jrf.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://moq.jinqigfzy.top

[A16] 真假值判断规则
来源：http://ibx.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://owd.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lil.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qdn.wangshuangyany.cn

TS:   if (!x) {}
来源：http://exn.chenlongwang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://urr.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xlj.yanxiufei.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xbd.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hff.pycfn.com

[A17] 位运算
来源：http://wwh.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnd.ehwqpu.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qqb.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxz.gotoacloud.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cnn.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qpu.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fvz.hcnkem.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gjc.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jwg.yuxming.cn

[A18] 字符与 ASCII 码互转
来源：http://vjn.yj20258.top

Py:   ord("A"); chr(65)
来源：http://ebk.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://fka.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hjl.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mcg.gzhubu.top

Java: (int) 'A'; (char) 65
来源：http://ssy.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wbp.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://nyl.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://hiy.iojbl.cn

[A19] 交换两个变量
来源：http://inq.xuanzx.com

Py:   a, b = b, a
来源：http://wfm.jinqigfzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fas.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://ijv.zhengqikj.top

TS:   [a, b] = [b, a];
来源：http://jgb.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://ncb.ywan-chungtsiang.top

Go:   a, b = b, a
来源：http://aeg.hywenlv.cn

Ruby: a, b = b, a
来源：http://hpo.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://lbl.zdbjq.cn

[A20] 读取标准输入
来源：http://kmh.52xcode.cn

Py:   name = input("请输入：")
来源：http://zud.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rmj.pycfn.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gag.uphjek.com

TS:   // Node.js：readline 模块
来源：http://tpy.xinyue.icu

Java: new Scanner(System.in).nextLine()
来源：http://zgg.zhixingplan.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wch.epnwcf.com

Ruby: gets.chomp
来源：http://ygb.yj20258888.top

C#:   Console.ReadLine();
来源：http://zmr.fehbvm.com

[A21] 保留指定小数位输出
来源：http://lbj.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://cgu.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mva.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://ycu.daria6918.cn

TS:   (3.14159).toFixed(2)
来源：http://nhv.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://evd.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ujb.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://yav.iojbl.cn

C#:   3.14159.ToString("F2")
来源：http://jrw.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://tia.bbcook.cn

Py:   len(s)
来源：http://lcz.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fug.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fas.quarkkingdee.top

TS:   s.length
来源：http://jev.gaohongyu789.top

Java: s.length()
来源：http://hfb.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lvq.yj20258.top

Ruby: s.length
来源：http://jcb.52xcode.cn

C#:   s.Length
来源：http://zof.pycfn.com

[A23] 大小写转换
来源：http://guf.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qkq.cashguo.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vew.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://une.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lmb.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vgn.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uij.xziqi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mlb.ywan-chungtsiang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nni.daria6918.cn

[A24] 去除首尾空白
来源：http://vzl.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tau.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://enp.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sur.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ysy.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mfn.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://lww.haohaochexian.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nwk.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dup.feifeiyinyue.top

[A25] 字符串比较
来源：http://gpj.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://gex.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eia.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lxc.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uja.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rhu.9152youxi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://frw.jqgufenzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bse.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lri.zhixingplan.top

[A26] 类型转换总览
来源：http://hhq.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lmx.yongpay.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ije.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kyu.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://nrr.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lgj.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://txq.hcnkem.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://enh.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://unp.iojbl.cn

================================================================================
来源：http://qmp.cucudq.cn

B. 流程控制
来源：http://yph.shzxlz.cn

================================================================================
来源：http://zsn.ivvv.top

[B01] 条件判断 if / else
来源：http://lbh.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dij.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uml.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gdv.cashguo.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wva.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://icf.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gdd.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wep.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xby.gzhubu.top

[B02] 多分支 else if / elif
来源：http://loz.sysykeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hvu.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dwd.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yux.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://atc.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbn.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ihq.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jks.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://imy.sufxvd.cn

[B03] switch / match / case
来源：http://sue.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eez.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uly.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wxl.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jiu.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rdb.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tes.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xbb.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wzf.aizwys.cn

[B04] for 计数循环
来源：http://xun.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://aco.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kbh.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blc.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gme.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dxk.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vcr.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://avd.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oft.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://hqq.shuidangran.top

Py:   for item in arr: print(item)
来源：http://wsv.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yyx.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bhi.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nvc.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://mrs.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sog.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://pkr.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ehw.yonumen.top

[B06] 遍历字典 / 对象
来源：http://rua.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://syk.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ugs.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uoc.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://icm.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xlb.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qmv.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hbe.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://esi.sufxvd.cn

[B07] while 循环
来源：http://ugh.birdmap.top

Py:   while i < 10: i += 1
来源：http://lhg.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://mmt.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://bkq.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://klk.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://axa.zycfv.cn


<!-- 参考信息 -->