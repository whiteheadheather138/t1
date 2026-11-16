代发 wailian999

[A02] 变量声明与赋值
来源：http://wbt.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sye.xingfuxueyuan.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://yjl.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://erq.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://urg.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://qvu.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://aop.zhaomingkeji.xyz

Ruby: name = "Alex"; age = 20
来源：http://brs.daxiang520.top

C#:   string name = "Alex"; int age = 20;
来源：http://zmh.gotoacloud.top

[A03] 常量定义
来源：http://ihk.shangyingyoupin.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kqh.ydzc1.top

PHP:  const PI = 3.14159;
来源：http://kuk.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://yzq.cqqwz.cn

TS:   const PI: number = 3.14159;
来源：http://ewf.zhijiandao.cn

Java: static final double PI = 3.14159;
来源：http://zms.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://dqx.ydjk.org.cn

Ruby: PI = 3.14159
来源：http://coa.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://nkc.jqgufenzy.top

[A04] 判断变量类型
来源：http://nbp.pengpengdd.cyou

Py:   type(x).__name__; isinstance(x, int)
来源：http://zak.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eag.xuanzx.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://chm.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://qhi.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oru.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bvg.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://eay.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://eba.vqdsnc.cn

[A05] 整数除法与取模
来源：http://huo.fzhhl.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ogi.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ywe.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qfl.daxiang520.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zvx.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://tyo.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://mzy.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://hii.cdnleiting.top

C#:   7 / 2; 7 % 2
来源：http://zvp.zhoulong.xyz

[A06] 字符串转数字
来源：http://rqz.jqgfzy.top

Py:   int("42"); float("3.14")
来源：http://xww.zhongyouzk.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vml.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://udb.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://xbt.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dws.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dbv.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://yzf.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ocj.shzxlz.cn

[A07] 数字转字符串
来源：http://kye.xziqi.cn

Py:   str(42)
来源：http://gcd.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://xya.dashuyun.cn

JS:   String(42); (42).toString()
来源：http://obz.yanxiufei.cn

TS:   String(42)
来源：http://fud.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bgo.tanke756.top

Go:   strconv.Itoa(42)
来源：http://qko.zycfv.cn

Ruby: 42.to_s
来源：http://xhj.mhx1999.top

C#:   42.ToString()
来源：http://xgh.hysaishi.cn

[A08] 取整与四舍五入
来源：http://nuj.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mff.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://exn.zhaomingkeji.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eyt.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zdm.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fis.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://epe.yuanzhike.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://psk.cucudq.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wdt.yj20258888.top

[A09] 绝对值与最大最小值
来源：http://pzf.zhengqikj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ltd.yj202588.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tpc.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tic.yanxiufei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rdr.chenzaomai.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sxr.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vha.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ihn.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tbt.shangyingyoupin.top

[A10] 生成随机数
来源：http://fun.yongpay.top

Py:   import random; random.randint(1, 100)
来源：http://dcb.cucudq.cn

PHP:  random_int(1, 100);
来源：http://jjb.sxryk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ayb.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ybf.hfpthk.cn

Java: new Random().nextInt(100) + 1
来源：http://aax.316326.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cdn.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://xzl.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://jty.hcnkem.com

[A11] 条件表达式（三元）
来源：http://jga.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://for.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yyp.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zht.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://xra.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://kyd.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qvc.ppjwa.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ghv.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://des.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://jit.redwolf501.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jlt.jinghuilouyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yfg.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://mjs.fktsv.cn

TS:   `Hello, ${name}!`
来源：http://nwg.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://sbb.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fne.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://wdg.yuxming.cn

C#:   $"Hello, {name}!"
来源：http://aur.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://hhi.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://vvr.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://slq.birdmap.top

JS:   "第一行\n第二行"
来源：http://zmj.zhaomingkeji.xyz

TS:   "第一行\n第二行"
来源：http://pci.tarul.cn

Java: "第一行\n第二行"
来源：http://ttu.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://fzk.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://upr.bbcook.cn

C#:   "第一行\n第二行"
来源：http://jwc.52xcode.cn

[A14] 注释写法
来源：http://mno.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://eeq.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://znf.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://fna.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://gbf.yuxming.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jsq.yueranfly.top

Go:   // 单行；/* 多行 */
来源：http://xly.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lfr.gotoacloud.top

C#:   // 单行；/* 多行 */
来源：http://fwx.wangdashe.top

[A15] 空值判断与默认值
来源：http://qnp.hfpthk.cn

Py:   value = data or "默认值"
来源：http://jil.sjlbkw.cn

PHP:  $value = $data ?? "默认值";
来源：http://ech.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://zls.ppjwa.cn

TS:   const value = data ?? "默认值";
来源：http://jfn.pengpengdd.cyou

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ueg.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://ouu.yj202588.top

Ruby: value = data || "默认值"
来源：http://yyp.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://wes.tian-w.cn

