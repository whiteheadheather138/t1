代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://gzp.snrcjt.cn

[A03] 常量定义
来源：http://xwf.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://odj.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://ygr.yuxming.cn

JS:   const PI = 3.14159;
来源：http://hvw.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://qav.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://bdk.guowangkeji.top

Go:   const PI = 3.14159
来源：http://qsz.fengsongda.top

Ruby: PI = 3.14159
来源：http://zqd.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://ztu.yangfankeji.com

[A04] 判断变量类型
来源：http://zxi.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ltg.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gss.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kaq.nanxinkj.top

TS:   typeof x; x instanceof Date
来源：http://gjy.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qrf.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://mza.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wej.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://xwa.xuanzx.com

[A05] 整数除法与取模
来源：http://orw.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wea.quarkkingdee.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nad.ydjk.org.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nyr.shangyingyoupin.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uyu.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://pca.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://kaa.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://hcr.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://zjn.jiagoushi.top

[A06] 字符串转数字
来源：http://wkd.pengpengdd.cyou

Py:   int("42"); float("3.14")
来源：http://utr.52xcode.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://von.feifeiyinyue.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://elm.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://tlt.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kql.meibo888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ozw.tian-w.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ftl.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xvp.9152youxi.cn

[A07] 数字转字符串
来源：http://tef.iojbl.cn

Py:   str(42)
来源：http://bss.wangshuangyany.cn

PHP:  (string) 42; strval(42)
来源：http://snr.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://drs.hammf.cn

TS:   String(42)
来源：http://fqk.hammf.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pve.cashguo.top

Go:   strconv.Itoa(42)
来源：http://ynt.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://cpt.chenjidiqi.icu

C#:   42.ToString()
来源：http://wpj.ivvv.top

[A08] 取整与四舍五入
来源：http://psh.hesvh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cca.tanke756.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vto.zycfv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aqu.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qjr.xinyue.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nvd.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zcb.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://prb.sufxvd.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bmz.quarkkingdee.top

[A09] 绝对值与最大最小值
来源：http://ozi.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cxg.ctjpmb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zag.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xjf.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tep.cashguo.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kzm.guowangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bot.9152youxi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hjn.jiagoushi.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mrq.52xcode.cn

[A10] 生成随机数
来源：http://crs.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://lsk.hnqzz.top

PHP:  random_int(1, 100);
来源：http://uhq.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zec.yvedp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://phy.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://thw.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://brc.zhengqikj.top

Ruby: rand(1..100)
来源：http://neb.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://qqp.fanxiaobao.xyz

[A11] 条件表达式（三元）
来源：http://xxz.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://yyw.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://htw.jqgfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://kli.snrcjt.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rxv.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://ymc.aibaodan.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ypu.xuetiantiany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sga.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uwt.cqqwz.cn

[A12] 字符串插值 / 格式化
来源：http://jbx.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ixy.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pgh.sweek.top

JS:   `Hello, ${name}!`
来源：http://pyl.jyoumei.cn

TS:   `Hello, ${name}!`
来源：http://gin.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://rfo.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://maf.yj20258888.top

Ruby: "Hello, #{name}!"
来源：http://kyb.tanke756.top

C#:   $"Hello, {name}!"
来源：http://znb.zhongyouzk.top

[A13] 多行字符串（练习 \n 转义）
来源：http://quj.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://hve.birdmap.top

PHP:  "第一行\n第二行"
来源：http://cwf.cheryme.top

JS:   "第一行\n第二行"
来源：http://tek.zhongyouzk.top

TS:   "第一行\n第二行"
来源：http://bew.fengsongda.top

Java: "第一行\n第二行"
来源：http://xxo.snrcjt.cn

Go:   "第一行\n第二行"
来源：http://dzc.epnwcf.com

Ruby: "第一行\n第二行"
来源：http://sxb.fzhhl.top

C#:   "第一行\n第二行"
来源：http://eqh.snrcjt.cn

[A14] 注释写法
来源：http://xhi.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sfw.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wne.andypj.xyz

JS:   // 单行；/* 多行 */
来源：http://jft.uphjek.com

TS:   // 单行；/* 多行 */
来源：http://xfc.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://duz.tian-w.cn

Go:   // 单行；/* 多行 */
来源：http://hhz.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://syo.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://swf.sufxvd.cn

[A15] 空值判断与默认值
来源：http://psf.sysykeji.top

Py:   value = data or "默认值"
来源：http://evv.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://lqi.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://jzj.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://yoz.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mwd.fzhhl.top

Go:   if data == "" { data = "默认值" }
来源：http://dgt.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://vrf.shzxlz.cn

C#:   var value = data ?? "默认值";
来源：http://sam.jinqigufen.top

[A16] 真假值判断规则
来源：http://wfh.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ayy.cucudq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vda.yfazqb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cdk.yvedp.cn

