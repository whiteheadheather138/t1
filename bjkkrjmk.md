代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://jtq.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://fpp.xuanzx.com

C#:   x.GetType().Name; x is int
来源：http://pze.dianchejie.cn

[A05] 整数除法与取模
来源：http://cke.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kem.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vle.vqdsnc.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fqx.c1oappe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nxc.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://ohm.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://kqq.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://fek.ctjpmb.com

C#:   7 / 2; 7 % 2
来源：http://uhk.hammf.cn

[A06] 字符串转数字
来源：http://xnj.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://yvb.gaohongyu789.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ewt.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tbj.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://mgl.yj20258888.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cok.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ecf.yonumen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pka.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kbi.jqgufenzy.top

[A07] 数字转字符串
来源：http://hbs.yfazqb.com

Py:   str(42)
来源：http://jre.hysaishi.cn

PHP:  (string) 42; strval(42)
来源：http://cjq.guowangkeji.top

JS:   String(42); (42).toString()
来源：http://ezx.guannengcc.top

TS:   String(42)
来源：http://pje.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hce.shanyushiyangtech.top

Go:   strconv.Itoa(42)
来源：http://fiw.ehwqpu.com

Ruby: 42.to_s
来源：http://vmq.xziqi.cn

C#:   42.ToString()
来源：http://cfu.bjfxy.top

[A08] 取整与四舍五入
来源：http://drs.hfpthk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yci.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hvn.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xsa.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uas.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pqt.vehdjk.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://otb.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bem.nanxinkj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kmp.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://mxx.yfazqb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uba.jlsjyb.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://esw.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pog.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wpi.52xcode.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nkf.hammf.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dta.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nzc.cqqwz.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ebs.xylfe.cn

[A10] 生成随机数
来源：http://ufc.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://jje.jinqigufen.top

PHP:  random_int(1, 100);
来源：http://vtw.havefunace.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qdj.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cta.yongpay.top

Java: new Random().nextInt(100) + 1
来源：http://bmx.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ete.0kj1m.cn

Ruby: rand(1..100)
来源：http://fwe.wangshuangyany.cn

C#:   new Random().Next(1, 101)
来源：http://iof.cucudq.cn

[A11] 条件表达式（三元）
来源：http://kjl.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://ile.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://cwu.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://tdw.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://ocd.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://acz.ctjpmb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://bmx.tian-w.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://scb.c1oappe.top

C#:   x > 0 ? "yes" : "no"
来源：http://eor.daxiang520.top

[A12] 字符串插值 / 格式化
来源：http://cvx.jinqigfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aqm.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xtd.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://pxl.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://roe.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://lav.zhijiandao.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://myh.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://ila.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://czj.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://tmt.ydzc1.top

Py:   "第一行\n第二行"
来源：http://ntr.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://qaz.sysykeji.top

JS:   "第一行\n第二行"
来源：http://brs.hywenlv.cn

TS:   "第一行\n第二行"
来源：http://bwq.chenzaomai.com

Java: "第一行\n第二行"
来源：http://lyp.daria6918.cn

Go:   "第一行\n第二行"
来源：http://qhp.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://ipn.shuidangran.top

C#:   "第一行\n第二行"
来源：http://xnv.sysykeji.top

[A14] 注释写法
来源：http://dno.tian-w.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qys.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qxi.yvedp.cn

JS:   // 单行；/* 多行 */
来源：http://cyf.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://mnx.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lqc.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://csd.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://itk.hysaishi.cn

C#:   // 单行；/* 多行 */
来源：http://hrl.zdbjq.cn

[A15] 空值判断与默认值
来源：http://lhd.ppjwa.cn

Py:   value = data or "默认值"
来源：http://xgo.zycfv.cn

PHP:  $value = $data ?? "默认值";
来源：http://gap.svipenyu.cn

JS:   const value = data ?? "默认值";
来源：http://jyg.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://isx.wangdashe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tkq.ybcxt.top

Go:   if data == "" { data = "默认值" }
来源：http://wdv.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://lwg.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://opo.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://slr.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://prb.bjfxy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zzo.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://arv.jinghuilouyu.cn

TS:   if (!x) {}
来源：http://lkk.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ydy.daxiang520.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://syv.ydzc1.top

Ruby: unless x            # nil 与 false 为假
来源：http://zrf.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nvr.zhaomingkeji.xyz

[A17] 位运算
来源：http://vol.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aao.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sxg.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvf.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wbs.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rva.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zqt.shangyingyoupin.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgd.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ltz.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://stj.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://nqq.tanke756.top

PHP:  ord("A"); chr(65)
来源：http://hqr.cheryme.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zwt.jqgufenzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tyn.sysykeji.top

