代发 wailian999

[A02] 变量声明与赋值
来源：http://vak.hcnkem.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mfn.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://khu.xinyue.icu

JS:   let name = "Alex"; const age = 20;
来源：http://ikh.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gss.52xcode.cn

Java: String name = "Alex"; int age = 20;
来源：http://fde.pycfn.com

Go:   name := "Alex"; age := 20
来源：http://wvc.316326.xyz

Ruby: name = "Alex"; age = 20
来源：http://fba.guowangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://ukb.ehwqpu.com

[A03] 常量定义
来源：http://ony.nanxinkj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jjo.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://rfn.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://ctv.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://ghm.sufxvd.cn

Java: static final double PI = 3.14159;
来源：http://fqn.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://fis.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://ssf.ybcxt.top

C#:   const double PI = 3.14159;
来源：http://whn.guannengcc.top

[A04] 判断变量类型
来源：http://bfl.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://tjj.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mhq.jianghu66.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iek.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://qqu.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gff.xziqi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lrt.chenjidiqi.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://dzu.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://ivj.hfpthk.cn

[A05] 整数除法与取模
来源：http://lop.tianlin.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hli.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://max.jinqigufen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://czp.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://seq.bjfxy.top

Java: 7 / 2; 7 % 2
来源：http://jah.tianlin.xyz

Go:   7 / 2; 7 % 2
来源：http://nyc.ydzc1.top

Ruby: 7 / 2; 7 % 2
来源：http://jrh.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://ujw.yuanzhike.top

[A06] 字符串转数字
来源：http://mab.hywenlv.cn

Py:   int("42"); float("3.14")
来源：http://hgt.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kce.tian-w.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zgr.birdmap.top

TS:   parseInt("42", 10); Number("42")
来源：http://rea.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hcv.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rrk.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jif.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qbh.yfazqb.com

[A07] 数字转字符串
来源：http://sxv.mhx1999.top

Py:   str(42)
来源：http://rpa.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://kab.mhx1999.top

JS:   String(42); (42).toString()
来源：http://qyj.smart0.xyz

TS:   String(42)
来源：http://ust.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mpu.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://vam.yuanzhike.top

Ruby: 42.to_s
来源：http://gcm.hysaishi.cn

C#:   42.ToString()
来源：http://hjk.zdqjudy.top

[A08] 取整与四舍五入
来源：http://czu.aizwys.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://drl.zhijiandao.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nhp.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tjg.tianlin.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hfm.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jac.xuanzx.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xxs.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vnv.ehwqpu.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iij.birdmap.top

[A09] 绝对值与最大最小值
来源：http://tru.shuidangran.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jhi.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cya.andypj.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://aqf.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://brz.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dnf.fanxiaobao.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xpq.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tds.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://air.chenjidiqi.icu

[A10] 生成随机数
来源：http://yoj.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://toe.svipenyu.cn

PHP:  random_int(1, 100);
来源：http://beg.ybcxt.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xek.zycfv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://utl.daxiang520.top

Java: new Random().nextInt(100) + 1
来源：http://cfo.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jnp.shzxlz.cn

Ruby: rand(1..100)
来源：http://ssm.yj202588.top

C#:   new Random().Next(1, 101)
来源：http://gbp.jyoumei.cn

[A11] 条件表达式（三元）
来源：http://onf.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://gxe.ywan-chungtsiang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bvg.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://euj.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zyu.yonumen.top

Java: x > 0 ? "yes" : "no"
来源：http://zle.yj20258.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dee.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dpb.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://qgi.ywan-chungtsiang.top

[A12] 字符串插值 / 格式化
来源：http://sct.jianghu66.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kvd.0kj1m.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sxi.quarkkingdee.top

JS:   `Hello, ${name}!`
来源：http://wvr.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://btj.snrcjt.cn

Java: "Hello, %s!".formatted(name)
来源：http://rse.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xrd.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://pcu.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://zsh.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mqg.yj202588.top

Py:   "第一行\n第二行"
来源：http://bbz.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://sax.hysaishi.cn

JS:   "第一行\n第二行"
来源：http://upg.zhoulong.xyz

TS:   "第一行\n第二行"
来源：http://mjw.ctjpmb.com

Java: "第一行\n第二行"
来源：http://hmq.uphjek.com

Go:   "第一行\n第二行"
来源：http://yhc.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://yav.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://nzn.havefunace.top

[A14] 注释写法
来源：http://inf.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rxq.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sue.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://zaz.zhaomingkeji.xyz

TS:   // 单行；/* 多行 */
来源：http://hcz.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vfa.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://epy.birdmap.top

Ruby: # 单行；=begin 多行 =end
来源：http://txt.wangshuangyany.cn

C#:   // 单行；/* 多行 */
来源：http://sqj.cqqwz.cn

[A15] 空值判断与默认值
来源：http://wdl.ppjwa.cn

Py:   value = data or "默认值"
来源：http://opr.tian-w.cn

PHP:  $value = $data ?? "默认值";
来源：http://jde.aizwys.cn

