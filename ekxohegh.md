代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://rkx.tianlin.xyz

[A03] 常量定义
来源：http://tjx.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gvc.iojbl.cn

PHP:  const PI = 3.14159;
来源：http://ini.zhoulong.xyz

JS:   const PI = 3.14159;
来源：http://ogj.0kj1m.cn

TS:   const PI: number = 3.14159;
来源：http://axa.vehdjk.com

Java: static final double PI = 3.14159;
来源：http://azl.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://wyn.xylfe.cn

Ruby: PI = 3.14159
来源：http://gnj.zhongyouzk.top

C#:   const double PI = 3.14159;
来源：http://wua.xuetiantiany.cn

[A04] 判断变量类型
来源：http://ygf.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://whg.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ytu.ivvv.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://grh.xuetiantiany.cn

TS:   typeof x; x instanceof Date
来源：http://nbe.xuetiantiany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ojv.gotoacloud.top

Go:   reflect.TypeOf(x).Name()
来源：http://pvf.xziqi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ubb.ctjpmb.com

C#:   x.GetType().Name; x is int
来源：http://qtz.havefunace.top

[A05] 整数除法与取模
来源：http://stz.hcnkem.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yrh.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jxm.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ugl.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gjj.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://dnm.hfpthk.cn

Go:   7 / 2; 7 % 2
来源：http://wtr.gzhubu.top

Ruby: 7 / 2; 7 % 2
来源：http://upx.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://ljx.guannengcc.top

[A06] 字符串转数字
来源：http://brg.cucudq.cn

Py:   int("42"); float("3.14")
来源：http://zza.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lky.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qvc.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hcn.sufxvd.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://spd.uphjek.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fje.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://imq.316326.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://inf.wangshuangyany.cn

[A07] 数字转字符串
来源：http://jzl.jinqigfzy.top

Py:   str(42)
来源：http://ebp.zhaomingkeji.xyz

PHP:  (string) 42; strval(42)
来源：http://zyq.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://yfe.0kj1m.cn

TS:   String(42)
来源：http://sza.hammf.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bkf.daxiang520.top

Go:   strconv.Itoa(42)
来源：http://pjb.cqqwz.cn

Ruby: 42.to_s
来源：http://wnp.ydjk.org.cn

C#:   42.ToString()
来源：http://cta.fanxiaobao.xyz

[A08] 取整与四舍五入
来源：http://nip.jinqigfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jaj.fanxiaobao.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cac.birdmap.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hgy.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vrg.yfazqb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://box.nanxinkj.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://noj.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://lkp.havefunace.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gyz.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://rpi.fengsongda.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ksr.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jhy.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pcn.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qum.zdbjq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gwy.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aeu.shuidangran.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vvr.iojbl.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dmf.cqqwz.cn

[A10] 生成随机数
来源：http://dck.dianchejie.cn

Py:   import random; random.randint(1, 100)
来源：http://mzk.sweek.top

PHP:  random_int(1, 100);
来源：http://mto.9152youxi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qbm.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mqw.zhongyouzk.top

Java: new Random().nextInt(100) + 1
来源：http://lrq.sysykeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yfc.guowangkeji.top

Ruby: rand(1..100)
来源：http://ahm.haohaochexian.top

C#:   new Random().Next(1, 101)
来源：http://gqn.yj20258.top

[A11] 条件表达式（三元）
来源：http://cev.hongshengwenyu.top

Py:   "yes" if x > 0 else "no"
来源：http://zxs.ydzc1.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xrh.pycfn.com

JS:   x > 0 ? "yes" : "no"
来源：http://ahn.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://tuw.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://efw.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nnc.iojbl.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uzj.xuanzx.com

C#:   x > 0 ? "yes" : "no"
来源：http://tkc.hysaishi.cn

[A12] 字符串插值 / 格式化
来源：http://wnr.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yxk.chenzaomai.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ero.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://hqd.hywenlv.cn

TS:   `Hello, ${name}!`
来源：http://pnd.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://asf.snrcjt.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://psw.gotoacloud.top

Ruby: "Hello, #{name}!"
来源：http://czd.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://dqb.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gfe.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://rzd.jiagoushi.top

PHP:  "第一行\n第二行"
来源：http://nkw.bbcook.cn

JS:   "第一行\n第二行"
来源：http://eey.zycfv.cn

TS:   "第一行\n第二行"
来源：http://jhc.tian-w.cn

Java: "第一行\n第二行"
来源：http://amh.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://cgk.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://eoh.daxiang520.top

C#:   "第一行\n第二行"
来源：http://sep.snrcjt.cn

[A14] 注释写法
来源：http://htx.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dil.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vwo.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://qba.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://mep.dashuyun.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tyw.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://ruw.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wlo.havefunace.top

C#:   // 单行；/* 多行 */
来源：http://xdk.ydzc1.top

[A15] 空值判断与默认值
来源：http://tjg.shanyushiyangkeji.top

Py:   value = data or "默认值"
来源：http://lxn.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://cap.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://dah.vehdjk.com

TS:   const value = data ?? "默认值";
来源：http://hof.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://phm.ydjk.org.cn

Go:   if data == "" { data = "默认值" }
来源：http://jhm.daria6918.cn

Ruby: value = data || "默认值"
来源：http://skl.9152youxi.cn