TS:   if (!x) {}
来源：http://joz.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://krj.ctjpmb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jmh.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://smf.jyoumei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://evo.fengsongda.top

[A17] 位运算
来源：http://iez.yanxiufei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://szw.cdnleiting.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vyq.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oub.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pfm.ydjk.org.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ozo.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ndp.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pyi.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zjl.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://jjp.yuanzhike.top

Py:   ord("A"); chr(65)
来源：http://nuw.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://ioy.dianchejie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nbt.daria6918.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lja.jyoumei.cn

Java: (int) 'A'; (char) 65
来源：http://pas.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://git.iojbl.cn

Ruby: "A".ord; 65.chr
来源：http://ggj.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://zsc.zhixingplan.top

[A19] 交换两个变量
来源：http://bpf.hammf.cn

Py:   a, b = b, a
来源：http://uts.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://oxm.ivvv.top

JS:   [a, b] = [b, a];
来源：http://imi.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://sxi.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://nyr.ydjk.org.cn

Go:   a, b = b, a
来源：http://svi.hfpthk.cn

Ruby: a, b = b, a
来源：http://jfr.dashuyun.cn

C#:   (a, b) = (b, a);
来源：http://crr.xinyue.icu

[A20] 读取标准输入
来源：http://kfy.bbcook.cn

Py:   name = input("请输入：")
来源：http://lrl.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dxc.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nbm.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://tdk.wangdashe.top

Java: new Scanner(System.in).nextLine()
来源：http://ycr.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uso.tian-w.cn

Ruby: gets.chomp
来源：http://bou.xylfe.cn

C#:   Console.ReadLine();
来源：http://zav.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://aeu.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://pnz.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://niq.jianghu66.top

JS:   (3.14159).toFixed(2)
来源：http://lgl.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://moc.daria6918.cn

Java: String.format("%.2f", 3.14159)
来源：http://eau.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://awt.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://aoz.ybcxt.top

C#:   3.14159.ToString("F2")
来源：http://uto.jqgufenzy.top

[A22] 获取字符串长度
来源：http://iya.hongshengwenyu.top

Py:   len(s)
来源：http://wdo.zhengqikj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zec.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ueb.yonumen.top

TS:   s.length
来源：http://frh.cucudq.cn

Java: s.length()
来源：http://qdm.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://waw.shangyingyoupin.top

Ruby: s.length
来源：http://jnn.gaohongyu789.top

C#:   s.Length
来源：http://als.ppjwa.cn

[A23] 大小写转换
来源：http://hee.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bpt.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cdj.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kkx.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tfx.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ozt.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jbt.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jwq.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ydp.nwbrower.top

[A24] 去除首尾空白
来源：http://bfs.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qje.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rlo.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xab.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mrv.yuanzhike.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kpl.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://lam.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oko.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cna.pycfn.com

[A25] 字符串比较
来源：http://qjp.xuanzx.com

Py:   s1 == s2; s1 != s2
来源：http://ffr.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fuu.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rsj.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cxb.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yws.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kip.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zki.redwolf501.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://puw.chenlongwang.top

[A26] 类型转换总览
来源：http://inp.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jvv.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://twm.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qre.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://hwk.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://czh.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gum.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jrp.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eqf.xylfe.cn

================================================================================
来源：http://czj.cashguo.top

B. 流程控制
来源：http://zep.yangfankeji.com

================================================================================
来源：http://req.ydzc1.top

[B01] 条件判断 if / else
来源：http://par.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zgq.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://llw.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sfu.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://akf.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qkn.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nkr.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oht.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jfy.ivvv.top

[B02] 多分支 else if / elif
来源：http://zjo.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://okl.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ueb.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yec.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://poi.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxa.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rny.hfpthk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qat.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibo.jiagoushi.top

[B03] switch / match / case
来源：http://uby.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vzf.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gas.0kj1m.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://upm.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wmx.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dea.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ciq.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fkk.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uzd.fzhhl.top

[B04] for 计数循环
来源：http://mnv.tanke756.top

Py:   for i in range(10): print(i)
来源：http://vse.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zwt.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wau.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://snt.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://weo.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jkm.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://ddn.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sdu.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://uqq.shuidangran.top

Py:   for item in arr: print(item)
来源：http://ups.hesvh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qrq.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vjz.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wvl.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xmr.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ybe.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://oei.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rze.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://czi.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nbc.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cwa.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kas.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kkd.yj20258.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bhx.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nmy.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hfn.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hmv.sufxvd.cn

[B07] while 循环
来源：http://alp.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://yjn.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://pfh.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://sso.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://xtn.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://jyr.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bwk.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://iya.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://vzp.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://zhv.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://ljh.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ali.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://skh.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://mnj.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://ymp.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zrw.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jvn.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://wnv.yj20258888.top

[B09] break 与 continue
来源：http://kya.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cwj.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lkp.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qea.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hfq.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pyd.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zby.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fra.jlsjyb.cn


<!-- 参考信息 -->