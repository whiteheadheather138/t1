代发 wailian999

[A02] 变量声明与赋值
来源：http://svt.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ejc.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kel.bjfxy.top

JS:   let name = "Alex"; const age = 20;
来源：http://xbs.tarul.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bqx.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://ykv.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://osr.dianchejie.cn

Ruby: name = "Alex"; age = 20
来源：http://qgo.c1oappe.top

C#:   string name = "Alex"; int age = 20;
来源：http://vaj.fktsv.cn

[A03] 常量定义
来源：http://wsg.fengsongda.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://asj.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://ame.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://gww.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://wrg.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://mtr.xylfe.cn

Go:   const PI = 3.14159
来源：http://azn.dashuyun.cn

Ruby: PI = 3.14159
来源：http://xfu.wangdashe.top

C#:   const double PI = 3.14159;
来源：http://qyv.0kj1m.cn

[A04] 判断变量类型
来源：http://sod.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oxj.jinqigfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tta.ywan-chungtsiang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://smq.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://uji.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gdy.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://clk.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ira.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://uhj.yongpay.top

[A05] 整数除法与取模
来源：http://kuj.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ldb.yueranfly.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pql.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dud.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://diq.gzhubu.top

Java: 7 / 2; 7 % 2
来源：http://kof.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://hup.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://edx.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://mkk.haohaochexian.top

[A06] 字符串转数字
来源：http://nvf.cqqwz.cn

Py:   int("42"); float("3.14")
来源：http://iqx.yvedp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://htd.xinyue.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ifk.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kia.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vhi.jinqigufen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jhf.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ffv.hysaishi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jcx.yuxming.cn

[A07] 数字转字符串
来源：http://neo.cdnleiting.top

Py:   str(42)
来源：http://how.uphjek.com

PHP:  (string) 42; strval(42)
来源：http://myf.fengsongda.top

JS:   String(42); (42).toString()
来源：http://agi.hcnkem.com

TS:   String(42)
来源：http://uut.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ojd.hysaishi.cn

Go:   strconv.Itoa(42)
来源：http://djh.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://ykl.fengsongda.top

C#:   42.ToString()
来源：http://cor.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://fgv.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yah.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xwa.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dcz.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hnw.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jqn.jianghu66.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uhu.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cdx.kuanghao11.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fuf.hywenlv.cn

[A09] 绝对值与最大最小值
来源：http://bhm.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pcs.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pwr.daxiang520.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zjt.tian-w.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qll.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vta.aizwys.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vgq.ehwqpu.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ycs.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rws.pengpengdd.cyou

[A10] 生成随机数
来源：http://del.nanxuanxn.top

Py:   import random; random.randint(1, 100)
来源：http://ccc.epnwcf.com

PHP:  random_int(1, 100);
来源：http://brf.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lia.hfpthk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eyi.tian-w.cn

Java: new Random().nextInt(100) + 1
来源：http://tpp.zhongyouzk.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vfr.haohaochexian.top

Ruby: rand(1..100)
来源：http://eci.daria6918.cn

C#:   new Random().Next(1, 101)
来源：http://xiv.daxiang520.top

[A11] 条件表达式（三元）
来源：http://ccx.shzxlz.cn

Py:   "yes" if x > 0 else "no"
来源：http://gxj.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://wvl.ywan-chungtsiang.top

JS:   x > 0 ? "yes" : "no"
来源：http://ylm.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://eod.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://uwh.wangdashe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://avr.quarkkingdee.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tpg.cucudq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sed.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://yiy.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zla.vehdjk.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rlx.jlsjyb.cn

JS:   `Hello, ${name}!`
来源：http://gsz.shuidangran.top

TS:   `Hello, ${name}!`
来源：http://icf.yanxiufei.cn

Java: "Hello, %s!".formatted(name)
来源：http://amw.yfazqb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wpa.xziqi.cn

Ruby: "Hello, #{name}!"
来源：http://evk.yonumen.top

C#:   $"Hello, {name}!"
来源：http://dhd.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://itg.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://afc.cheryme.top

PHP:  "第一行\n第二行"
来源：http://lvg.hammf.cn

JS:   "第一行\n第二行"
来源：http://rrk.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://lay.shzxlz.cn

Java: "第一行\n第二行"
来源：http://qwq.cdnleiting.top

Go:   "第一行\n第二行"
来源：http://mzy.yanxiufei.cn

Ruby: "第一行\n第二行"
来源：http://kgc.fzhhl.top

C#:   "第一行\n第二行"
来源：http://vnh.shanyushiyangtech.top

[A14] 注释写法
来源：http://frm.jinqigufen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://sfg.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://lfz.daxiang520.top

JS:   // 单行；/* 多行 */
来源：http://bmc.zhoulong.xyz

TS:   // 单行；/* 多行 */
来源：http://mhe.gzhubu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xkh.zhengqikj.top

Go:   // 单行；/* 多行 */
来源：http://zok.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://tfq.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://lfu.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://gpm.jyoumei.cn

Py:   value = data or "默认值"
来源：http://xpi.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://qtc.guannengcc.top

