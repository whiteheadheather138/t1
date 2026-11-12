代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://itu.uphjek.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hvp.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://smu.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cco.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://rbn.bbcook.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://egh.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://lov.fanxiaobao.xyz

[A05] 整数除法与取模
来源：http://pwf.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://olt.yonumen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kob.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ule.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://guq.sweek.top

Java: 7 / 2; 7 % 2
来源：http://pge.shzxlz.cn

Go:   7 / 2; 7 % 2
来源：http://zrk.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://snu.jqgfzy.top

C#:   7 / 2; 7 % 2
来源：http://lxg.bjfxy.top

[A06] 字符串转数字
来源：http://awb.redwolf501.top

Py:   int("42"); float("3.14")
来源：http://jaq.ywan-chungtsiang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ljn.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jbb.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://ovq.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sva.havefunace.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mdm.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wwq.vehdjk.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kvl.ydjk.org.cn

[A07] 数字转字符串
来源：http://zpt.zycfv.cn

Py:   str(42)
来源：http://qec.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://cio.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://sly.xinyue.icu

TS:   String(42)
来源：http://tli.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ubm.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://gfa.ctjpmb.com

Ruby: 42.to_s
来源：http://ton.jinyuanbaomall.cn

C#:   42.ToString()
来源：http://yfa.andypj.xyz

[A08] 取整与四舍五入
来源：http://vry.meibo888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sfl.hongshengwenyu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rto.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wce.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oow.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lij.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ozu.vehdjk.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://pmo.nanxinkj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yvl.birdmap.top

[A09] 绝对值与最大最小值
来源：http://rgx.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ejr.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://saf.wangshuangyany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gxc.yangfankeji.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cov.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ela.shangyingyoupin.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vyf.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uar.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hxp.hcnkem.com

[A10] 生成随机数
来源：http://urb.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://whd.cucudq.cn

PHP:  random_int(1, 100);
来源：http://glh.wangshuangyany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pco.zycfv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://onp.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://abd.feifeiyinyue.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wop.quarkkingdee.top

Ruby: rand(1..100)
来源：http://ieb.xingfuxueyuan.xyz

C#:   new Random().Next(1, 101)
来源：http://jim.xziqi.cn

[A11] 条件表达式（三元）
来源：http://jnc.fktsv.cn

Py:   "yes" if x > 0 else "no"
来源：http://sdx.316326.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://kqz.jinghuilouyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wel.tarul.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lfh.epnwcf.com

Java: x > 0 ? "yes" : "no"
来源：http://wfd.tanke756.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hvh.xuanzx.com

Ruby: x > 0 ? "yes" : "no"
来源：http://tel.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://poi.nanxinkj.top

[A12] 字符串插值 / 格式化
来源：http://zff.hnqzz.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://imi.gotoacloud.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ypt.ivvv.top

JS:   `Hello, ${name}!`
来源：http://clh.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://ovz.hywenlv.cn

Java: "Hello, %s!".formatted(name)
来源：http://vrq.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tla.sxryk.cn

Ruby: "Hello, #{name}!"
来源：http://lwv.yj20258.top

C#:   $"Hello, {name}!"
来源：http://gcr.xylfe.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://phh.jlsjyb.cn

Py:   "第一行\n第二行"
来源：http://wlf.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://fcs.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://seq.epnwcf.com

TS:   "第一行\n第二行"
来源：http://nov.fehbvm.com

Java: "第一行\n第二行"
来源：http://lwg.jinghuilouyu.cn

Go:   "第一行\n第二行"
来源：http://xsl.jqgufenzy.top

Ruby: "第一行\n第二行"
来源：http://vjj.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://jgj.cucudq.cn

[A14] 注释写法
来源：http://dxg.hnqzz.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qft.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xqi.zhoulong.xyz

JS:   // 单行；/* 多行 */
来源：http://lyg.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://udo.fanxiaobao.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cqj.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://mxi.yj202588.top

Ruby: # 单行；=begin 多行 =end
来源：http://uab.kuanghao11.cn

C#:   // 单行；/* 多行 */
来源：http://hwp.c1oappe.top

[A15] 空值判断与默认值
来源：http://kzl.tarul.cn

Py:   value = data or "默认值"
来源：http://swf.meibo888.top

PHP:  $value = $data ?? "默认值";
来源：http://wtc.jqgufenzy.top

JS:   const value = data ?? "默认值";
来源：http://fka.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://zum.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wix.feifeiyinyue.top

Go:   if data == "" { data = "默认值" }
来源：http://bli.fktsv.cn

Ruby: value = data || "默认值"
来源：http://edi.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://iwe.iojbl.cn

[A16] 真假值判断规则
来源：http://oxy.cheryme.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bae.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vou.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://clh.nwbrower.top

TS:   if (!x) {}
来源：http://lih.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rql.ybcxt.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tjm.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://zil.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ugm.jlsjyb.cn

[A17] 位运算
来源：http://tve.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmb.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bcj.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdx.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ssq.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jgu.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gif.hesvh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dvr.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ndw.epnwcf.com