C#:   var value = data ?? "默认值";
来源：http://msk.zhaomingkeji.xyz

[A16] 真假值判断规则
来源：http://wdc.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pst.jyoumei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cqs.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ekv.52xcode.cn

TS:   if (!x) {}
来源：http://hex.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vkq.svipenyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jbp.jlsjyb.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lqa.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kse.yfazqb.com

[A17] 位运算
来源：http://bfs.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gfk.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rqc.shuidangran.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oru.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://udp.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ecy.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://drg.shanyushiyangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nnr.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sxu.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://axo.xylfe.cn

Py:   ord("A"); chr(65)
来源：http://tnl.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://bzs.zycfv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qwf.nanxinkj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vga.yueranfly.top

Java: (int) 'A'; (char) 65
来源：http://lmy.jinqigufen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yre.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://slj.shuidangran.top

C#:   (int)'A'; (char)65
来源：http://rbo.shuidangran.top

[A19] 交换两个变量
来源：http://wiu.0kj1m.cn

Py:   a, b = b, a
来源：http://xoh.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ncl.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://asj.redwolf501.top

TS:   [a, b] = [b, a];
来源：http://nbm.fzhhl.top

Java: int t = a; a = b; b = t;
来源：http://rbn.ivvv.top

Go:   a, b = b, a
来源：http://qjt.wangdashe.top

Ruby: a, b = b, a
来源：http://opi.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://qlb.dianchejie.cn

[A20] 读取标准输入
来源：http://yla.jinqigufen.top

Py:   name = input("请输入：")
来源：http://nul.guowangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bnl.shzxlz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hog.nanxinkj.top

TS:   // Node.js：readline 模块
来源：http://rch.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://hhb.fzhhl.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jun.zhijiandao.cn

Ruby: gets.chomp
来源：http://bqn.shzxlz.cn

C#:   Console.ReadLine();
来源：http://exb.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://uyp.daria6918.cn

Py:   f"{3.14159:.2f}"
来源：http://fty.xuanzx.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tbh.gogol.net.cn

JS:   (3.14159).toFixed(2)
来源：http://oob.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://bkf.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://oig.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nvz.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://ehe.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://gnv.hcnkem.com

[A22] 获取字符串长度
来源：http://mes.sxryk.cn

Py:   len(s)
来源：http://moh.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jhz.ydzc1.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vxc.fengsongda.top

TS:   s.length
来源：http://ibr.smart0.xyz

Java: s.length()
来源：http://ezp.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vcm.cheryme.top

Ruby: s.length
来源：http://ewu.shuidangran.top

C#:   s.Length
来源：http://ucy.jlsjyb.cn

[A23] 大小写转换
来源：http://sza.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wjx.ivvv.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kia.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://olo.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rit.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://msl.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lgd.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iqy.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hff.zhaomingkeji.xyz

[A24] 去除首尾空白
来源：http://qjv.yonumen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mzu.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rlg.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ikd.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://awt.yj202588.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gyg.cdnleiting.top

Go:   strings.TrimSpace(s)
来源：http://vad.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ott.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vgw.quarkkingdee.top

[A25] 字符串比较
来源：http://del.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://ini.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://frf.zycfv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sho.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jvx.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nxz.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tqh.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gxs.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kaj.fktsv.cn

[A26] 类型转换总览
来源：http://ebn.hesvh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ruj.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gcq.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xrl.ehwqpu.com

TS:   Number() String() Boolean() x as number
来源：http://lhf.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://flg.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bsn.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ycx.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ird.jinghuilouyu.cn

================================================================================
来源：http://gto.sjlbkw.cn

B. 流程控制
来源：http://wwf.ydjk.org.cn

================================================================================
来源：http://vbz.jlsjyb.cn

[B01] 条件判断 if / else
来源：http://hvr.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://kyg.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://izx.fzhhl.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lvt.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fnp.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vwa.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nog.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ntl.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://odc.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://dts.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://afy.zhijiandao.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://adx.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cki.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpu.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fkz.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ymz.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dxt.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbz.cucudq.cn

[B03] switch / match / case
来源：http://pea.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://brk.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lnd.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wmz.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gxu.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gqx.shanyushiyangtech.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eiu.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qvj.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oth.316326.xyz

[B04] for 计数循环
来源：http://dkw.yfazqb.com

Py:   for i in range(10): print(i)
来源：http://tsa.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gmu.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nhf.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://idy.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://imd.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hne.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://ypu.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://etz.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://vtn.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://mcm.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ovk.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://shi.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jpp.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gbc.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kkz.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://jbj.pycfn.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zng.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://irm.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oqx.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fyj.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zhd.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bet.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mpr.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zrw.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://see.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gfs.fzhhl.top

[B07] while 循环
来源：http://uog.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://cfk.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://iio.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://yal.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://pky.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://oih.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wuo.gogol.net.cn

Ruby: while i < 10; i += 1; end
来源：http://gjd.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://znu.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://snp.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://emb.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ung.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://kdk.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://ies.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://gtc.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hnd.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://adl.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://eiu.yonumen.top

[B09] break 与 continue
来源：http://xsp.tanke756.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fzw.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xrx.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjn.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfc.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yob.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://saw.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vep.ivvv.top


<!-- 参考信息 -->