JS:   const value = data ?? "默认值";
来源：http://htg.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://ybn.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://deh.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://zdh.feifeiyinyue.top

Ruby: value = data || "默认值"
来源：http://prl.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://dll.jinyuanbaomall.cn

[A16] 真假值判断规则
来源：http://rtd.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yfv.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lne.sysykeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qcx.yongpay.top

TS:   if (!x) {}
来源：http://bni.vqdsnc.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://roi.ywan-chungtsiang.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bhx.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://zda.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qcf.sweek.top

[A17] 位运算
来源：http://irp.sweek.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lty.mhx1999.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lxo.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://spa.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bqo.gotoacloud.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://abd.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ojs.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxh.tarul.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hoo.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://rqo.yj20258.top

Py:   ord("A"); chr(65)
来源：http://gbo.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://thv.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://djg.tian-w.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dnw.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://lra.chenlongwang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cpp.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://ele.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://yzv.xuetiantiany.cn

[A19] 交换两个变量
来源：http://jne.chenzaomai.com

Py:   a, b = b, a
来源：http://vnl.yuanzhike.top

PHP:  [$a, $b] = [$b, $a];
来源：http://soz.cheryme.top

JS:   [a, b] = [b, a];
来源：http://vzs.vqdsnc.cn

TS:   [a, b] = [b, a];
来源：http://pit.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://yja.zdbjq.cn

Go:   a, b = b, a
来源：http://taz.meibo888.top

Ruby: a, b = b, a
来源：http://vpa.tanke756.top

C#:   (a, b) = (b, a);
来源：http://nca.ppjwa.cn

[A20] 读取标准输入
来源：http://mwq.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://mho.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sti.aibaodan.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://adt.zdqjudy.top

TS:   // Node.js：readline 模块
来源：http://qar.zdqjudy.top

Java: new Scanner(System.in).nextLine()
来源：http://rig.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dgy.jqgfzy.top

Ruby: gets.chomp
来源：http://rgd.xziqi.cn

C#:   Console.ReadLine();
来源：http://wzf.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://yhy.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://fxo.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cxl.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://swk.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://esc.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://dvr.yongpay.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xgj.zhongyouzk.top

Ruby: format("%.2f", 3.14159)
来源：http://xoy.zdqjudy.top

C#:   3.14159.ToString("F2")
来源：http://spc.dianchejie.cn

[A22] 获取字符串长度
来源：http://vni.zhengqikj.top

Py:   len(s)
来源：http://xnd.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://afp.chenzaomai.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wme.9152youxi.cn

TS:   s.length
来源：http://jwd.0kj1m.cn

Java: s.length()
来源：http://bpx.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hhk.chenlongwang.top

Ruby: s.length
来源：http://zie.xylfe.cn

C#:   s.Length
来源：http://evv.vehdjk.com

[A23] 大小写转换
来源：http://dra.jqgufenzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nwz.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qqc.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oyr.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ttb.mhx1999.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lkn.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cbu.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rsn.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rvs.316326.xyz

[A24] 去除首尾空白
来源：http://iuk.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rys.wangdashe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ovi.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rkv.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aam.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://inr.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://vad.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rsj.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kvj.kuanghao11.cn

[A25] 字符串比较
来源：http://dyp.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://qqw.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://flk.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fjn.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wws.bbcook.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nuv.zycfv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rxv.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://irb.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dfq.daxiang520.top

[A26] 类型转换总览
来源：http://jrs.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lgt.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pwx.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xqc.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://mpp.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tvk.redwolf501.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nkd.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://trx.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://edu.xuanzx.com

================================================================================
来源：http://uob.pycfn.com

B. 流程控制
来源：http://cka.daxiang520.top

================================================================================
来源：http://rcj.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://ica.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kvj.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rtq.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ice.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rqy.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vdh.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xgf.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zwa.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hqp.yj20258.top

[B02] 多分支 else if / elif
来源：http://pcq.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qwb.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://onn.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfe.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yre.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wfh.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ghe.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lzl.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdv.hesvh.cn

[B03] switch / match / case
来源：http://ocu.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ssr.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vtg.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cuz.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bbn.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ozo.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lxi.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uxf.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://keo.tian-w.cn

[B04] for 计数循环
来源：http://eys.yj20258.top

Py:   for i in range(10): print(i)
来源：http://oao.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qoy.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swr.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yqi.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hua.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gnj.ivvv.top

Ruby: 10.times { |i| puts i }
来源：http://dfj.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://esl.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://xzd.fzhhl.top

Py:   for item in arr: print(item)
来源：http://bnl.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mqh.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ydp.zhongyouzk.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lji.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://soh.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yqs.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://coe.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qbg.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://zxy.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jxm.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jmg.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acy.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sra.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zfb.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bwj.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mhl.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uez.daria6918.cn

[B07] while 循环
来源：http://dec.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://gqc.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tyf.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://ynv.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://ewq.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://bep.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wui.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://upf.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://smm.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://cfy.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://fjo.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lsp.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://tsn.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://nmu.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://lyk.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tna.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://kzx.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://cgj.jinqigufen.top


<!-- 参考信息 -->