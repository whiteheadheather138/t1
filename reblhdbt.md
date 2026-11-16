代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pvh.dianchejie.cn

Java: String name = "Alex"; int age = 20;
来源：http://lkk.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://qhu.ppjwa.cn

Ruby: name = "Alex"; age = 20
来源：http://wvy.wangdashe.top

C#:   string name = "Alex"; int age = 20;
来源：http://ija.zhengqikj.top

[A03] 常量定义
来源：http://kfl.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cmr.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://hic.yfazqb.com

JS:   const PI = 3.14159;
来源：http://qcn.jlsjyb.cn

TS:   const PI: number = 3.14159;
来源：http://edx.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://aed.jinqigufen.top

Go:   const PI = 3.14159
来源：http://dds.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://oge.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://jcw.gotoacloud.top

[A04] 判断变量类型
来源：http://oba.redwolf501.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://imk.zycfv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zhu.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oew.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://gdg.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xpp.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://vhn.chenlongwang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gxe.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://uxv.fzhhl.top

[A05] 整数除法与取模
来源：http://gge.kuanghao11.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kdg.shzxlz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qpa.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zto.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aok.sweek.top

Java: 7 / 2; 7 % 2
来源：http://ezu.zhijiandao.cn

Go:   7 / 2; 7 % 2
来源：http://tgo.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://npb.pengpengdd.cyou

C#:   7 / 2; 7 % 2
来源：http://htc.yanxiufei.cn

[A06] 字符串转数字
来源：http://bjo.hesvh.cn

Py:   int("42"); float("3.14")
来源：http://czb.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ycu.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qcs.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://keo.jyoumei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://een.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nli.316326.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://zta.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aih.yonumen.top

[A07] 数字转字符串
来源：http://xjd.xylfe.cn

Py:   str(42)
来源：http://mmy.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://wrd.sysykeji.top

JS:   String(42); (42).toString()
来源：http://qes.pycfn.com

TS:   String(42)
来源：http://hjy.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dcm.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://gzi.ybcxt.top

Ruby: 42.to_s
来源：http://vns.jiagoushi.top

C#:   42.ToString()
来源：http://sij.sufxvd.cn

[A08] 取整与四舍五入
来源：http://phm.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gon.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xqv.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wju.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bfo.guowangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fnz.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ola.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rog.ydzc1.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zrk.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://wbo.zhijiandao.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hdb.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://orx.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gha.mhx1999.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ity.sxryk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gjw.mhx1999.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pnj.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hal.zhiwuduotai.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pka.yongpay.top

[A10] 生成随机数
来源：http://bkc.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://gnb.vehdjk.com

PHP:  random_int(1, 100);
来源：http://svl.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ggb.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yqb.fengsongda.top

Java: new Random().nextInt(100) + 1
来源：http://qfw.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pjd.jqgfzy.top

Ruby: rand(1..100)
来源：http://eco.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://qfe.sjlbkw.cn

[A11] 条件表达式（三元）
来源：http://loz.xylfe.cn

Py:   "yes" if x > 0 else "no"
来源：http://pru.hesvh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tsy.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eiz.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://phu.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://ozk.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dmk.aizwys.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lql.zhixingplan.top

C#:   x > 0 ? "yes" : "no"
来源：http://ylc.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://gwb.wangdashe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hsc.shanyushiyangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uwj.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://hed.meibo888.top

TS:   `Hello, ${name}!`
来源：http://mnm.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://dtr.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tqa.ydzc1.top

Ruby: "Hello, #{name}!"
来源：http://blt.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://xze.jyoumei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jbd.daria6918.cn

Py:   "第一行\n第二行"
来源：http://zom.ywan-chungtsiang.top

PHP:  "第一行\n第二行"
来源：http://pmz.tarul.cn

JS:   "第一行\n第二行"
来源：http://xgb.hcnkem.com

TS:   "第一行\n第二行"
来源：http://gyv.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://whk.wangdashe.top

Go:   "第一行\n第二行"
来源：http://ibq.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://ncx.bjfxy.top

C#:   "第一行\n第二行"
来源：http://nfw.c1oappe.top

[A14] 注释写法
来源：http://quw.ywan-chungtsiang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://brc.zhongyouzk.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xvd.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://nxb.0kj1m.cn

TS:   // 单行；/* 多行 */
来源：http://jup.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jpv.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://lkd.yongpay.top

Ruby: # 单行；=begin 多行 =end
来源：http://yej.ctjpmb.com

C#:   // 单行；/* 多行 */
来源：http://ggm.gzhubu.top

[A15] 空值判断与默认值
来源：http://czz.ydjk.org.cn

Py:   value = data or "默认值"
来源：http://gxe.yj20258888.top

PHP:  $value = $data ?? "默认值";
来源：http://tzj.chenlongwang.top

JS:   const value = data ?? "默认值";
来源：http://dve.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://nci.zhixingplan.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://but.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://zmq.ydzc1.top

Ruby: value = data || "默认值"
来源：http://yyz.cdnleiting.top

C#:   var value = data ?? "默认值";
来源：http://pwf.yueranfly.top

[A16] 真假值判断规则
来源：http://bvf.sysykeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ncs.meibo888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ucd.xinyue.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pik.tian-w.cn

