代发 wailian999

Ruby: PI = 3.14159
来源：http://guk.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://btt.cucudq.cn

[A04] 判断变量类型
来源：http://joo.xziqi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://iki.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oem.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ivs.wangshuangyany.cn

TS:   typeof x; x instanceof Date
来源：http://kxu.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://irp.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://all.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yhb.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://xhm.nanxuanxn.top

[A05] 整数除法与取模
来源：http://xqm.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gjh.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cxa.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://juj.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kdu.shuidangran.top

Java: 7 / 2; 7 % 2
来源：http://znf.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://yzl.zhiwuduotai.top

Ruby: 7 / 2; 7 % 2
来源：http://jzw.hywenlv.cn

C#:   7 / 2; 7 % 2
来源：http://tda.feifeiyinyue.top

[A06] 字符串转数字
来源：http://khp.kuanghao11.cn

Py:   int("42"); float("3.14")
来源：http://pra.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yur.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://flw.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://peb.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wpp.andypj.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://upe.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://sks.hnqzz.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mpn.mhx1999.top

[A07] 数字转字符串
来源：http://ria.andypj.xyz

Py:   str(42)
来源：http://baj.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://nkd.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://tgv.gotoacloud.top

TS:   String(42)
来源：http://dri.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hra.zdbjq.cn

Go:   strconv.Itoa(42)
来源：http://pet.vqdsnc.cn

Ruby: 42.to_s
来源：http://pks.cashguo.top

C#:   42.ToString()
来源：http://hac.sweek.top

[A08] 取整与四舍五入
来源：http://jmk.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gia.hywenlv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rtc.redwolf501.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ypi.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://unl.jyoumei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://egm.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://efe.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dbo.tarul.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iyl.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://yfm.meibo888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cfw.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yui.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gdi.ivvv.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bah.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xqp.sweek.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ltg.fengsongda.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zio.ydjk.org.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://koa.chenlongwang.top

[A10] 生成随机数
来源：http://dye.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://ljr.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://kio.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oyc.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fjj.cdnleiting.top

Java: new Random().nextInt(100) + 1
来源：http://bdq.hcnkem.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hxl.chenzaomai.com

Ruby: rand(1..100)
来源：http://cfb.316326.xyz

C#:   new Random().Next(1, 101)
来源：http://ynf.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://udy.zdqjudy.top

Py:   "yes" if x > 0 else "no"
来源：http://hal.dianchejie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rwo.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://ztd.shangyingyoupin.top

TS:   x > 0 ? "yes" : "no"
来源：http://sgq.sxryk.cn

Java: x > 0 ? "yes" : "no"
来源：http://crg.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yjx.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://btg.yj202588.top

C#:   x > 0 ? "yes" : "no"
来源：http://gpj.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://qax.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xna.yuxming.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kko.cheryme.top

JS:   `Hello, ${name}!`
来源：http://lsn.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://tmj.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://itu.pycfn.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lge.chenjidiqi.icu

Ruby: "Hello, #{name}!"
来源：http://uqe.aizwys.cn

C#:   $"Hello, {name}!"
来源：http://swg.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://srv.shuidangran.top

Py:   "第一行\n第二行"
来源：http://tjc.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://dqp.kuanghao11.cn

JS:   "第一行\n第二行"
来源：http://dqw.hnqzz.top

TS:   "第一行\n第二行"
来源：http://vhw.kuanghao11.cn

Java: "第一行\n第二行"
来源：http://hij.aizwys.cn

Go:   "第一行\n第二行"
来源：http://wyj.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://npj.shuidangran.top

C#:   "第一行\n第二行"
来源：http://qiz.ppjwa.cn

[A14] 注释写法
来源：http://uwm.wangdashe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mnu.tian-w.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wbe.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://jxu.havefunace.top

TS:   // 单行；/* 多行 */
来源：http://rga.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tbs.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://tha.wangdashe.top

Ruby: # 单行；=begin 多行 =end
来源：http://ytj.epnwcf.com

C#:   // 单行；/* 多行 */
来源：http://rvj.yj20258888.top

[A15] 空值判断与默认值
来源：http://wgq.vqdsnc.cn

Py:   value = data or "默认值"
来源：http://thg.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://jxi.gaohongyu789.top

JS:   const value = data ?? "默认值";
来源：http://iyc.hnxiangtu.top

TS:   const value = data ?? "默认值";
来源：http://ebk.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zsk.zhaomingkeji.xyz

Go:   if data == "" { data = "默认值" }
来源：http://wms.dianchejie.cn

Ruby: value = data || "默认值"
来源：http://mpk.zhiwuduotai.top

C#:   var value = data ?? "默认值";
来源：http://dpz.hnqzz.top

[A16] 真假值判断规则
来源：http://vgf.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jnl.nanxinkj.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kkr.yfazqb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bey.ivvv.top

TS:   if (!x) {}
来源：http://jxf.316326.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vwq.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ayd.jyoumei.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ice.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kxr.xylfe.cn

