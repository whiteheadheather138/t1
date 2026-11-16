代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://jhb.zhengqikj.top

[A03] 常量定义
来源：http://ygl.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tfg.aibaodan.cn

PHP:  const PI = 3.14159;
来源：http://bsh.ybcxt.top

JS:   const PI = 3.14159;
来源：http://con.sufxvd.cn

TS:   const PI: number = 3.14159;
来源：http://bfp.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://dmx.chenlongwang.top

Go:   const PI = 3.14159
来源：http://sym.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://frb.jinqigfzy.top

C#:   const double PI = 3.14159;
来源：http://zad.pengpengdd.cyou

[A04] 判断变量类型
来源：http://asp.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pmu.gotoacloud.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nvm.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kei.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://lru.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hnd.sufxvd.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cxx.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jmj.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://daf.uphjek.com

[A05] 整数除法与取模
来源：http://ujb.sweek.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mnt.xuanzx.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ocd.yuanzhike.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://egm.ivvv.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eed.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://jfh.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://cyf.gzhubu.top

Ruby: 7 / 2; 7 % 2
来源：http://yfl.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://wpw.hammf.cn

[A06] 字符串转数字
来源：http://rwv.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://bpe.gotoacloud.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rdx.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bbs.yj20258.top

TS:   parseInt("42", 10); Number("42")
来源：http://zom.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://asu.sysykeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tts.tian-w.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jlr.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nwt.wangdashe.top

[A07] 数字转字符串
来源：http://nfq.zhixingplan.top

Py:   str(42)
来源：http://cql.yfazqb.com

PHP:  (string) 42; strval(42)
来源：http://jgs.gaohongyu789.top

JS:   String(42); (42).toString()
来源：http://amk.cdnleiting.top

TS:   String(42)
来源：http://vln.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rnl.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://yps.tian-w.cn

Ruby: 42.to_s
来源：http://kxj.nanxuanxn.top

C#:   42.ToString()
来源：http://urt.andypj.xyz

[A08] 取整与四舍五入
来源：http://ygk.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kqm.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hos.hywenlv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://atq.gaohongyu789.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wkk.svipenyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mky.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jiz.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://mzw.nwbrower.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cep.wangshuangyany.cn

[A09] 绝对值与最大最小值
来源：http://xmx.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ymf.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vvv.zhoulong.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ihw.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cuk.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pws.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ayy.cqqwz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rxe.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wjn.birdmap.top

[A10] 生成随机数
来源：http://mrv.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://ndu.havefunace.top

PHP:  random_int(1, 100);
来源：http://des.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gru.tarul.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cba.bbcook.cn

Java: new Random().nextInt(100) + 1
来源：http://qwq.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zid.uphjek.com

Ruby: rand(1..100)
来源：http://plw.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://zxm.andypj.xyz

[A11] 条件表达式（三元）
来源：http://ggg.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://gbu.epnwcf.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://fyt.guannengcc.top

JS:   x > 0 ? "yes" : "no"
来源：http://rdp.mhx1999.top

TS:   x > 0 ? "yes" : "no"
来源：http://dnb.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://sqx.zycfv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nad.xylfe.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qoi.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://azx.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://ort.haohaochexian.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sba.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://veo.cucudq.cn

JS:   `Hello, ${name}!`
来源：http://krr.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://jcs.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://xrx.zhoulong.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://krb.jianghu66.top

Ruby: "Hello, #{name}!"
来源：http://ijo.daria6918.cn

C#:   $"Hello, {name}!"
来源：http://raw.sjlbkw.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fnn.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://ihn.iojbl.cn

PHP:  "第一行\n第二行"
来源：http://fhn.yj20258.top

JS:   "第一行\n第二行"
来源：http://uwj.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://ihi.tarul.cn

Java: "第一行\n第二行"
来源：http://ftd.pycfn.com

Go:   "第一行\n第二行"
来源：http://bue.yfazqb.com

Ruby: "第一行\n第二行"
来源：http://crc.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://irn.ppjwa.cn

[A14] 注释写法
来源：http://edx.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://koz.jqgufenzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tcj.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://vqd.shanyushiyangtech.top

TS:   // 单行；/* 多行 */
来源：http://klf.ywan-chungtsiang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jym.cqqwz.cn

Go:   // 单行；/* 多行 */
来源：http://czy.sufxvd.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bcy.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://loo.sweek.top

[A15] 空值判断与默认值
来源：http://dwq.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://vyi.jinqigfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://nfo.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://qor.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://gvn.xziqi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://seh.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://sin.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://rgp.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://gaz.birdmap.top

[A16] 真假值判断规则
来源：http://jul.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jre.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dff.zhiwuduotai.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wqo.xingfuxueyuan.xyz

TS:   if (!x) {}
来源：http://nfv.xuetiantiany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jzj.shuidangran.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ltj.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://hei.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://buf.andypj.xyz

