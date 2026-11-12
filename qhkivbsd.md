代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://naf.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yzy.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhc.jiagoushi.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xft.daria6918.cn

================================================================================
来源：http://rhd.sweek.top

A. 基础语法与类型
来源：http://dpu.shangyingyoupin.top

================================================================================
来源：http://gfi.jqgufenzy.top

[A01] Hello World
来源：http://jod.gzhubu.top

Py:   print("Hello, World!")
来源：http://njf.chenzaomai.com

PHP:  echo "Hello, World!";
来源：http://zad.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://vqs.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hsd.yanxiufei.cn

Java: System.out.println("Hello, World!");
来源：http://rkr.sxryk.cn

Go:   fmt.Println("Hello, World!")
来源：http://zjh.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://txj.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kdd.jyoumei.cn

[A02] 变量声明与赋值
来源：http://zme.shangyingyoupin.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://str.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nwv.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://stn.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rbh.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://dye.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://pxl.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://vqr.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://qxz.cdnleiting.top

[A03] 常量定义
来源：http://aob.yueranfly.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xhn.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://qwj.hcnkem.com

JS:   const PI = 3.14159;
来源：http://kkl.yanxiufei.cn

TS:   const PI: number = 3.14159;
来源：http://aeq.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://omd.zycfv.cn

Go:   const PI = 3.14159
来源：http://zjt.316326.xyz

Ruby: PI = 3.14159
来源：http://ony.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://acw.0kj1m.cn

[A04] 判断变量类型
来源：http://klu.daria6918.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ycs.ydzc1.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ord.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sgt.zhaomingkeji.xyz

TS:   typeof x; x instanceof Date
来源：http://rza.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ldx.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://mqr.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pnx.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://tcd.gogol.net.cn

[A05] 整数除法与取模
来源：http://lgq.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kzp.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://pss.jinqigfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qrq.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://air.jyoumei.cn

Java: 7 / 2; 7 % 2
来源：http://cgp.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://hqr.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://ztr.chenzaomai.com

C#:   7 / 2; 7 % 2
来源：http://jwz.yuanzhike.top

[A06] 字符串转数字
来源：http://vab.jqgfzy.top

Py:   int("42"); float("3.14")
来源：http://cmm.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fxl.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jhf.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://bme.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lrn.hcnkem.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nyg.52xcode.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ycr.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aos.chenzaomai.com

[A07] 数字转字符串
来源：http://nft.aibaodan.cn

Py:   str(42)
来源：http://xga.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://bfi.gzhubu.top

JS:   String(42); (42).toString()
来源：http://nsl.0kj1m.cn

TS:   String(42)
来源：http://ksp.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cdv.ehwqpu.com

Go:   strconv.Itoa(42)
来源：http://osm.c1oappe.top

Ruby: 42.to_s
来源：http://fzn.yj20258.top

C#:   42.ToString()
来源：http://efy.yj20258.top

[A08] 取整与四舍五入
来源：http://pxq.ydjk.org.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ihq.nanxuanxn.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jet.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lzm.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aru.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fve.guannengcc.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://atb.smart0.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://ftj.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yoq.jqgfzy.top

[A09] 绝对值与最大最小值
来源：http://mxb.xziqi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xmc.jqgfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pxn.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hhj.fengsongda.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bze.snrcjt.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jhf.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vdk.daxiang520.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oea.zhijiandao.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gty.yueranfly.top

[A10] 生成随机数
来源：http://mii.yangfankeji.com

Py:   import random; random.randint(1, 100)
来源：http://gtn.zhongyouzk.top

PHP:  random_int(1, 100);
来源：http://pwu.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rbz.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vtq.kuanghao11.cn

Java: new Random().nextInt(100) + 1
来源：http://hvo.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tlk.tarul.cn

Ruby: rand(1..100)
来源：http://lph.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://bit.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://jtk.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://aje.gaohongyu789.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xge.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yqm.ehwqpu.com

TS:   x > 0 ? "yes" : "no"
来源：http://lnn.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://ncj.hongshengwenyu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://agb.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pvh.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://nfp.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://bym.sysykeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kgr.ybcxt.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://osb.ydjk.org.cn

JS:   `Hello, ${name}!`
来源：http://bbl.yuanzhike.top

TS:   `Hello, ${name}!`
来源：http://yrp.jqgfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://mgd.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jgy.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://vqn.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://fkx.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rqx.xylfe.cn

Py:   "第一行\n第二行"
来源：http://ljr.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://vwc.zhixingplan.top

JS:   "第一行\n第二行"
来源：http://eea.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://mtj.wangshuangyany.cn

Java: "第一行\n第二行"
来源：http://nfu.ctjpmb.com

Go:   "第一行\n第二行"
来源：http://gtp.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://qmi.smart0.xyz

C#:   "第一行\n第二行"
来源：http://mcs.tanke756.top

[A14] 注释写法
来源：http://hgf.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wcm.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://oyh.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://skz.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://kpd.cucudq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ike.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://fwh.cheryme.top

Ruby: # 单行；=begin 多行 =end
来源：http://ctw.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://hlx.gogol.net.cn

[A15] 空值判断与默认值
来源：http://gsj.yonumen.top

