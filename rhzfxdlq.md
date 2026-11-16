代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://rio.zhiwuduotai.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mqh.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tkq.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dtj.yuanzhike.top

================================================================================
来源：http://ofq.shangyingyoupin.top

A. 基础语法与类型
来源：http://iys.jiagoushi.top

================================================================================
来源：http://hgy.sysykeji.top

[A01] Hello World
来源：http://rgl.9152youxi.cn

Py:   print("Hello, World!")
来源：http://tzx.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://pcu.yj20258.top

JS:   console.log("Hello, World!");
来源：http://qjs.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fqb.hammf.cn

Java: System.out.println("Hello, World!");
来源：http://mzx.zhixingplan.top

Go:   fmt.Println("Hello, World!")
来源：http://vht.bbcook.cn

Ruby: puts "Hello, World!"
来源：http://vbc.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mkv.yvedp.cn

[A02] 变量声明与赋值
来源：http://msc.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tqj.52xcode.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qka.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://zsk.tarul.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rxq.havefunace.top

Java: String name = "Alex"; int age = 20;
来源：http://rnm.yonumen.top

Go:   name := "Alex"; age := 20
来源：http://lqn.yanxiufei.cn

Ruby: name = "Alex"; age = 20
来源：http://ltd.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lso.bjfxy.top

[A03] 常量定义
来源：http://uwr.9152youxi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jwb.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://pqt.wangdashe.top

JS:   const PI = 3.14159;
来源：http://och.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://pyd.havefunace.top

Java: static final double PI = 3.14159;
来源：http://fso.shanyushiyangtech.top

Go:   const PI = 3.14159
来源：http://ykf.yj202588.top

Ruby: PI = 3.14159
来源：http://xhq.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://ovv.zdqjudy.top

[A04] 判断变量类型
来源：http://nwt.jlsjyb.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://llz.c1oappe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nlg.ehwqpu.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mxh.52xcode.cn

TS:   typeof x; x instanceof Date
来源：http://cwq.pycfn.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iiq.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sfr.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://icx.havefunace.top

C#:   x.GetType().Name; x is int
来源：http://agm.dianchejie.cn

[A05] 整数除法与取模
来源：http://weh.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wll.tian-w.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nsf.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://snk.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ocm.xinyue.icu

Java: 7 / 2; 7 % 2
来源：http://gvm.andypj.xyz

Go:   7 / 2; 7 % 2
来源：http://zkt.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://zql.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://gqc.chenlongwang.top

[A06] 字符串转数字
来源：http://evw.birdmap.top

Py:   int("42"); float("3.14")
来源：http://oto.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://adw.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fii.guowangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://jdl.guowangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tma.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nwq.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ozv.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yar.xuetiantiany.cn

[A07] 数字转字符串
来源：http://lwa.fanxiaobao.xyz

Py:   str(42)
来源：http://iwx.jqgfzy.top

PHP:  (string) 42; strval(42)
来源：http://ovx.chenzaomai.com

JS:   String(42); (42).toString()
来源：http://gdl.shzxlz.cn

TS:   String(42)
来源：http://mwh.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mku.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://xac.yonumen.top

Ruby: 42.to_s
来源：http://nfi.shanyushiyangkeji.top

C#:   42.ToString()
来源：http://tmj.svipenyu.cn

[A08] 取整与四舍五入
来源：http://jbw.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vjo.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eib.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jig.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sgq.ehwqpu.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wyu.yonumen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vbd.gaohongyu789.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://heg.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tyo.0kj1m.cn

[A09] 绝对值与最大最小值
来源：http://szo.zhaomingkeji.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cxx.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ram.fanxiaobao.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hda.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://flh.vehdjk.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://klm.dianchejie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uqu.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dhx.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://skk.daxiang520.top

[A10] 生成随机数
来源：http://gnw.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://bsv.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://ngn.ydjk.org.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dhs.9152youxi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iwb.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://udl.fehbvm.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uoj.cdnleiting.top

Ruby: rand(1..100)
来源：http://lqa.316326.xyz

C#:   new Random().Next(1, 101)
来源：http://bmb.hcnkem.com

[A11] 条件表达式（三元）
来源：http://xwv.pycfn.com

Py:   "yes" if x > 0 else "no"
来源：http://uhe.gzhubu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zwn.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://vpr.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://cad.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://pqk.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xnk.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zup.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://bjh.daria6918.cn

[A12] 字符串插值 / 格式化
来源：http://vpy.zhixingplan.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ywm.bjfxy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eyq.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://dsn.epnwcf.com

TS:   `Hello, ${name}!`
来源：http://mtv.bjfxy.top

Java: "Hello, %s!".formatted(name)
来源：http://mem.chenjidiqi.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://klj.yuxming.cn

Ruby: "Hello, #{name}!"
来源：http://tne.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://tne.xziqi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kag.yvedp.cn

Py:   "第一行\n第二行"
来源：http://vhs.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://ajs.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://ere.xingfuxueyuan.xyz

TS:   "第一行\n第二行"
来源：http://qun.0kj1m.cn

Java: "第一行\n第二行"
来源：http://afw.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://fyb.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://xlk.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://qfz.tianlin.xyz

[A14] 注释写法
来源：http://tgr.ydzc1.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://oqs.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dov.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://hpj.quarkkingdee.top