[A17] 位运算
来源：http://ndm.jiagoushi.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cmc.havefunace.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rog.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jqz.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ztr.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qbc.zhijiandao.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lky.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rqz.feifeiyinyue.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://flc.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://evu.jinghuilouyu.cn

Py:   ord("A"); chr(65)
来源：http://cor.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://lbe.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pga.sysykeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mke.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://abd.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nwc.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://rof.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://fdo.yfazqb.com

[A19] 交换两个变量
来源：http://uqh.ywan-chungtsiang.top

Py:   a, b = b, a
来源：http://gci.shanyushiyangtech.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ezo.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://klq.yanxiufei.cn

TS:   [a, b] = [b, a];
来源：http://cbz.jinghuilouyu.cn

Java: int t = a; a = b; b = t;
来源：http://vcv.hywenlv.cn

Go:   a, b = b, a
来源：http://xqd.jinqigufen.top

Ruby: a, b = b, a
来源：http://zbk.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://xwb.yfazqb.com

[A20] 读取标准输入
来源：http://tmt.mhx1999.top

Py:   name = input("请输入：")
来源：http://keg.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hdf.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://chx.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://iqv.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://hpd.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qgu.uphjek.com

Ruby: gets.chomp
来源：http://vit.316326.xyz

C#:   Console.ReadLine();
来源：http://nry.hesvh.cn

[A21] 保留指定小数位输出
来源：http://urz.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://cir.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yri.epnwcf.com

JS:   (3.14159).toFixed(2)
来源：http://aab.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://dkw.bjfxy.top

Java: String.format("%.2f", 3.14159)
来源：http://asj.redwolf501.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vcs.ywan-chungtsiang.top

Ruby: format("%.2f", 3.14159)
来源：http://pva.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://wht.guannengcc.top

[A22] 获取字符串长度
来源：http://hlz.fzhhl.top

Py:   len(s)
来源：http://jfy.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nig.shuidangran.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vpr.chenlongwang.top

TS:   s.length
来源：http://hlm.kuanghao11.cn

Java: s.length()
来源：http://yxi.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cym.nanxinkj.top

Ruby: s.length
来源：http://tvt.dianchejie.cn

C#:   s.Length
来源：http://sco.ybcxt.top

[A23] 大小写转换
来源：http://swn.shanyushiyangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mqd.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://csu.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kke.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hxf.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hfc.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cuj.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://exz.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lwu.zhaomingkeji.xyz

[A24] 去除首尾空白
来源：http://jqz.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jeb.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://osc.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lrc.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bxw.hywenlv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ubd.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://wgc.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xmm.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blc.hammf.cn

[A25] 字符串比较
来源：http://zst.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://ncb.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rel.hywenlv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fyv.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ctw.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hhl.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ouq.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dxm.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oxr.meibo888.top

[A26] 类型转换总览
来源：http://moc.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nut.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ffs.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cpm.shzxlz.cn

TS:   Number() String() Boolean() x as number
来源：http://ure.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lny.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xje.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tig.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fur.havefunace.top

================================================================================
来源：http://xif.zhaomingkeji.xyz

B. 流程控制
来源：http://eby.zhaomingkeji.xyz

================================================================================
来源：http://srg.redwolf501.top

[B01] 条件判断 if / else
来源：http://vgn.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tzy.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://glv.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sfi.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kzu.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bim.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qck.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://etp.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ltg.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://bjw.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zuj.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rem.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhy.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqz.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bag.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oqu.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dia.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slg.vqdsnc.cn

[B03] switch / match / case
来源：http://gsi.dianchejie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ikr.redwolf501.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://opz.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yym.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rnp.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oib.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uwd.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ewt.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://roo.andypj.xyz

[B04] for 计数循环
来源：http://ujp.feifeiyinyue.top

Py:   for i in range(10): print(i)
来源：http://ndw.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vpz.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://isl.vehdjk.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zid.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ytw.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ved.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://ics.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blt.yonumen.top

[B05] 遍历数组 / 列表
来源：http://xxe.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://rqd.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pml.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bvf.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pvq.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gul.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pyz.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://hja.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hbj.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://jds.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sjv.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qjb.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fro.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ntd.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sxy.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pbs.iojbl.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tbu.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mcp.zycfv.cn

[B07] while 循环
来源：http://orw.daxiang520.top

Py:   while i < 10: i += 1
来源：http://qbb.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://eho.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://uwh.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://scf.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://xpe.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://imb.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://iqx.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://khr.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://uwn.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://zwa.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://aix.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://tyr.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://mrs.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://rcy.shanyushiyangtech.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wif.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://hnl.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://yze.hysaishi.cn

[B09] break 与 continue
来源：http://upj.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nbr.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sqr.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://irr.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://goe.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnm.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://plx.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zfd.tian-w.cn


<!-- 参考信息 -->