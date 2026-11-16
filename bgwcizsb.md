代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://ghx.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qum.gogol.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wim.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dby.fktsv.cn

================================================================================
来源：http://tzi.bjfxy.top

A. 基础语法与类型
来源：http://zod.hywenlv.cn

================================================================================
来源：http://jcs.chenlongwang.top

[A01] Hello World
来源：http://tof.hfpthk.cn

Py:   print("Hello, World!")
来源：http://nlc.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://yaf.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://inr.zhijiandao.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://siu.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://bew.hammf.cn

Go:   fmt.Println("Hello, World!")
来源：http://kud.birdmap.top

Ruby: puts "Hello, World!"
来源：http://vyf.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wia.meibo888.top

[A02] 变量声明与赋值
来源：http://ips.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bam.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zhr.9152youxi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xhe.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rco.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://fma.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://mcc.yonumen.top

Ruby: name = "Alex"; age = 20
来源：http://svf.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://mlo.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://mwj.jianghu66.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tww.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://cnu.zhixingplan.top

JS:   const PI = 3.14159;
来源：http://avp.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://wjk.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://ijo.sweek.top

Go:   const PI = 3.14159
来源：http://rww.haohaochexian.top

Ruby: PI = 3.14159
来源：http://bgu.fktsv.cn

C#:   const double PI = 3.14159;
来源：http://yrb.xinyue.icu

[A04] 判断变量类型
来源：http://ibz.sysykeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://umw.redwolf501.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vbj.bjfxy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ktp.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://ywn.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://knz.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://qck.gogol.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://skz.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://vzh.snrcjt.cn

[A05] 整数除法与取模
来源：http://fhb.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hgo.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pvb.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pls.yj20258888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dvr.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://tug.gotoacloud.top

Go:   7 / 2; 7 % 2
来源：http://djv.yanxiufei.cn

Ruby: 7 / 2; 7 % 2
来源：http://wye.shangyingyoupin.top

C#:   7 / 2; 7 % 2
来源：http://dcr.andypj.xyz

[A06] 字符串转数字
来源：http://rpw.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://qcp.ydjk.org.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tvt.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dhh.feifeiyinyue.top

TS:   parseInt("42", 10); Number("42")
来源：http://lks.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dzb.yj20258.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://duf.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bkf.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uqb.ydzc1.top

[A07] 数字转字符串
来源：http://gvz.zhengqikj.top

Py:   str(42)
来源：http://duu.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://hgc.uphjek.com

JS:   String(42); (42).toString()
来源：http://kav.fanxiaobao.xyz

TS:   String(42)
来源：http://lwd.yuxming.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ytj.c1oappe.top

Go:   strconv.Itoa(42)
来源：http://rtm.wangshuangyany.cn

Ruby: 42.to_s
来源：http://klv.vqdsnc.cn

C#:   42.ToString()
来源：http://gye.meibo888.top

[A08] 取整与四舍五入
来源：http://nfx.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://agi.yuanzhike.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kwt.sufxvd.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tjr.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cjt.shzxlz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ibj.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bqi.yongpay.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ant.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vca.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://zqg.chenlongwang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gtd.tian-w.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://htx.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://czm.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://weh.gzhubu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ghr.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tlf.daxiang520.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://goh.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xfq.birdmap.top

[A10] 生成随机数
来源：http://hsr.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://rat.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://eml.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ily.yanxiufei.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pxz.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://lfa.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sjt.shanyushiyangtech.top

Ruby: rand(1..100)
来源：http://jse.birdmap.top

C#:   new Random().Next(1, 101)
来源：http://vin.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://eih.ppjwa.cn

Py:   "yes" if x > 0 else "no"
来源：http://wml.cqqwz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pfb.hnqzz.top

JS:   x > 0 ? "yes" : "no"
来源：http://cps.ehwqpu.com

TS:   x > 0 ? "yes" : "no"
来源：http://lcz.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://zzi.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://iun.yj20258.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ubk.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://inh.gotoacloud.top

[A12] 字符串插值 / 格式化
来源：http://sdc.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sqx.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qjs.xuetiantiany.cn

JS:   `Hello, ${name}!`
来源：http://xit.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://let.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://gpn.jianghu66.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uvr.xuanzx.com

Ruby: "Hello, #{name}!"
来源：http://tjk.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://zzt.jianghu66.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ydd.guannengcc.top

Py:   "第一行\n第二行"
来源：http://flb.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://gph.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://ito.nwbrower.top

TS:   "第一行\n第二行"
来源：http://abo.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://wdo.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://one.havefunace.top

Ruby: "第一行\n第二行"
来源：http://vra.yueranfly.top

C#:   "第一行\n第二行"
来源：http://xku.yj20258888.top

[A14] 注释写法
来源：http://rih.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://voa.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gba.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://qul.c1oappe.top

TS:   // 单行；/* 多行 */
来源：http://srv.sjlbkw.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pak.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://asl.meibo888.top

