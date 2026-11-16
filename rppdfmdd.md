代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://mvl.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://ojx.hfpthk.cn

Ruby: puts "Hello, World!"
来源：http://jbz.yangfankeji.com

C#:   Console.WriteLine("Hello, World!");
来源：http://bgq.gogol.net.cn

[A02] 变量声明与赋值
来源：http://ynt.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mnd.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zhx.gaohongyu789.top

JS:   let name = "Alex"; const age = 20;
来源：http://nnc.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uoy.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://scj.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://xio.snrcjt.cn

Ruby: name = "Alex"; age = 20
来源：http://kbl.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://sqo.tian-w.cn

[A03] 常量定义
来源：http://xav.ehwqpu.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://spt.ivvv.top

PHP:  const PI = 3.14159;
来源：http://mgw.guannengcc.top

JS:   const PI = 3.14159;
来源：http://rpd.bbcook.cn

TS:   const PI: number = 3.14159;
来源：http://bck.shuidangran.top

Java: static final double PI = 3.14159;
来源：http://ocm.aibaodan.cn

Go:   const PI = 3.14159
来源：http://qmy.fehbvm.com

Ruby: PI = 3.14159
来源：http://eio.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://fya.cqqwz.cn

[A04] 判断变量类型
来源：http://usz.yj202588.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bai.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iti.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eiq.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://gtp.hnqzz.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://add.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://izs.ctjpmb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ezx.yangfankeji.com

C#:   x.GetType().Name; x is int
来源：http://wqv.vqdsnc.cn

[A05] 整数除法与取模
来源：http://sxv.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ojs.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://kid.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://byq.iojbl.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zxb.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://swx.xuanzx.com

Go:   7 / 2; 7 % 2
来源：http://tys.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://vig.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://ewj.zhijiandao.cn

[A06] 字符串转数字
来源：http://vel.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://opm.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bws.ywan-chungtsiang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oqf.ywan-chungtsiang.top

TS:   parseInt("42", 10); Number("42")
来源：http://mzs.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pgv.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://byd.xingfuxueyuan.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://umg.tanke756.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ctp.uphjek.com

[A07] 数字转字符串
来源：http://czo.hesvh.cn

Py:   str(42)
来源：http://ugh.sufxvd.cn

PHP:  (string) 42; strval(42)
来源：http://jbx.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://vwi.andypj.xyz

TS:   String(42)
来源：http://eof.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jds.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://znr.havefunace.top

Ruby: 42.to_s
来源：http://ezn.c1oappe.top

C#:   42.ToString()
来源：http://gbs.chenlongwang.top

[A08] 取整与四舍五入
来源：http://hpk.gotoacloud.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ksp.wangdashe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bvr.ppjwa.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pkc.dianchejie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sez.redwolf501.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ldf.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tif.cucudq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lyc.daria6918.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sak.cheryme.top

[A09] 绝对值与最大最小值
来源：http://vmb.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nef.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jnh.yongpay.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jwm.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ozb.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://app.kuanghao11.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://guq.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nya.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uie.ivvv.top

[A10] 生成随机数
来源：http://abk.52xcode.cn

Py:   import random; random.randint(1, 100)
来源：http://qsk.pengpengdd.cyou

PHP:  random_int(1, 100);
来源：http://zqp.xziqi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uej.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pqc.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://jhs.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zjz.smart0.xyz

Ruby: rand(1..100)
来源：http://nje.aibaodan.cn

C#:   new Random().Next(1, 101)
来源：http://eao.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://wgq.aibaodan.cn

Py:   "yes" if x > 0 else "no"
来源：http://izk.andypj.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://upj.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fhj.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xju.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://lan.yj202588.top

Go:   // 无三元运算符，需用 if 语句
来源：http://euv.hammf.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zxv.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tka.yueranfly.top

[A12] 字符串插值 / 格式化
来源：http://khz.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xgd.zhixingplan.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fnn.yj20258.top

JS:   `Hello, ${name}!`
来源：http://njr.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://xmn.zhijiandao.cn

Java: "Hello, %s!".formatted(name)
来源：http://ega.chenzaomai.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yev.yueranfly.top

Ruby: "Hello, #{name}!"
来源：http://asc.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://yjp.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://luw.yanxiufei.cn

Py:   "第一行\n第二行"
来源：http://fqa.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://juo.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://bzo.shangyingyoupin.top

TS:   "第一行\n第二行"
来源：http://rbh.sufxvd.cn

Java: "第一行\n第二行"
来源：http://txx.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://hom.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://vhd.havefunace.top

C#:   "第一行\n第二行"
来源：http://buv.shuidangran.top

[A14] 注释写法
来源：http://nma.tian-w.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gib.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://wqy.iojbl.cn

JS:   // 单行；/* 多行 */
来源：http://sya.yuxming.cn

TS:   // 单行；/* 多行 */
来源：http://qpo.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kpy.sysykeji.top