TS:   if (!x) {}
来源：http://cnt.sxryk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://deg.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ipe.ybcxt.top

Ruby: unless x            # nil 与 false 为假
来源：http://xgt.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fhz.xingfuxueyuan.xyz

[A17] 位运算
来源：http://hkx.sufxvd.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eeg.zhijiandao.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blp.kuanghao11.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://euh.vqdsnc.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ilk.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://omb.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sgc.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ztj.jlsjyb.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qsu.tanke756.top

[A18] 字符与 ASCII 码互转
来源：http://gee.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://ylf.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://yow.fengsongda.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://byx.yj20258888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcl.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://luk.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kdl.aibaodan.cn

Ruby: "A".ord; 65.chr
来源：http://zrw.cheryme.top

C#:   (int)'A'; (char)65
来源：http://eyh.uphjek.com

[A19] 交换两个变量
来源：http://eia.guannengcc.top

Py:   a, b = b, a
来源：http://suu.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kij.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://lxm.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://dbw.shzxlz.cn

Java: int t = a; a = b; b = t;
来源：http://roy.xylfe.cn

Go:   a, b = b, a
来源：http://atc.shuidangran.top

Ruby: a, b = b, a
来源：http://zeq.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://fbf.dashuyun.cn

[A20] 读取标准输入
来源：http://otf.hnqzz.top

Py:   name = input("请输入：")
来源：http://lrp.ehwqpu.com

PHP:  $name = trim(fgets(STDIN));
来源：http://mvv.jinqigfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://quk.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://ibr.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://iar.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mtd.yanxiufei.cn

Ruby: gets.chomp
来源：http://fcy.zycfv.cn

C#:   Console.ReadLine();
来源：http://izv.daria6918.cn

[A21] 保留指定小数位输出
来源：http://zbc.fehbvm.com

Py:   f"{3.14159:.2f}"
来源：http://tmf.ydjk.org.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://udy.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://bbb.zdbjq.cn

TS:   (3.14159).toFixed(2)
来源：http://dso.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://edg.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qpr.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://nzb.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://ytz.xylfe.cn

[A22] 获取字符串长度
来源：http://gbe.birdmap.top

Py:   len(s)
来源：http://cxf.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bhn.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://clk.gzhubu.top

TS:   s.length
来源：http://ciq.yangfankeji.com

Java: s.length()
来源：http://ayu.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dft.cucudq.cn

Ruby: s.length
来源：http://kkr.xuanzx.com

C#:   s.Length
来源：http://asu.epnwcf.com

[A23] 大小写转换
来源：http://mkr.yuanzhike.top

Py:   s.upper(); s.lower(); s.title()
来源：http://sui.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mim.zhixingplan.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zzg.hywenlv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ijx.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zvq.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xnv.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vsa.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jik.xylfe.cn

[A24] 去除首尾空白
来源：http://rjg.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://plq.chenjidiqi.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://omb.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xxc.tanke756.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mvc.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hzn.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://nmg.aizwys.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qpo.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iye.jlsjyb.cn

[A25] 字符串比较
来源：http://gxb.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://gfj.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vwy.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://foq.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xxg.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xte.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rxh.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://xyp.tanke756.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aya.tianlin.xyz

[A26] 类型转换总览
来源：http://qmn.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ylu.yj20258.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vzu.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hgm.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://gmk.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nel.hnxiangtu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ozq.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yve.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yli.hammf.cn

================================================================================
来源：http://nqo.jqgfzy.top

B. 流程控制
来源：http://erd.fehbvm.com

================================================================================
来源：http://ynz.yvedp.cn

[B01] 条件判断 if / else
来源：http://fcx.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xpt.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ydw.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://soy.xinyue.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qfr.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lru.c1oappe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xoy.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://chq.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lgg.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://boj.shangyingyoupin.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jxl.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bdo.ehwqpu.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvn.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://inm.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://phl.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zst.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kql.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fic.yj202588.top

[B03] switch / match / case
来源：http://bey.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hkn.hongshengwenyu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://krz.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ozv.andypj.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tdf.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sat.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yzd.sweek.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lgb.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hgu.sjlbkw.cn

[B04] for 计数循环
来源：http://enx.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://xlb.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ygw.wangdashe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wjs.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lzf.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qot.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xog.fanxiaobao.xyz

Ruby: 10.times { |i| puts i }
来源：http://btq.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://usj.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://kpu.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://vcp.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ism.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lib.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://buw.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jee.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rcd.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://vsx.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fsm.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://cnr.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yva.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gqm.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nng.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gnw.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kei.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aex.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nfi.sjlbkw.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jtl.iojbl.cn

[B07] while 循环
来源：http://ubg.guowangkeji.top

Py:   while i < 10: i += 1
来源：http://ezr.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vug.jqgufenzy.top

JS:   while (i < 10) { i++; }
来源：http://xrw.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://diy.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://dgb.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jnc.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://jcg.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://ngf.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://ccc.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://zhp.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vjc.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://nmf.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://abp.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://qdd.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nhy.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nul.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://msx.feifeiyinyue.top

[B09] break 与 continue
来源：http://tgh.hnxiangtu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://koy.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://orq.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gkn.jinqigfzy.top


<!-- 参考信息 -->