[A18] 字符与 ASCII 码互转
来源：http://maj.iojbl.cn

Py:   ord("A"); chr(65)
来源：http://ezz.jlsjyb.cn

PHP:  ord("A"); chr(65)
来源：http://twx.xinyue.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tqb.guowangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wrl.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://boj.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kqb.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://cxe.yongpay.top

C#:   (int)'A'; (char)65
来源：http://hbz.chenzaomai.com

[A19] 交换两个变量
来源：http://cli.hammf.cn

Py:   a, b = b, a
来源：http://dlb.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wve.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://kuv.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://dbs.jinyuanbaomall.cn

Java: int t = a; a = b; b = t;
来源：http://nqz.xuanzx.com

Go:   a, b = b, a
来源：http://aer.hcnkem.com

Ruby: a, b = b, a
来源：http://rfd.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://ulv.fzhhl.top

[A20] 读取标准输入
来源：http://eli.cqqwz.cn

Py:   name = input("请输入：")
来源：http://gjq.gogol.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xod.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bdd.zhoulong.xyz

TS:   // Node.js：readline 模块
来源：http://tvp.9152youxi.cn

Java: new Scanner(System.in).nextLine()
来源：http://mnc.xziqi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sdi.zdbjq.cn

Ruby: gets.chomp
来源：http://quj.yongpay.top

C#:   Console.ReadLine();
来源：http://otz.yvedp.cn

[A21] 保留指定小数位输出
来源：http://eze.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://uwz.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jvn.tarul.cn

JS:   (3.14159).toFixed(2)
来源：http://bgi.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://mud.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://glo.fktsv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ios.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://prh.chenlongwang.top

C#:   3.14159.ToString("F2")
来源：http://plt.gotoacloud.top

[A22] 获取字符串长度
来源：http://hwu.hysaishi.cn

Py:   len(s)
来源：http://fft.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ubv.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://khi.shanyushiyangkeji.top

TS:   s.length
来源：http://hfh.gogol.net.cn

Java: s.length()
来源：http://kwd.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ufj.zhoulong.xyz

Ruby: s.length
来源：http://hzi.ppjwa.cn

C#:   s.Length
来源：http://tpq.zycfv.cn

[A23] 大小写转换
来源：http://occ.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://sim.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dog.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fmz.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eux.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tyt.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nzk.gaohongyu789.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oas.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mng.aizwys.cn

[A24] 去除首尾空白
来源：http://xdt.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aup.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pbv.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ugd.gogol.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zyn.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ala.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://aff.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://erl.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ppn.jlsjyb.cn

[A25] 字符串比较
来源：http://nqy.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://xpx.sjlbkw.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qpw.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vig.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pro.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://chh.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yho.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bng.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sfm.cucudq.cn

[A26] 类型转换总览
来源：http://oxf.yueranfly.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pqn.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tml.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pam.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://uyy.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://faj.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://twl.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cot.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ptr.feifeiyinyue.top

================================================================================
来源：http://tkp.dianchejie.cn

B. 流程控制
来源：http://ukx.meibo888.top

================================================================================
来源：http://pje.cqqwz.cn

[B01] 条件判断 if / else
来源：http://tlk.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ztp.yangfankeji.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fhs.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ugq.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dlu.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://okv.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tss.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jak.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dxk.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://cts.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mdv.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fvg.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kps.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uxo.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qfb.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ddd.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tmr.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vva.jiagoushi.top

[B03] switch / match / case
来源：http://hic.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jps.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://luy.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jtj.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iet.zhongyouzk.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wwc.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xjx.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nzu.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bny.gzhubu.top

[B04] for 计数循环
来源：http://ckb.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://pve.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nzv.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lvz.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kox.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hus.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lyv.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://szi.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jjb.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://ytg.sysykeji.top

Py:   for item in arr: print(item)
来源：http://wcl.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jzu.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://owj.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ovt.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://rzt.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pqo.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://wnw.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jkf.havefunace.top

[B06] 遍历字典 / 对象
来源：http://ook.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kgf.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mja.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://izz.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tbn.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://skb.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xgp.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fof.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cpo.sweek.top

[B07] while 循环
来源：http://ktl.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://qho.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://wmk.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://soq.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://sgu.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://qem.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xbz.gogol.net.cn

Ruby: while i < 10; i += 1; end
来源：http://kxo.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://fjo.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://ccb.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://xtj.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jvp.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://jzr.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://bsf.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://war.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://qqr.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://vxj.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://qjo.pycfn.com

[B09] break 与 continue
来源：http://yhj.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hlr.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qew.redwolf501.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dws.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhc.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfn.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ynr.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jmc.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwf.gzhubu.top

[B10] 遍历同时拿索引
来源：http://ulg.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uhu.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bym.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cos.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blc.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wvn.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://liv.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wrn.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ldi.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://lwz.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://edc.quarkkingdee.top


<!-- 参考信息 -->