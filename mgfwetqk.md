代发 wailian999

================================================================================
来源：http://zlv.hongshengwenyu.top

A. 基础语法与类型
来源：http://tii.daria6918.cn

================================================================================
来源：http://ljs.xziqi.cn

[A01] Hello World
来源：http://roj.ydzc1.top

Py:   print("Hello, World!")
来源：http://ppg.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://hiw.zhengqikj.top

JS:   console.log("Hello, World!");
来源：http://ijz.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ctt.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://cde.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://ezj.yonumen.top

Ruby: puts "Hello, World!"
来源：http://aew.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gmm.xziqi.cn

[A02] 变量声明与赋值
来源：http://vkg.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uyv.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zwc.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://bqq.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jzg.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://rtw.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://vbg.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://agp.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://wui.yj202588.top

[A03] 常量定义
来源：http://qpw.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bvy.yueranfly.top

PHP:  const PI = 3.14159;
来源：http://ame.smart0.xyz

JS:   const PI = 3.14159;
来源：http://twy.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://uyb.xziqi.cn

Java: static final double PI = 3.14159;
来源：http://tps.birdmap.top

Go:   const PI = 3.14159
来源：http://opd.havefunace.top

Ruby: PI = 3.14159
来源：http://qjf.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://egz.uphjek.com

[A04] 判断变量类型
来源：http://ije.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://mhz.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sme.jiagoushi.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hvs.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://hzz.pycfn.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qnu.smart0.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://wsj.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://otp.shuidangran.top

C#:   x.GetType().Name; x is int
来源：http://cyn.zdbjq.cn

[A05] 整数除法与取模
来源：http://ckb.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tbv.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dyb.zdbjq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xdz.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zqv.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://pgm.jinyuanbaomall.cn

Go:   7 / 2; 7 % 2
来源：http://mgj.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://vxm.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://bbo.gogol.net.cn

[A06] 字符串转数字
来源：http://nds.jqgfzy.top

Py:   int("42"); float("3.14")
来源：http://mrl.zhiwuduotai.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xuh.jinyuanbaomall.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tnl.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://cbt.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jpq.cheryme.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mwa.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jyv.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://who.mhx1999.top

[A07] 数字转字符串
来源：http://pio.hammf.cn

Py:   str(42)
来源：http://kuw.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://rhx.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://omb.dianchejie.cn

TS:   String(42)
来源：http://fws.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://aob.hnqzz.top

Go:   strconv.Itoa(42)
来源：http://jzr.wangshuangyany.cn

Ruby: 42.to_s
来源：http://qko.nanxinkj.top

C#:   42.ToString()
来源：http://hed.zycfv.cn

[A08] 取整与四舍五入
来源：http://gya.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://giv.zhiwuduotai.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nbd.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tru.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lkb.guannengcc.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qdf.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fdt.tian-w.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://unb.jqgfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zuj.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://qzl.mhx1999.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ndi.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://waf.fanxiaobao.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nxq.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kqa.shangyingyoupin.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hmh.yj20258888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://knb.yuxming.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xke.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nrn.hnqzz.top

[A10] 生成随机数
来源：http://nkz.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://dns.bbcook.cn

PHP:  random_int(1, 100);
来源：http://nfu.xylfe.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ujf.cdnleiting.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yuh.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://ljk.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xqf.xinyue.icu

Ruby: rand(1..100)
来源：http://ody.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://dbu.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://fch.zhiwuduotai.top

Py:   "yes" if x > 0 else "no"
来源：http://ffq.nanxinkj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pcs.smart0.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://aah.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nfo.shzxlz.cn

Java: x > 0 ? "yes" : "no"
来源：http://clp.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://eaj.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ngc.zdbjq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cnb.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://qwm.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wve.ywan-chungtsiang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jfk.hnxiangtu.top

JS:   `Hello, ${name}!`
来源：http://giq.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://eql.daria6918.cn

Java: "Hello, %s!".formatted(name)
来源：http://ztk.shanyushiyangkeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mqm.zhongyouzk.top

Ruby: "Hello, #{name}!"
来源：http://upn.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://ffr.svipenyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uye.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://jez.xingfuxueyuan.xyz

PHP:  "第一行\n第二行"
来源：http://flw.wangdashe.top

JS:   "第一行\n第二行"
来源：http://nzx.xziqi.cn

TS:   "第一行\n第二行"
来源：http://qgp.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://naz.hnqzz.top

Go:   "第一行\n第二行"
来源：http://aoe.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://lqy.yfazqb.com

C#:   "第一行\n第二行"
来源：http://vyi.jinqigufen.top

[A14] 注释写法
来源：http://mgm.yongpay.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nym.meibo888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wdt.zdqjudy.top

JS:   // 单行；/* 多行 */
来源：http://vgj.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://zdj.xuanzx.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jxy.zhixingplan.top

Go:   // 单行；/* 多行 */
来源：http://jfy.jlsjyb.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vfy.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://nkn.yueranfly.top

[A15] 空值判断与默认值
来源：http://ctn.c1oappe.top

