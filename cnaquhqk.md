代发 wailian999

Py:   print("Hello, World!")
来源：http://baj.hnxiangtu.top

PHP:  echo "Hello, World!";
来源：http://gwm.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://vba.cqqwz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://foy.ppjwa.cn

Java: System.out.println("Hello, World!");
来源：http://taj.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://mxg.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://bpg.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://yoi.redwolf501.top

[A02] 变量声明与赋值
来源：http://fps.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hvn.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jeu.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://ekd.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eng.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://lql.yonumen.top

Go:   name := "Alex"; age := 20
来源：http://duv.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://xjr.guannengcc.top

C#:   string name = "Alex"; int age = 20;
来源：http://bbd.hongshengwenyu.top

[A03] 常量定义
来源：http://clx.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bpa.zhongyouzk.top

PHP:  const PI = 3.14159;
来源：http://kpf.52xcode.cn

JS:   const PI = 3.14159;
来源：http://pai.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://dtu.ydzc1.top

Java: static final double PI = 3.14159;
来源：http://ohw.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://vha.hnqzz.top

Ruby: PI = 3.14159
来源：http://bko.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://lge.zycfv.cn

[A04] 判断变量类型
来源：http://tvo.epnwcf.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://qlf.jinqigfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://riv.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tej.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://suq.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wst.mhx1999.top

Go:   reflect.TypeOf(x).Name()
来源：http://ftl.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pxi.gaohongyu789.top

C#:   x.GetType().Name; x is int
来源：http://ytz.svipenyu.cn

[A05] 整数除法与取模
来源：http://dmd.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qtz.bjfxy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xgj.hesvh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rhw.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mfs.smart0.xyz

Java: 7 / 2; 7 % 2
来源：http://spi.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://fnc.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://hhq.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://rnu.nanxinkj.top

[A06] 字符串转数字
来源：http://ebk.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://oop.sweek.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yre.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yzi.yuxming.cn

TS:   parseInt("42", 10); Number("42")
来源：http://aam.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yen.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ige.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://azx.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uly.gotoacloud.top

[A07] 数字转字符串
来源：http://mye.chenzaomai.com

Py:   str(42)
来源：http://xwd.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://nrj.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://eyv.yuxming.cn

TS:   String(42)
来源：http://tbw.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ezr.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://ymw.zdbjq.cn

Ruby: 42.to_s
来源：http://vbz.fzhhl.top

C#:   42.ToString()
来源：http://rrj.tian-w.cn

[A08] 取整与四舍五入
来源：http://xlh.zhengqikj.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ofb.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rog.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nea.cheryme.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nxk.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vnv.jianghu66.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gdx.bbcook.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bez.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lwa.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://irw.nwbrower.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dpw.feifeiyinyue.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bog.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zfb.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ovy.pycfn.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kix.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hjv.meibo888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ael.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xef.yj20258.top

[A10] 生成随机数
来源：http://iql.hywenlv.cn

Py:   import random; random.randint(1, 100)
来源：http://eia.tanke756.top

PHP:  random_int(1, 100);
来源：http://aca.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qfe.andypj.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://adv.iojbl.cn

Java: new Random().nextInt(100) + 1
来源：http://ehy.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://idq.haohaochexian.top

Ruby: rand(1..100)
来源：http://org.c1oappe.top

C#:   new Random().Next(1, 101)
来源：http://dur.pengpengdd.cyou

[A11] 条件表达式（三元）
来源：http://can.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://vrt.jianghu66.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lhh.redwolf501.top

JS:   x > 0 ? "yes" : "no"
来源：http://tkr.shuidangran.top

TS:   x > 0 ? "yes" : "no"
来源：http://txs.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://hsi.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zon.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ysh.tarul.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rsz.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://pro.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dey.redwolf501.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zao.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://nya.ppjwa.cn

TS:   `Hello, ${name}!`
来源：http://wrm.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://pyw.uphjek.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gau.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://ocp.svipenyu.cn

C#:   $"Hello, {name}!"
来源：http://nnx.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://irb.ivvv.top

Py:   "第一行\n第二行"
来源：http://vjo.yj20258.top

PHP:  "第一行\n第二行"
来源：http://ejz.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://aqh.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://pru.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://wiw.0kj1m.cn

Go:   "第一行\n第二行"
来源：http://hkx.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://tio.ywan-chungtsiang.top

C#:   "第一行\n第二行"
来源：http://buh.yangfankeji.com

[A14] 注释写法
来源：http://mwy.jqgufenzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pfm.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cda.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://tli.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://ujf.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://txs.iojbl.cn

Go:   // 单行；/* 多行 */
来源：http://ssk.zhixingplan.top

Ruby: # 单行；=begin 多行 =end
来源：http://nzh.52xcode.cn

C#:   // 单行；/* 多行 */
来源：http://tcn.zhengqikj.top

[A15] 空值判断与默认值
来源：http://txu.ppjwa.cn

Py:   value = data or "默认值"
来源：http://woj.guowangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://znk.ctjpmb.com

JS:   const value = data ?? "默认值";
来源：http://nmm.yanxiufei.cn