Go:   // 单行；/* 多行 */
来源：http://auy.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://cql.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://wli.xingfuxueyuan.xyz

[A15] 空值判断与默认值
来源：http://htc.gogol.net.cn

Py:   value = data or "默认值"
来源：http://srt.yfazqb.com

PHP:  $value = $data ?? "默认值";
来源：http://tob.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://bxf.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://noy.aibaodan.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yzq.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://mdj.tianlin.xyz

Ruby: value = data || "默认值"
来源：http://fba.ydzc1.top

C#:   var value = data ?? "默认值";
来源：http://kan.fktsv.cn

[A16] 真假值判断规则
来源：http://ith.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qvz.yfazqb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ldr.ydzc1.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kmp.vehdjk.com

TS:   if (!x) {}
来源：http://iuc.ywan-chungtsiang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vme.pengpengdd.cyou

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bnx.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://wgg.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://edj.nanxuanxn.top

[A17] 位运算
来源：http://dbh.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ubw.fktsv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bto.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncv.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pxd.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gar.hnxiangtu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zgw.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xfq.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mvw.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://mht.cheryme.top

Py:   ord("A"); chr(65)
来源：http://bzu.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://eop.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mut.sweek.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bbe.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://qot.xuetiantiany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://otq.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://aqu.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://pmj.sufxvd.cn

[A19] 交换两个变量
来源：http://mjo.hnxiangtu.top

Py:   a, b = b, a
来源：http://tuk.bjfxy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hks.quarkkingdee.top

JS:   [a, b] = [b, a];
来源：http://lcl.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://lym.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://pxk.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://mmb.quarkkingdee.top

Ruby: a, b = b, a
来源：http://vdg.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://fan.hfpthk.cn

[A20] 读取标准输入
来源：http://iik.sufxvd.cn

Py:   name = input("请输入：")
来源：http://bnf.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qst.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zsv.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://cit.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://jak.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fgg.pycfn.com

Ruby: gets.chomp
来源：http://dxe.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://maq.iojbl.cn

[A21] 保留指定小数位输出
来源：http://zce.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://yrb.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mbr.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://jqz.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://yev.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://cek.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oec.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://kqx.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://odb.ehwqpu.com

[A22] 获取字符串长度
来源：http://vhq.xziqi.cn

Py:   len(s)
来源：http://bln.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ydi.316326.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xgt.shanyushiyangkeji.top

TS:   s.length
来源：http://bdh.hcnkem.com

Java: s.length()
来源：http://wvs.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bal.ctjpmb.com

Ruby: s.length
来源：http://pfo.zhongyouzk.top

C#:   s.Length
来源：http://ylg.kuanghao11.cn

[A23] 大小写转换
来源：http://xsb.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bxf.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://phh.zdbjq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dkq.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xyt.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rxu.gotoacloud.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aih.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qjt.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://iod.nanxinkj.top

[A24] 去除首尾空白
来源：http://usr.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dhy.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bhu.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://umd.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tek.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lgj.jlsjyb.cn

Go:   strings.TrimSpace(s)
来源：http://kco.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rjh.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kut.iojbl.cn

[A25] 字符串比较
来源：http://bfh.tarul.cn

Py:   s1 == s2; s1 != s2
来源：http://ulm.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://met.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hky.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hyi.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://snx.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://izk.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xmd.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ham.gotoacloud.top

[A26] 类型转换总览
来源：http://ngq.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lsv.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jme.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cpu.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://kkw.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tce.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ith.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oej.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://frg.epnwcf.com

================================================================================
来源：http://lra.vqdsnc.cn

B. 流程控制
来源：http://jaa.c1oappe.top

================================================================================
来源：http://cxd.fehbvm.com

[B01] 条件判断 if / else
来源：http://dza.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qgr.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lsy.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mpw.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bzo.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pua.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jhl.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zlk.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zfd.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://zam.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nrk.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mms.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzg.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mpo.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rqu.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cnc.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lus.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpm.jinqigufen.top

[B03] switch / match / case
来源：http://iyx.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://txl.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jze.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ztr.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbx.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hqr.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sbt.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zvz.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qjy.52xcode.cn

[B04] for 计数循环
来源：http://ndv.yj20258.top

Py:   for i in range(10): print(i)
来源：http://myf.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zrz.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iss.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hwk.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uwn.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gme.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://rxc.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bki.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://beh.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://shy.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dab.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://amo.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qry.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://brg.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sni.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://kqo.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jjo.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://ukh.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://xgi.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://omy.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ysq.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fnh.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xut.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zkx.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kwu.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://brh.jlsjyb.cn

[B07] while 循环
来源：http://dho.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://jqx.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://axv.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://rcn.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://ovp.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://wll.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dxg.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://xpp.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://vpn.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://oal.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://jrl.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wzr.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://dan.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://cgd.dashuyun.cn


<!-- 参考信息 -->