Py:   value = data or "默认值"
来源：http://prw.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://sqz.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://axi.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://mtb.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tkx.bjfxy.top

Go:   if data == "" { data = "默认值" }
来源：http://jjc.hesvh.cn

Ruby: value = data || "默认值"
来源：http://cor.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://kcc.jyoumei.cn

[A16] 真假值判断规则
来源：http://joe.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://srj.shuidangran.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sti.nwbrower.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://otg.hfpthk.cn

TS:   if (!x) {}
来源：http://hhw.tian-w.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zla.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rcv.0kj1m.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xjo.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://juf.shangyingyoupin.top

[A17] 位运算
来源：http://tqv.shzxlz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fca.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://icf.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lta.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://emx.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://trr.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://quw.jinqigfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zcq.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ilb.wangshuangyany.cn

[A18] 字符与 ASCII 码互转
来源：http://bei.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://pxw.chenlongwang.top

PHP:  ord("A"); chr(65)
来源：http://gvb.yj20258888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kut.yfazqb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://plp.bbcook.cn

Java: (int) 'A'; (char) 65
来源：http://fil.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uyw.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://awm.sweek.top

C#:   (int)'A'; (char)65
来源：http://puh.ctjpmb.com

[A19] 交换两个变量
来源：http://ajn.havefunace.top

Py:   a, b = b, a
来源：http://sun.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://grd.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://xeb.havefunace.top

TS:   [a, b] = [b, a];
来源：http://deh.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://lqn.jqgufenzy.top

Go:   a, b = b, a
来源：http://wqd.ydjk.org.cn

Ruby: a, b = b, a
来源：http://uhz.yanxiufei.cn

C#:   (a, b) = (b, a);
来源：http://tkr.vqdsnc.cn

[A20] 读取标准输入
来源：http://zlh.fengsongda.top

Py:   name = input("请输入：")
来源：http://cem.jqgufenzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://aev.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lui.ctjpmb.com

TS:   // Node.js：readline 模块
来源：http://wcm.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://jzd.quarkkingdee.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://asq.gzhubu.top

Ruby: gets.chomp
来源：http://yxs.yuxming.cn

C#:   Console.ReadLine();
来源：http://qsn.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://ube.sjlbkw.cn

Py:   f"{3.14159:.2f}"
来源：http://czm.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ohm.dashuyun.cn

JS:   (3.14159).toFixed(2)
来源：http://ipo.shanyushiyangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://ygq.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://ijs.jinyuanbaomall.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://byv.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://nfg.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://iqw.gogol.net.cn

[A22] 获取字符串长度
来源：http://yfl.kuanghao11.cn

Py:   len(s)
来源：http://xyo.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pnp.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fxf.fehbvm.com

TS:   s.length
来源：http://awk.jqgfzy.top

Java: s.length()
来源：http://llj.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uuy.yueranfly.top

Ruby: s.length
来源：http://tpz.hysaishi.cn

C#:   s.Length
来源：http://dvu.nanxinkj.top

[A23] 大小写转换
来源：http://dfo.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tbd.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://quq.hnqzz.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zrn.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yjx.meibo888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qka.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bue.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sjy.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ubj.yangfankeji.com

[A24] 去除首尾空白
来源：http://rjc.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nlo.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hyi.cdnleiting.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lqt.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dwa.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fio.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://yje.aizwys.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nwa.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ywk.hnqzz.top

[A25] 字符串比较
来源：http://dgh.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://rbx.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gzg.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zkt.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cnh.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pyx.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://toj.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jej.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yjv.tianlin.xyz

[A26] 类型转换总览
来源：http://vto.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://osx.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pkb.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fac.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://okm.hnqzz.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lny.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vkx.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aqx.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ift.ywan-chungtsiang.top

================================================================================
来源：http://mfd.zycfv.cn

B. 流程控制
来源：http://wxh.hfpthk.cn

================================================================================
来源：http://ujo.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://tpu.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xif.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://frg.vqdsnc.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sag.jyoumei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bmr.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xpo.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pvy.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cwm.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fjd.gzhubu.top

[B02] 多分支 else if / elif
来源：http://dbx.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uav.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zbi.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bwp.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdy.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mrk.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nso.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eya.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfe.yueranfly.top

[B03] switch / match / case
来源：http://iyf.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nlv.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yog.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbt.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://taa.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hgj.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uii.havefunace.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ayk.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qdd.gzhubu.top

[B04] for 计数循环
来源：http://jwg.bjfxy.top

Py:   for i in range(10): print(i)
来源：http://suh.gaohongyu789.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://plb.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://knw.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hhw.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mtv.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kll.ivvv.top

Ruby: 10.times { |i| puts i }
来源：http://bch.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yqr.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://zdp.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://kdy.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xrj.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://ktq.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://atf.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ucu.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tsk.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://ztk.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jbh.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://pgq.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nqb.xziqi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yzp.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tpy.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spa.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oep.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://amp.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nnm.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nwu.birdmap.top

[B07] while 循环
来源：http://jyc.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://xtm.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pib.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://gnf.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://wcc.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://rab.xuanzx.com


<!-- 参考信息 -->