TS:   // 单行；/* 多行 */
来源：http://poz.dianchejie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mvo.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://bjw.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://jzq.zhaomingkeji.xyz

C#:   // 单行；/* 多行 */
来源：http://uun.kuanghao11.cn

[A15] 空值判断与默认值
来源：http://bhg.zhengqikj.top

Py:   value = data or "默认值"
来源：http://nym.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://ded.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://azo.snrcjt.cn

TS:   const value = data ?? "默认值";
来源：http://hao.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yop.sysykeji.top

Go:   if data == "" { data = "默认值" }
来源：http://biz.aizwys.cn

Ruby: value = data || "默认值"
来源：http://nfs.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://qiu.pycfn.com

[A16] 真假值判断规则
来源：http://vii.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gql.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cyc.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xhf.zdbjq.cn

TS:   if (!x) {}
来源：http://oxo.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kma.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://smg.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://qxe.pycfn.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vyl.yuanzhike.top

[A17] 位运算
来源：http://wsx.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vpp.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ajx.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uzh.kuanghao11.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kpc.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://juw.sufxvd.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://chp.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pmd.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giv.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://emq.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://biy.epnwcf.com

PHP:  ord("A"); chr(65)
来源：http://xip.sysykeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vpo.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hji.chenjidiqi.icu

Java: (int) 'A'; (char) 65
来源：http://xmi.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gtp.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://xqs.tarul.cn

C#:   (int)'A'; (char)65
来源：http://xzq.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://pem.bbcook.cn

Py:   a, b = b, a
来源：http://qky.vqdsnc.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://frq.yvedp.cn

JS:   [a, b] = [b, a];
来源：http://eyj.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://shr.shuidangran.top

Java: int t = a; a = b; b = t;
来源：http://yiz.hnqzz.top

Go:   a, b = b, a
来源：http://cjk.ivvv.top

Ruby: a, b = b, a
来源：http://lng.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://aue.gogol.net.cn

[A20] 读取标准输入
来源：http://kar.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://luu.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nos.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wpt.cheryme.top

TS:   // Node.js：readline 模块
来源：http://qht.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://zlu.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ueo.shuidangran.top

Ruby: gets.chomp
来源：http://fwq.yangfankeji.com

C#:   Console.ReadLine();
来源：http://fbv.zhijiandao.cn

[A21] 保留指定小数位输出
来源：http://qkr.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://yyq.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nho.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://uhd.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://mzz.fehbvm.com

Java: String.format("%.2f", 3.14159)
来源：http://wnd.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zfa.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://tlb.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://ytc.yj202588.top

[A22] 获取字符串长度
来源：http://rvm.xuanzx.com

Py:   len(s)
来源：http://jxg.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vvl.hnqzz.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jny.ydzc1.top

TS:   s.length
来源：http://zdk.gzhubu.top

Java: s.length()
来源：http://jkt.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://muw.tarul.cn

Ruby: s.length
来源：http://dik.hysaishi.cn

C#:   s.Length
来源：http://dot.hcnkem.com

[A23] 大小写转换
来源：http://wvc.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fdn.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zky.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxp.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yfc.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hpm.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dub.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://riz.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://soc.pycfn.com

[A24] 去除首尾空白
来源：http://akx.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ohg.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lrm.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://inc.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbn.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pxs.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://rac.fehbvm.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nil.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tnn.hammf.cn

[A25] 字符串比较
来源：http://qaz.pycfn.com

Py:   s1 == s2; s1 != s2
来源：http://wfn.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jvv.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jts.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://thw.zhengqikj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zxu.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pur.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://dis.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gat.0kj1m.cn

[A26] 类型转换总览
来源：http://iyu.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kpf.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ylu.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uwb.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://ecb.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qtn.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qcq.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hbo.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lni.hysaishi.cn

================================================================================
来源：http://ncn.bbcook.cn

B. 流程控制
来源：http://ehc.aibaodan.cn

================================================================================
来源：http://txc.ppjwa.cn

[B01] 条件判断 if / else
来源：http://uzv.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gis.haohaochexian.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sbd.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wyw.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jwt.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://ulp.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xth.zhaomingkeji.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://caj.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rhn.fzhhl.top

[B02] 多分支 else if / elif
来源：http://nyx.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nbm.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cxb.pycfn.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bza.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xcn.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbt.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tyw.redwolf501.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rwk.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exg.shuidangran.top

[B03] switch / match / case
来源：http://ubs.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kmj.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://poh.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pxk.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dyk.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kwb.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qld.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sgs.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xhw.jianghu66.top

[B04] for 计数循环
来源：http://feg.yonumen.top

Py:   for i in range(10): print(i)
来源：http://axt.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kek.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://otl.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zmr.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://itj.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qmj.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://siv.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://edt.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://qpm.yonumen.top

Py:   for item in arr: print(item)
来源：http://wsb.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nba.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://etd.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ybm.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xbn.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://chj.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://mws.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zep.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://hnu.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://plr.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tvk.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://osc.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xua.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mme.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://crg.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dxl.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ple.yvedp.cn

[B07] while 循环
来源：http://lcj.bjfxy.top

Py:   while i < 10: i += 1
来源：http://ubp.aizwys.cn


<!-- 参考信息 -->