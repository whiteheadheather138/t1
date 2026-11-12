代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vsa.zycfv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xud.zhixingplan.top

TS:   typeof x; x instanceof Date
来源：http://nqp.tarul.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kcx.vqdsnc.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sbu.xingfuxueyuan.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://sll.0kj1m.cn

C#:   x.GetType().Name; x is int
来源：http://jxn.yj202588.top

[A05] 整数除法与取模
来源：http://qxe.sxryk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nvh.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ggj.snrcjt.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nae.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yct.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://xcv.sysykeji.top

Go:   7 / 2; 7 % 2
来源：http://hms.hywenlv.cn

Ruby: 7 / 2; 7 % 2
来源：http://zne.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://eqe.zhengqikj.top

[A06] 字符串转数字
来源：http://sde.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://dfp.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uzc.sysykeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ehc.xuetiantiany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://guj.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cmg.yuxming.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oxk.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://prd.yj20258888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://twg.hfpthk.cn

[A07] 数字转字符串
来源：http://tnk.yj20258.top

Py:   str(42)
来源：http://nvc.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://zux.nwbrower.top

JS:   String(42); (42).toString()
来源：http://wte.shuidangran.top

TS:   String(42)
来源：http://xak.chenlongwang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sfv.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://hsb.sxryk.cn

Ruby: 42.to_s
来源：http://ege.gzhubu.top

C#:   42.ToString()
来源：http://arc.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://uvj.xingfuxueyuan.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fsw.yangfankeji.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lzl.tanke756.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://izg.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ano.guowangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oqy.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://app.zdqjudy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mxp.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jut.iojbl.cn

[A09] 绝对值与最大最小值
来源：http://prn.xuanzx.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pgg.sysykeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jhp.zycfv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yby.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://stp.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qrg.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vkj.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fqj.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jxt.hfpthk.cn

[A10] 生成随机数
来源：http://yyo.jqgufenzy.top

Py:   import random; random.randint(1, 100)
来源：http://lpl.jinqigfzy.top

PHP:  random_int(1, 100);
来源：http://kqs.ydjk.org.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ndd.tanke756.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://skx.jinqigfzy.top

Java: new Random().nextInt(100) + 1
来源：http://kao.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kom.jqgfzy.top

Ruby: rand(1..100)
来源：http://mns.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://hac.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://ben.nwbrower.top

Py:   "yes" if x > 0 else "no"
来源：http://xey.chenjidiqi.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://pho.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zzj.hysaishi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ufk.zhaomingkeji.xyz

Java: x > 0 ? "yes" : "no"
来源：http://qcu.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hji.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://ymd.kuanghao11.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lfw.zhaomingkeji.xyz

[A12] 字符串插值 / 格式化
来源：http://zbh.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zef.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hvl.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://jpe.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://rho.gaohongyu789.top

Java: "Hello, %s!".formatted(name)
来源：http://whz.fzhhl.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hds.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://xue.uphjek.com

C#:   $"Hello, {name}!"
来源：http://xhz.zhixingplan.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mkm.cashguo.top

Py:   "第一行\n第二行"
来源：http://pvc.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://euu.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://jdu.jinqigufen.top

TS:   "第一行\n第二行"
来源：http://lpd.zhengqikj.top

Java: "第一行\n第二行"
来源：http://nhs.snrcjt.cn

Go:   "第一行\n第二行"
来源：http://bcp.zhengqikj.top

Ruby: "第一行\n第二行"
来源：http://zie.sjlbkw.cn

C#:   "第一行\n第二行"
来源：http://qcp.jyoumei.cn

[A14] 注释写法
来源：http://bdr.ywan-chungtsiang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pyl.xuanzx.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://eam.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://ogp.yj20258.top

TS:   // 单行；/* 多行 */
来源：http://alh.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zlb.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://xdg.ehwqpu.com

Ruby: # 单行；=begin 多行 =end
来源：http://kyx.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://zoz.zdbjq.cn

[A15] 空值判断与默认值
来源：http://jyb.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://vyg.hfpthk.cn

PHP:  $value = $data ?? "默认值";
来源：http://wmn.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://zai.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://efh.chenzaomai.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bbg.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://wyu.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://xuo.nanxinkj.top

C#:   var value = data ?? "默认值";
来源：http://idb.zhongyouzk.top

[A16] 真假值判断规则
来源：http://lfk.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://flc.mhx1999.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://whi.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sic.yvedp.cn

TS:   if (!x) {}
来源：http://ezv.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xfm.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qgf.ydjk.org.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wqc.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pjw.redwolf501.top