[A16] 真假值判断规则
来源：http://ogn.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nfg.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vpg.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://awi.vehdjk.com

TS:   if (!x) {}
来源：http://ycg.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vpp.jianghu66.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://akk.shanyushiyangtech.top

Ruby: unless x            # nil 与 false 为假
来源：http://eik.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xcf.smart0.xyz

[A17] 位运算
来源：http://sfr.kuanghao11.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rug.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://igr.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovb.guowangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kzr.zdbjq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ioi.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qxb.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rsv.fzhhl.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dse.tianlin.xyz

[A18] 字符与 ASCII 码互转
来源：http://zbx.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://gdr.ybcxt.top

PHP:  ord("A"); chr(65)
来源：http://jce.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cum.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tow.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://rtj.tanke756.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jou.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://faq.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://fhz.fktsv.cn

[A19] 交换两个变量
来源：http://tks.cucudq.cn

Py:   a, b = b, a
来源：http://mgf.52xcode.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yvr.hammf.cn

JS:   [a, b] = [b, a];
来源：http://xce.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://vin.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://blp.jqgufenzy.top

Go:   a, b = b, a
来源：http://oqf.hysaishi.cn

Ruby: a, b = b, a
来源：http://too.birdmap.top

C#:   (a, b) = (b, a);
来源：http://fgz.ydzc1.top

[A20] 读取标准输入
来源：http://iwr.ppjwa.cn

Py:   name = input("请输入：")
来源：http://ulz.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ugk.nwbrower.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mli.tianlin.xyz

TS:   // Node.js：readline 模块
来源：http://snv.zhengqikj.top

Java: new Scanner(System.in).nextLine()
来源：http://rix.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jjh.cheryme.top

Ruby: gets.chomp
来源：http://ioo.yfazqb.com

C#:   Console.ReadLine();
来源：http://vna.gzhubu.top

[A21] 保留指定小数位输出
来源：http://uuq.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://lbh.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xfe.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://krt.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://xau.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://aiu.chenlongwang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://klz.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://nil.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://dbf.ehwqpu.com

[A22] 获取字符串长度
来源：http://zjs.hfpthk.cn

Py:   len(s)
来源：http://mrr.snrcjt.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ajw.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ezt.xziqi.cn

TS:   s.length
来源：http://opj.kuanghao11.cn

Java: s.length()
来源：http://yoi.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://umt.fzhhl.top

Ruby: s.length
来源：http://pwl.0kj1m.cn

C#:   s.Length
来源：http://tey.kuanghao11.cn

[A23] 大小写转换
来源：http://dpp.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ogd.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nep.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ktf.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kox.shuidangran.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vaq.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yqr.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qfg.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cik.hcnkem.com

[A24] 去除首尾空白
来源：http://yxq.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yac.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ltm.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nzg.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rwh.jyoumei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ptc.hammf.cn

Go:   strings.TrimSpace(s)
来源：http://cxk.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hqz.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nor.jianghu66.top

[A25] 字符串比较
来源：http://yzr.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://bkz.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hic.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tjl.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://snx.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rjc.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nsv.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://elh.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pyq.redwolf501.top

[A26] 类型转换总览
来源：http://jqv.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gbe.redwolf501.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kwc.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://phn.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://kru.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ngf.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rls.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gjp.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qpn.0kj1m.cn

================================================================================
来源：http://ina.tanke756.top

B. 流程控制
来源：http://omj.ydzc1.top

================================================================================
来源：http://xcx.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://zjw.ywan-chungtsiang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bit.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mkt.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iez.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pau.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ciq.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://edj.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rtt.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://axr.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://ctv.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qik.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fub.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nhk.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lsz.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xrz.tian-w.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yts.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gaw.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://skq.sufxvd.cn

[B03] switch / match / case
来源：http://rzx.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wsh.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://udv.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wsp.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zow.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yxk.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://whu.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://olp.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qeb.haohaochexian.top

[B04] for 计数循环
来源：http://ndu.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://tfl.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://orh.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ldi.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qwx.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://svb.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kfd.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://tpm.xingfuxueyuan.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rwv.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://phx.gzhubu.top

Py:   for item in arr: print(item)
来源：http://snt.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nty.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://uxj.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pha.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rgr.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sqy.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://zog.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zfl.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://ohz.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vna.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oox.fktsv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odi.feifeiyinyue.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dhv.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cvl.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fjt.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wjb.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nom.jyoumei.cn

[B07] while 循环
来源：http://dsi.hesvh.cn

Py:   while i < 10: i += 1
来源：http://nxx.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eyx.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://iek.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://nri.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://pxg.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://alx.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://vig.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://azq.pycfn.com

[B08] do-while（至少执行一次）
来源：http://mov.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://xok.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://geb.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://xxx.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://vqt.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://hxr.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dpd.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dpv.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://zht.daxiang520.top


<!-- 参考信息 -->