JS:   const value = data ?? "默认值";
来源：http://lwd.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://pmu.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cbh.jiagoushi.top

Go:   if data == "" { data = "默认值" }
来源：http://lgw.yj20258888.top

Ruby: value = data || "默认值"
来源：http://wxy.hfpthk.cn

C#:   var value = data ?? "默认值";
来源：http://xbm.snrcjt.cn

[A16] 真假值判断规则
来源：http://wto.svipenyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dgv.hcnkem.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://amj.jlsjyb.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nlh.zhoulong.xyz

TS:   if (!x) {}
来源：http://vvy.hnqzz.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sno.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vwt.gotoacloud.top

Ruby: unless x            # nil 与 false 为假
来源：http://wyy.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ghq.yj20258.top

[A17] 位运算
来源：http://shy.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://asn.zhixingplan.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zao.yj20258888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hev.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ozc.vqdsnc.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zim.aizwys.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blf.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmy.ivvv.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fyc.tarul.cn

[A18] 字符与 ASCII 码互转
来源：http://xxi.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://mna.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://vyh.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcc.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bbp.hywenlv.cn

Java: (int) 'A'; (char) 65
来源：http://qez.cucudq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://imn.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://ssx.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://lao.jianghu66.top

[A19] 交换两个变量
来源：http://qgb.jinqigfzy.top

Py:   a, b = b, a
来源：http://yit.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://crl.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://gib.daxiang520.top

TS:   [a, b] = [b, a];
来源：http://qzx.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://wub.daria6918.cn

Go:   a, b = b, a
来源：http://xqj.tanke756.top

Ruby: a, b = b, a
来源：http://agn.fktsv.cn

C#:   (a, b) = (b, a);
来源：http://ivc.sweek.top

[A20] 读取标准输入
来源：http://myc.pycfn.com

Py:   name = input("请输入：")
来源：http://med.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cbq.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pff.jyoumei.cn

TS:   // Node.js：readline 模块
来源：http://jtn.hysaishi.cn

Java: new Scanner(System.in).nextLine()
来源：http://skx.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xxm.birdmap.top

Ruby: gets.chomp
来源：http://ttd.yj202588.top

C#:   Console.ReadLine();
来源：http://ovr.shuidangran.top

[A21] 保留指定小数位输出
来源：http://onu.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://glp.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pyw.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://kxc.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://dsn.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://fsi.daria6918.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eba.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://poh.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://jdv.yongpay.top

[A22] 获取字符串长度
来源：http://zhr.ehwqpu.com

Py:   len(s)
来源：http://ofo.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ake.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jnk.zdqjudy.top

TS:   s.length
来源：http://kjh.uphjek.com

Java: s.length()
来源：http://ouq.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://atz.birdmap.top

Ruby: s.length
来源：http://lnf.yfazqb.com

C#:   s.Length
来源：http://csb.bjfxy.top

[A23] 大小写转换
来源：http://xll.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jkd.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qlb.zhixingplan.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ehb.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ono.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://amo.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ihx.jiagoushi.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mju.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qfw.andypj.xyz

[A24] 去除首尾空白
来源：http://qcd.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bht.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fwv.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gzf.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ysy.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oqk.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://alc.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cey.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hpp.hongshengwenyu.top

[A25] 字符串比较
来源：http://wfe.pycfn.com

Py:   s1 == s2; s1 != s2
来源：http://uix.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ths.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lxn.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xln.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tmr.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gnv.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ajt.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pdj.c1oappe.top

[A26] 类型转换总览
来源：http://bhs.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nkl.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rsl.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://izv.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://nco.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ohu.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sue.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vrb.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jqq.hnxiangtu.top

================================================================================
来源：http://lvz.xuetiantiany.cn

B. 流程控制
来源：http://hxx.yanxiufei.cn

================================================================================
来源：http://yvd.daxiang520.top

[B01] 条件判断 if / else
来源：http://jbr.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xha.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jyu.ywan-chungtsiang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jth.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rol.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ibh.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bub.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bvc.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ubw.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://wko.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://euv.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mpi.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilg.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cjs.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzc.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eaj.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vjg.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wui.fktsv.cn

[B03] switch / match / case
来源：http://rix.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zgg.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eyn.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fqn.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nyy.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vrd.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oim.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wkl.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nbw.guowangkeji.top

[B04] for 计数循环
来源：http://lny.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://zek.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xlj.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fvu.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pfu.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bmd.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lip.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://ktw.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jbp.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://rdx.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://ezk.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bio.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hhp.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://cte.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ijh.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fcx.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://xmp.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ulo.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://ihe.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://svv.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ygf.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ktf.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gyv.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eis.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oun.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qao.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cup.0kj1m.cn

[B07] while 循环
来源：http://zux.c1oappe.top

Py:   while i < 10: i += 1
来源：http://ftw.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://uuo.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://mfm.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://dee.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://nvn.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://efx.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://xpm.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://jca.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://fad.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://xbj.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wrp.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://uws.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://gqy.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://imr.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tjf.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ckd.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://mnu.9152youxi.cn


<!-- 参考信息 -->