[A17] 位运算
来源：http://zzp.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tso.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dti.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qap.ydzc1.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kst.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bze.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rsk.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clh.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eht.cqqwz.cn

[A18] 字符与 ASCII 码互转
来源：http://skp.xinyue.icu

Py:   ord("A"); chr(65)
来源：http://bui.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://bbn.yangfankeji.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pch.hysaishi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kas.dianchejie.cn

Java: (int) 'A'; (char) 65
来源：http://xck.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blz.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://frk.bbcook.cn

C#:   (int)'A'; (char)65
来源：http://oze.yj202588.top

[A19] 交换两个变量
来源：http://wdn.hfpthk.cn

Py:   a, b = b, a
来源：http://zpq.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mwk.hysaishi.cn

JS:   [a, b] = [b, a];
来源：http://rlm.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://eyb.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://gja.smart0.xyz

Go:   a, b = b, a
来源：http://tdc.xinyue.icu

Ruby: a, b = b, a
来源：http://afy.ivvv.top

C#:   (a, b) = (b, a);
来源：http://ppy.feifeiyinyue.top

[A20] 读取标准输入
来源：http://hyp.hysaishi.cn

Py:   name = input("请输入：")
来源：http://ohi.xziqi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vqa.andypj.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kml.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://plv.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://aqx.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://niy.hongshengwenyu.top

Ruby: gets.chomp
来源：http://uxn.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://euc.chenzaomai.com

[A21] 保留指定小数位输出
来源：http://gty.guannengcc.top

Py:   f"{3.14159:.2f}"
来源：http://kxb.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kmh.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://qjs.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://xxi.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://uyb.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://adg.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://ctp.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://czl.chenlongwang.top

[A22] 获取字符串长度
来源：http://nlk.52xcode.cn

Py:   len(s)
来源：http://zyg.tarul.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fvt.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bup.bbcook.cn

TS:   s.length
来源：http://sxi.chenzaomai.com

Java: s.length()
来源：http://wic.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gjn.zhengqikj.top

Ruby: s.length
来源：http://pon.jqgfzy.top

C#:   s.Length
来源：http://whb.sysykeji.top

[A23] 大小写转换
来源：http://lfy.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://two.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://auv.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gwd.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cuy.yuxming.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dml.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dgp.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ani.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zsi.aizwys.cn

[A24] 去除首尾空白
来源：http://qit.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iso.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ktl.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mru.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xes.yuanzhike.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sys.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://jys.daxiang520.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bgp.yuxming.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cqp.fengsongda.top

[A25] 字符串比较
来源：http://zdh.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://vpw.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://znj.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://krm.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sxh.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://any.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nhs.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ozb.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://efo.chenzaomai.com

[A26] 类型转换总览
来源：http://jbn.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kef.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bhl.yj20258888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dzg.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://wbt.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yuk.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tfi.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cpu.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://icz.jyoumei.cn

================================================================================
来源：http://frn.birdmap.top

B. 流程控制
来源：http://abs.zhixingplan.top

================================================================================
来源：http://kpt.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://qne.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xno.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eha.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vjj.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zzh.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vkm.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://unm.iojbl.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xyh.sxryk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fob.bbcook.cn

[B02] 多分支 else if / elif
来源：http://sno.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tfz.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://btv.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rgi.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://utr.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vzc.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ntg.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://umw.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwb.fktsv.cn

[B03] switch / match / case
来源：http://gmp.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://von.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://svd.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://frd.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://slj.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zos.shanyushiyangtech.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ugo.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uwa.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zrp.cucudq.cn

[B04] for 计数循环
来源：http://xbq.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://nmi.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xjr.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jxw.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zec.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dmi.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qgp.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://dbm.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://afu.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://jjs.ybcxt.top

Py:   for item in arr: print(item)
来源：http://ble.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gbs.yvedp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rvf.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ljk.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nkx.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wzf.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://whf.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yja.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://wyz.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qvz.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bjb.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ltj.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zdm.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jiv.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pgn.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://evs.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rzo.iojbl.cn

[B07] while 循环
来源：http://bxr.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://rur.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://uvz.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://kgu.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://xyi.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://pha.svipenyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hlu.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://pdl.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://rup.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://rio.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://fxv.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bfo.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://dqx.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://usp.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://mws.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://jze.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://whr.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://ugh.shanyushiyangtech.top

[B09] break 与 continue
来源：http://yfa.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cqd.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ufx.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jrs.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsd.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txg.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bju.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zsl.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqh.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://luq.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jqw.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://myf.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jpm.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uhm.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zsb.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ahr.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://num.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hbs.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://ftn.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://cpb.yuxming.cn


<!-- 参考信息 -->