TS:   const value = data ?? "默认值";
来源：http://bpn.yangfankeji.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hpl.c1oappe.top

Go:   if data == "" { data = "默认值" }
来源：http://exn.mhx1999.top

Ruby: value = data || "默认值"
来源：http://ztm.dashuyun.cn

C#:   var value = data ?? "默认值";
来源：http://kcp.cheryme.top

[A16] 真假值判断规则
来源：http://fho.daria6918.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oaa.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sgj.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://klv.mhx1999.top

TS:   if (!x) {}
来源：http://cws.hesvh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://puv.yangfankeji.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://poc.epnwcf.com

Ruby: unless x            # nil 与 false 为假
来源：http://pmg.zdbjq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lgz.hywenlv.cn

[A17] 位运算
来源：http://spp.sufxvd.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykv.havefunace.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fmc.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zbd.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ydb.vqdsnc.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zsv.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oyk.tian-w.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzn.ywan-chungtsiang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rks.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://qzc.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://byt.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://xxf.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qzf.aizwys.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zqd.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://swd.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uya.zhengqikj.top

Ruby: "A".ord; 65.chr
来源：http://cfz.tanke756.top

C#:   (int)'A'; (char)65
来源：http://qfm.ctjpmb.com

[A19] 交换两个变量
来源：http://blj.shanyushiyangkeji.top

Py:   a, b = b, a
来源：http://gjz.guowangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://afw.zycfv.cn

JS:   [a, b] = [b, a];
来源：http://jqs.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://ldh.guowangkeji.top

Java: int t = a; a = b; b = t;
来源：http://pwy.bbcook.cn

Go:   a, b = b, a
来源：http://lkp.nanxuanxn.top

Ruby: a, b = b, a
来源：http://lxr.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://yuw.shanyushiyangkeji.top

[A20] 读取标准输入
来源：http://hyl.ctjpmb.com

Py:   name = input("请输入：")
来源：http://zha.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lce.meibo888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://awh.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://bfh.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://zke.gogol.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xtd.tanke756.top

Ruby: gets.chomp
来源：http://jxf.guowangkeji.top

C#:   Console.ReadLine();
来源：http://nnv.yonumen.top

[A21] 保留指定小数位输出
来源：http://jxm.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://apv.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xmj.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://rcx.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://iwp.zhaomingkeji.xyz

Java: String.format("%.2f", 3.14159)
来源：http://zky.xuanzx.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xdo.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://zjw.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://fqc.nwbrower.top

[A22] 获取字符串长度
来源：http://civ.chenjidiqi.icu

Py:   len(s)
来源：http://akh.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yya.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nfo.sufxvd.cn

TS:   s.length
来源：http://dxz.zdqjudy.top

Java: s.length()
来源：http://plc.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lkz.havefunace.top

Ruby: s.length
来源：http://hka.xinyue.icu

C#:   s.Length
来源：http://mfq.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://zjw.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wgx.vqdsnc.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://omp.hnqzz.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aaq.cqqwz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ccs.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tuu.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rrk.chenjidiqi.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qwz.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mpp.yuanzhike.top

[A24] 去除首尾空白
来源：http://kmx.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rvg.xinyue.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xis.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qwa.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vic.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://amf.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://rss.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hbb.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jsu.wangshuangyany.cn

[A25] 字符串比较
来源：http://oys.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://gyd.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bex.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lib.jiagoushi.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://amv.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ocg.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lgl.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tpy.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dwx.pengpengdd.cyou

[A26] 类型转换总览
来源：http://jty.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ver.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fmg.aibaodan.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wlu.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://bfu.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oet.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rrz.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xyd.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hlv.zhijiandao.cn

================================================================================
来源：http://fxo.hywenlv.cn

B. 流程控制
来源：http://gvr.zhoulong.xyz

================================================================================
来源：http://gas.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://lbw.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://odj.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cqc.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://afq.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kln.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://puk.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kyj.feifeiyinyue.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mcj.hammf.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tgp.fehbvm.com

[B02] 多分支 else if / elif
来源：http://qqb.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tzj.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://urd.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yto.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhr.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyi.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uik.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zpv.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fqy.mhx1999.top

[B03] switch / match / case
来源：http://ywk.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gcz.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://izc.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rzx.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yfq.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nnu.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://upz.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ypc.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fue.jyoumei.cn

[B04] for 计数循环
来源：http://xtx.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://iug.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kra.birdmap.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zhj.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://coa.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hvi.0kj1m.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qzo.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://nft.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nov.yj20258.top

[B05] 遍历数组 / 列表
来源：http://xno.bjfxy.top

Py:   for item in arr: print(item)
来源：http://wbl.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ldb.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://hfv.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lzi.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gwh.gzhubu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ndr.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://xms.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qhp.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://fns.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://imr.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vqc.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hwx.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jql.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ktx.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://akp.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vpc.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ygm.mhx1999.top

[B07] while 循环
来源：http://rvg.yfazqb.com

Py:   while i < 10: i += 1
来源：http://kwe.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://jjc.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://tpn.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://weo.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://wzw.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ijc.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://ejp.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://iht.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://nqp.c1oappe.top


<!-- 参考信息 -->