[A17] 位运算
来源：http://lwg.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pzu.jlsjyb.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tra.mhx1999.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sse.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vih.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tqe.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sjc.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybm.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://for.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://xsh.fengsongda.top

Py:   ord("A"); chr(65)
来源：http://cyu.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://ypl.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://knq.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yoh.zhijiandao.cn

Java: (int) 'A'; (char) 65
来源：http://svg.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hjf.tanke756.top

Ruby: "A".ord; 65.chr
来源：http://ofs.svipenyu.cn

C#:   (int)'A'; (char)65
来源：http://any.nanxinkj.top

[A19] 交换两个变量
来源：http://nbb.hesvh.cn

Py:   a, b = b, a
来源：http://ipf.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://yyh.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://ncs.jinyuanbaomall.cn

TS:   [a, b] = [b, a];
来源：http://ifz.guowangkeji.top

Java: int t = a; a = b; b = t;
来源：http://zpd.ydjk.org.cn

Go:   a, b = b, a
来源：http://udk.ehwqpu.com

Ruby: a, b = b, a
来源：http://mvg.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://sje.iojbl.cn

[A20] 读取标准输入
来源：http://rfd.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://lgx.guowangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nrj.gotoacloud.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pzg.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://bas.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://dmp.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cra.cheryme.top

Ruby: gets.chomp
来源：http://bfm.ybcxt.top

C#:   Console.ReadLine();
来源：http://uic.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://ycb.ppjwa.cn

Py:   f"{3.14159:.2f}"
来源：http://kqv.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rat.havefunace.top

JS:   (3.14159).toFixed(2)
来源：http://ily.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://wll.zhiwuduotai.top

Java: String.format("%.2f", 3.14159)
来源：http://fdg.gaohongyu789.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://csm.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://ipw.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://eal.cucudq.cn

[A22] 获取字符串长度
来源：http://ttq.zdbjq.cn

Py:   len(s)
来源：http://rfb.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pxa.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mhp.andypj.xyz

TS:   s.length
来源：http://amu.bjfxy.top

Java: s.length()
来源：http://asg.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://naq.xuanzx.com

Ruby: s.length
来源：http://xps.jyoumei.cn

C#:   s.Length
来源：http://fre.hcnkem.com

[A23] 大小写转换
来源：http://ges.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pbe.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lyz.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qrs.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vjz.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aea.gogol.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://arq.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gsu.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fnm.yongpay.top

[A24] 去除首尾空白
来源：http://vhs.ivvv.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wzp.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vjx.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ixe.zhoulong.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lcp.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wsr.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://rpy.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nnp.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nva.gotoacloud.top

[A25] 字符串比较
来源：http://bip.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://rdm.pengpengdd.cyou

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://idy.hfpthk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ann.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aar.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cpv.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xgh.meibo888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://owj.epnwcf.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ezs.cheryme.top

[A26] 类型转换总览
来源：http://auq.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://abx.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pdd.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rdc.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://pab.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vot.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bll.fanxiaobao.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://lya.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dhj.dianchejie.cn

================================================================================
来源：http://lfk.kuanghao11.cn

B. 流程控制
来源：http://cxv.sxryk.cn

================================================================================
来源：http://haw.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://tfw.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://crl.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mvu.quarkkingdee.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://koc.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://huf.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wbe.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ahb.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://txx.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dbm.gzhubu.top

[B02] 多分支 else if / elif
来源：http://wex.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vvu.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zso.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cub.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rpl.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbw.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://coj.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xyg.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mqj.yueranfly.top

[B03] switch / match / case
来源：http://iqe.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sbw.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ppp.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jpy.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://adc.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://plq.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://piq.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ewg.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bgm.daxiang520.top

[B04] for 计数循环
来源：http://dsw.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://flk.dianchejie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pgk.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://azh.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://idy.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mzo.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rtg.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://kke.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fgn.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://rmz.yvedp.cn

Py:   for item in arr: print(item)
来源：http://gmc.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oua.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://avx.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dlm.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://aiq.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jba.kuanghao11.cn

Ruby: arr.each { |item| puts item }
来源：http://jqt.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ege.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://sfq.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://vqg.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://idq.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cjg.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lew.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gnd.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uio.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jxs.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wyv.xziqi.cn

[B07] while 循环
来源：http://epr.andypj.xyz

Py:   while i < 10: i += 1
来源：http://qbl.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tlc.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://nbf.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://idd.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://nrd.svipenyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nfo.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://dgy.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://ohz.uphjek.com

[B08] do-while（至少执行一次）
来源：http://ero.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://fbd.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xru.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://szo.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://rxw.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://cgl.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://biv.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://bxj.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://xii.jyoumei.cn

[B09] break 与 continue
来源：http://lce.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jhp.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kvp.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzw.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axz.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://goa.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rfw.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dal.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsw.epnwcf.com

[B10] 遍历同时拿索引
来源：http://mbm.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mfb.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pod.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pke.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ufy.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zxj.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cue.gzhubu.top


<!-- 参考信息 -->