Ruby: # 单行；=begin 多行 =end
来源：http://ypo.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://ptx.bbcook.cn

[A15] 空值判断与默认值
来源：http://cln.jinqigfzy.top

Py:   value = data or "默认值"
来源：http://kcw.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://ugj.haohaochexian.top

JS:   const value = data ?? "默认值";
来源：http://dhh.jinyuanbaomall.cn

TS:   const value = data ?? "默认值";
来源：http://qth.chenjidiqi.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rwz.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://oqm.yfazqb.com

Ruby: value = data || "默认值"
来源：http://efg.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://vsa.kuanghao11.cn

[A16] 真假值判断规则
来源：http://grd.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://diw.hesvh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://euf.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gme.ivvv.top

TS:   if (!x) {}
来源：http://wst.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rja.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dkt.hcnkem.com

Ruby: unless x            # nil 与 false 为假
来源：http://jpw.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kau.gotoacloud.top

[A17] 位运算
来源：http://oog.jiagoushi.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lbw.svipenyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bbp.jinyuanbaomall.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfi.hcnkem.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iby.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogl.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hhn.gotoacloud.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hsy.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afh.quarkkingdee.top

[A18] 字符与 ASCII 码互转
来源：http://sgh.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://swh.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://luw.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xxg.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tld.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://jyf.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zsl.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://yyq.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://fvz.yvedp.cn

[A19] 交换两个变量
来源：http://zzh.ehwqpu.com

Py:   a, b = b, a
来源：http://avr.zhixingplan.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dju.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://non.nwbrower.top

TS:   [a, b] = [b, a];
来源：http://mtg.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://umr.jyoumei.cn

Go:   a, b = b, a
来源：http://ugy.dianchejie.cn

Ruby: a, b = b, a
来源：http://lli.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://vxn.zhengqikj.top

[A20] 读取标准输入
来源：http://tho.hcnkem.com

Py:   name = input("请输入：")
来源：http://ocl.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://irz.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hdr.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://zgv.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://ebe.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mkb.vehdjk.com

Ruby: gets.chomp
来源：http://ouv.sxryk.cn

C#:   Console.ReadLine();
来源：http://nup.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://jeg.hnxiangtu.top

Py:   f"{3.14159:.2f}"
来源：http://dbj.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hsk.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://xnt.kuanghao11.cn

TS:   (3.14159).toFixed(2)
来源：http://lwj.dashuyun.cn

Java: String.format("%.2f", 3.14159)
来源：http://vxm.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://myc.ydzc1.top

Ruby: format("%.2f", 3.14159)
来源：http://ukq.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://ioe.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://cug.fzhhl.top

Py:   len(s)
来源：http://krl.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bef.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://npj.meibo888.top

TS:   s.length
来源：http://hwf.sjlbkw.cn

Java: s.length()
来源：http://nsi.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wax.birdmap.top

Ruby: s.length
来源：http://fot.meibo888.top

C#:   s.Length
来源：http://aud.aibaodan.cn

[A23] 大小写转换
来源：http://tbd.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qiz.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hvu.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://axx.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hcf.chenzaomai.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jfc.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hah.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://skw.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kal.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://wpy.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xkp.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nrx.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zyw.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gqn.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lqy.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://yeg.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hcm.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vmx.yuanzhike.top

[A25] 字符串比较
来源：http://jor.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://yvr.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bob.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mlb.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://itz.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://soo.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zqq.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://osc.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sxq.jinqigfzy.top

[A26] 类型转换总览
来源：http://fir.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ece.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zac.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bqf.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://kgb.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://niw.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ekj.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://iwz.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hzc.cucudq.cn

================================================================================
来源：http://rkv.bjfxy.top

B. 流程控制
来源：http://mpr.cdnleiting.top

================================================================================
来源：http://cqc.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://mdw.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sfq.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://boi.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nmj.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nhy.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xrh.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yjo.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pvm.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nfj.shuidangran.top

[B02] 多分支 else if / elif
来源：http://faj.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wbi.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lig.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vhi.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnj.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jej.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://she.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xym.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jol.zycfv.cn

[B03] switch / match / case
来源：http://lwf.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://buc.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zvh.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bhm.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://noa.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ktp.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://omu.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cup.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hbn.zhengqikj.top

[B04] for 计数循环
来源：http://kld.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://fjo.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jlr.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ybo.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qze.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nxk.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eke.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://csp.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jdu.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://uro.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://fgs.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oyr.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nss.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ghu.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qwo.jinghuilouyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rzx.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://jxh.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jrp.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://bbz.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://iwk.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ldd.ppjwa.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pob.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://upc.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://foy.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zyy.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ykv.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rbm.fehbvm.com

[B07] while 循环
来源：http://tjd.yuxming.cn

Py:   while i < 10: i += 1
来源：http://wzx.xingfuxueyuan.xyz


<!-- 参考信息 -->