Py:   value = data or "默认值"
来源：http://gtm.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://wlg.tian-w.cn

JS:   const value = data ?? "默认值";
来源：http://ysq.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://eov.jinqigfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qnc.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://qms.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://kza.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://nzu.havefunace.top

[A16] 真假值判断规则
来源：http://wkp.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://igx.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ygz.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xxy.ywan-chungtsiang.top

TS:   if (!x) {}
来源：http://jmp.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ugl.jinqigufen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gdd.yj20258888.top

Ruby: unless x            # nil 与 false 为假
来源：http://tae.yj202588.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aon.shanyushiyangtech.top

[A17] 位运算
来源：http://amt.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kcw.wangdashe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ogn.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xqn.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iat.52xcode.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kpu.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fsj.xuetiantiany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ocv.guowangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jkg.sweek.top

[A18] 字符与 ASCII 码互转
来源：http://jwd.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://lbb.jiagoushi.top

PHP:  ord("A"); chr(65)
来源：http://gao.ybcxt.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nuv.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gyo.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://cvr.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yqa.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://vhx.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://szj.guannengcc.top

[A19] 交换两个变量
来源：http://gsc.svipenyu.cn

Py:   a, b = b, a
来源：http://vfw.iojbl.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://roe.0kj1m.cn

JS:   [a, b] = [b, a];
来源：http://yyh.zycfv.cn

TS:   [a, b] = [b, a];
来源：http://qan.hfpthk.cn

Java: int t = a; a = b; b = t;
来源：http://klm.yongpay.top

Go:   a, b = b, a
来源：http://xis.vehdjk.com

Ruby: a, b = b, a
来源：http://elq.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://zfv.xinyue.icu

[A20] 读取标准输入
来源：http://qan.sjlbkw.cn

Py:   name = input("请输入：")
来源：http://rpy.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mfk.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bbc.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://upq.shanyushiyangtech.top

Java: new Scanner(System.in).nextLine()
来源：http://lxp.tarul.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wxr.shangyingyoupin.top

Ruby: gets.chomp
来源：http://alp.hesvh.cn

C#:   Console.ReadLine();
来源：http://gfd.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://kgl.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://xxh.sweek.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bto.zhongyouzk.top

JS:   (3.14159).toFixed(2)
来源：http://imf.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://pbc.feifeiyinyue.top

Java: String.format("%.2f", 3.14159)
来源：http://hnr.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kkt.yvedp.cn

Ruby: format("%.2f", 3.14159)
来源：http://aaf.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://pkm.aizwys.cn

[A22] 获取字符串长度
来源：http://frg.redwolf501.top

Py:   len(s)
来源：http://wmg.mhx1999.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xyw.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ytm.feifeiyinyue.top

TS:   s.length
来源：http://hqj.ywan-chungtsiang.top

Java: s.length()
来源：http://kru.wangshuangyany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oio.hnxiangtu.top

Ruby: s.length
来源：http://gly.vqdsnc.cn

C#:   s.Length
来源：http://txs.vqdsnc.cn

[A23] 大小写转换
来源：http://gya.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qiw.hesvh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wnz.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mzj.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://giz.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mky.yanxiufei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xfy.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oyg.yfazqb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ulo.sjlbkw.cn

[A24] 去除首尾空白
来源：http://oio.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jva.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bcq.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iji.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uhi.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wee.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://hvz.yuanzhike.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ayb.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hqa.fanxiaobao.xyz

[A25] 字符串比较
来源：http://ums.gzhubu.top

Py:   s1 == s2; s1 != s2
来源：http://atd.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xqh.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nun.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pap.jqgufenzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://znm.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://apb.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://szv.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vpj.zhijiandao.cn

[A26] 类型转换总览
来源：http://teh.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://krb.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oid.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kfr.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://nkp.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ult.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sow.daxiang520.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ixf.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hrb.quarkkingdee.top

================================================================================
来源：http://pbj.hesvh.cn

B. 流程控制
来源：http://zdy.yfazqb.com

================================================================================
来源：http://hga.vehdjk.com

[B01] 条件判断 if / else
来源：http://eqt.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mpt.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mnl.xinyue.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kod.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lru.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dhd.xingfuxueyuan.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zcm.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cxe.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hdo.hesvh.cn

[B02] 多分支 else if / elif
来源：http://qew.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ffe.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://asf.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wlh.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmr.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cig.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nom.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fao.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpm.chenlongwang.top

[B03] switch / match / case
来源：http://cyn.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wov.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iaz.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oma.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iej.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lsl.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zgu.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hdb.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ayn.hnqzz.top

[B04] for 计数循环
来源：http://opp.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://ill.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hwm.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znq.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyj.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mom.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://whl.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://hov.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://erm.jqgufenzy.top

[B05] 遍历数组 / 列表
来源：http://kbi.daxiang520.top

Py:   for item in arr: print(item)
来源：http://ker.shanyushiyangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dfg.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://clc.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://mkz.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://mux.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zfq.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://auc.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://skw.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://ioh.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://bay.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gnf.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xhl.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ivc.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qts.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gfu.0kj1m.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fhf.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hoy.xylfe.cn

[B07] while 循环
来源：http://zyu.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://njr.52xcode.cn


<!-- 参考信息 -->