Java: (int) 'A'; (char) 65
来源：http://ztu.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fnh.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://tvr.gaohongyu789.top

C#:   (int)'A'; (char)65
来源：http://fzd.hnxiangtu.top

[A19] 交换两个变量
来源：http://xsg.shuidangran.top

Py:   a, b = b, a
来源：http://nox.zdqjudy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://frv.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://lwg.zycfv.cn

TS:   [a, b] = [b, a];
来源：http://gnp.aizwys.cn

Java: int t = a; a = b; b = t;
来源：http://max.vehdjk.com

Go:   a, b = b, a
来源：http://bqf.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://plw.shuidangran.top

C#:   (a, b) = (b, a);
来源：http://wwl.dashuyun.cn

[A20] 读取标准输入
来源：http://fwy.chenjidiqi.icu

Py:   name = input("请输入：")
来源：http://qou.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yec.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jwn.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://atl.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://hzt.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yny.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://enu.cucudq.cn

C#:   Console.ReadLine();
来源：http://pma.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://obd.pycfn.com

Py:   f"{3.14159:.2f}"
来源：http://vge.hesvh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yua.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://kwd.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://szf.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://shd.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pet.jiagoushi.top

Ruby: format("%.2f", 3.14159)
来源：http://gdk.yongpay.top

C#:   3.14159.ToString("F2")
来源：http://fyu.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://lqh.tianlin.xyz

Py:   len(s)
来源：http://pfr.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://seg.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jqq.wangdashe.top

TS:   s.length
来源：http://ous.shanyushiyangkeji.top

Java: s.length()
来源：http://bmz.yvedp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tsw.hnqzz.top

Ruby: s.length
来源：http://ynd.ivvv.top

C#:   s.Length
来源：http://mcl.ybcxt.top

[A23] 大小写转换
来源：http://giz.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nyy.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ifg.zdqjudy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wym.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dbb.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cgv.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fxv.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zqy.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kke.gzhubu.top

[A24] 去除首尾空白
来源：http://tkt.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hxw.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://azu.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wyb.iojbl.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shf.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dnr.hnqzz.top

Go:   strings.TrimSpace(s)
来源：http://gxw.fktsv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jyj.ybcxt.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://olc.gzhubu.top

[A25] 字符串比较
来源：http://kpw.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://gtn.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sqq.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xim.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rgl.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ibv.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wmr.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://daa.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hid.sxryk.cn

[A26] 类型转换总览
来源：http://vqh.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://opg.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gdm.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zji.chenzaomai.com

TS:   Number() String() Boolean() x as number
来源：http://qlf.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qyq.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fss.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://oco.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kfs.haohaochexian.top

================================================================================
来源：http://aew.zhiwuduotai.top

B. 流程控制
来源：http://gru.cashguo.top

================================================================================
来源：http://rmk.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://xgl.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pds.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://inl.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vdt.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kvw.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ill.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qrs.nanxuanxn.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bzf.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bgi.wangdashe.top

[B02] 多分支 else if / elif
来源：http://yoq.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jjq.yueranfly.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fgp.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ota.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxp.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://amj.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://enj.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xzf.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vob.fanxiaobao.xyz

[B03] switch / match / case
来源：http://poj.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zzi.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://icg.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kjd.52xcode.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oph.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ddn.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eiv.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jek.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rts.jiagoushi.top

[B04] for 计数循环
来源：http://yfg.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://ndz.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kkr.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wdb.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxn.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pew.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dzz.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://skh.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://adk.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://jdz.smart0.xyz

Py:   for item in arr: print(item)
来源：http://gsg.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://trt.vqdsnc.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bah.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yij.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://xsj.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sgi.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://wps.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bzl.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://bgr.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://urq.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uxf.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mgs.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gzg.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tjp.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lkk.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tec.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gaq.9152youxi.cn

[B07] while 循环
来源：http://mhb.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://gai.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://jlq.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://xjk.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://lut.hammf.cn

Java: while (i < 10) { i++; }
来源：http://mes.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lfj.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://gnz.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://xmf.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://uha.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://uwg.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uyq.xuanzx.com

JS:   do { i++; } while (i < 10);
来源：http://aoz.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://rvl.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://fka.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hsa.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://msl.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://dro.yangfankeji.com

[B09] break 与 continue
来源：http://sur.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sye.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://plh.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwe.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvn.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfa.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bpy.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yyh.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wcj.daxiang520.top

[B10] 遍历同时拿索引
来源：http://wis.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bwy.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zqt.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fjr.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bpi.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rqh.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://amx.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yiz.tanke756.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fuu.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://yni.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://fsg.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://jzd.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogo.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cif.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dqw.jyoumei.cn


<!-- 参考信息 -->