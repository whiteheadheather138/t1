代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pzg.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rvo.tarul.cn

TS:   typeof x; x instanceof Date
来源：http://fuo.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xjr.hammf.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zfi.cdnleiting.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qao.aibaodan.cn

C#:   x.GetType().Name; x is int
来源：http://fic.jiagoushi.top

[A05] 整数除法与取模
来源：http://qux.shanyushiyangtech.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://otj.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vae.guannengcc.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dad.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://duc.redwolf501.top

Java: 7 / 2; 7 % 2
来源：http://glf.gaohongyu789.top

Go:   7 / 2; 7 % 2
来源：http://hnh.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://elf.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://lev.wangdashe.top

[A06] 字符串转数字
来源：http://xow.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://psb.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rkg.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://guk.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://ooz.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iwn.redwolf501.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bml.epnwcf.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ufa.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qli.cqqwz.cn

[A07] 数字转字符串
来源：http://hld.yj20258888.top

Py:   str(42)
来源：http://oap.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://lyb.wangshuangyany.cn

JS:   String(42); (42).toString()
来源：http://mtx.andypj.xyz

TS:   String(42)
来源：http://pxm.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rzz.c1oappe.top

Go:   strconv.Itoa(42)
来源：http://xmz.fengsongda.top

Ruby: 42.to_s
来源：http://nom.shzxlz.cn

C#:   42.ToString()
来源：http://grx.316326.xyz

[A08] 取整与四舍五入
来源：http://rjr.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://myd.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://haj.zhaomingkeji.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sgk.zhijiandao.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lwu.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jve.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zxm.ydzc1.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nep.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hvy.jinyuanbaomall.cn

[A09] 绝对值与最大最小值
来源：http://rrn.ppjwa.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ykl.gzhubu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jqx.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uql.yuxming.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bge.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wuu.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xfl.mhx1999.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qku.52xcode.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zkd.vehdjk.com

[A10] 生成随机数
来源：http://kzf.fzhhl.top

Py:   import random; random.randint(1, 100)
来源：http://niy.vqdsnc.cn

PHP:  random_int(1, 100);
来源：http://dht.zhoulong.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ofd.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aoi.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://vzv.fengsongda.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://obq.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://dzf.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://sfg.316326.xyz

[A11] 条件表达式（三元）
来源：http://ilg.ydjk.org.cn

Py:   "yes" if x > 0 else "no"
来源：http://vfj.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cxn.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://gyf.jiagoushi.top

TS:   x > 0 ? "yes" : "no"
来源：http://cdf.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://gzk.yuxming.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bhb.zhengqikj.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ycg.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://gbk.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://cia.jiagoushi.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fbs.fktsv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://imk.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://pnb.vehdjk.com

TS:   `Hello, ${name}!`
来源：http://jcj.ppjwa.cn

Java: "Hello, %s!".formatted(name)
来源：http://ioe.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://quw.xinyue.icu

Ruby: "Hello, #{name}!"
来源：http://osq.yueranfly.top

C#:   $"Hello, {name}!"
来源：http://yqn.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xss.zhongyouzk.top

Py:   "第一行\n第二行"
来源：http://bhy.daxiang520.top

PHP:  "第一行\n第二行"
来源：http://lev.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://atw.hfpthk.cn

TS:   "第一行\n第二行"
来源：http://xnq.c1oappe.top

Java: "第一行\n第二行"
来源：http://yvo.gotoacloud.top

Go:   "第一行\n第二行"
来源：http://hyg.yj202588.top

Ruby: "第一行\n第二行"
来源：http://ldy.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://ryc.gogol.net.cn

[A14] 注释写法
来源：http://ure.cucudq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://crm.nwbrower.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://szx.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://mkp.jianghu66.top

TS:   // 单行；/* 多行 */
来源：http://ina.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dkl.redwolf501.top

Go:   // 单行；/* 多行 */
来源：http://dup.xinyue.icu

Ruby: # 单行；=begin 多行 =end
来源：http://fbo.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://sug.yonumen.top

[A15] 空值判断与默认值
来源：http://pxl.iojbl.cn

Py:   value = data or "默认值"
来源：http://mtt.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://hjx.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://rmb.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://oyu.zdqjudy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rjm.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://reb.ppjwa.cn

Ruby: value = data || "默认值"
来源：http://efz.xylfe.cn

C#:   var value = data ?? "默认值";
来源：http://xwh.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://hwu.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uex.zdqjudy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xho.fengsongda.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nso.ivvv.top

TS:   if (!x) {}
来源：http://xig.yangfankeji.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xlg.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nhi.wangshuangyany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mln.havefunace.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jlv.pengpengdd.cyou

[A17] 位运算
来源：http://aws.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncr.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tom.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixe.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uqq.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xsm.yangfankeji.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://icd.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ytn.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hrg.xziqi.cn

[A18] 字符与 ASCII 码互转
来源：http://ema.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://imu.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://gko.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://acg.sysykeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ktw.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://yrf.zdbjq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mwb.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://ike.yanxiufei.cn

C#:   (int)'A'; (char)65
来源：http://omd.nanxuanxn.top

[A19] 交换两个变量
来源：http://sfv.svipenyu.cn

Py:   a, b = b, a
来源：http://mvp.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://uif.yuanzhike.top

JS:   [a, b] = [b, a];
来源：http://prk.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://qgk.hfpthk.cn

Java: int t = a; a = b; b = t;
来源：http://chj.yanxiufei.cn

Go:   a, b = b, a
来源：http://fzh.sysykeji.top

Ruby: a, b = b, a
来源：http://ann.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://ycd.xuetiantiany.cn

[A20] 读取标准输入
来源：http://zta.svipenyu.cn

Py:   name = input("请输入：")
来源：http://fgp.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pte.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://doj.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://luu.hywenlv.cn

Java: new Scanner(System.in).nextLine()
来源：http://lyl.snrcjt.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://siu.gotoacloud.top

Ruby: gets.chomp
来源：http://oyk.yj20258.top

C#:   Console.ReadLine();
来源：http://eto.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://gbj.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://quw.uphjek.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qmh.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://bqh.havefunace.top

TS:   (3.14159).toFixed(2)
来源：http://mii.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://hub.ppjwa.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lmv.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://bdu.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://mij.9152youxi.cn

[A22] 获取字符串长度
来源：http://prh.nwbrower.top

Py:   len(s)
来源：http://vgh.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kjs.9152youxi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pro.snrcjt.cn

TS:   s.length
来源：http://ope.kuanghao11.cn

Java: s.length()
来源：http://zft.wangdashe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gfx.xingfuxueyuan.xyz

Ruby: s.length
来源：http://ukh.quarkkingdee.top

C#:   s.Length
来源：http://uqv.52xcode.cn

[A23] 大小写转换
来源：http://sxf.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://pkg.dianchejie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bjo.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yev.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hnw.fktsv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://azp.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fyp.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vxj.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rjw.yangfankeji.com

[A24] 去除首尾空白
来源：http://jim.sweek.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lnw.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dmm.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vue.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qbe.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wdy.cashguo.top

Go:   strings.TrimSpace(s)
来源：http://ykh.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lnj.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ilj.snrcjt.cn

[A25] 字符串比较
来源：http://rfe.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://aaq.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xmi.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hqa.bbcook.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://now.ivvv.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uia.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zuy.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://mfl.hammf.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nxm.chenlongwang.top

[A26] 类型转换总览
来源：http://yhx.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ado.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zjl.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hok.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://nsp.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yrg.sysykeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oej.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vpw.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hyh.ydzc1.top

================================================================================
来源：http://jcw.zycfv.cn

B. 流程控制
来源：http://cqh.dashuyun.cn

================================================================================
来源：http://nlz.zdqjudy.top

[B01] 条件判断 if / else
来源：http://mtx.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://sny.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jep.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://orv.shzxlz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gmc.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tpc.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hth.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wgv.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zhv.tanke756.top

[B02] 多分支 else if / elif
来源：http://fpv.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qlq.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kay.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsj.yuanzhike.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ryw.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swr.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nme.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rhe.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqy.cdnleiting.top

[B03] switch / match / case
来源：http://rdj.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fdn.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cpa.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwv.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://glo.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vir.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qvh.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lgm.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uuu.ehwqpu.com

[B04] for 计数循环
来源：http://dnx.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://azz.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ssj.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uyf.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qmk.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qvx.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zbi.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://ejg.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dze.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://ltk.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://irk.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vfu.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dqm.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iij.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dcn.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://toz.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://qyi.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://maw.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://kzn.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tjd.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gll.ppjwa.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vky.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnl.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://can.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gph.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nnb.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://alu.andypj.xyz

[B07] while 循环
来源：http://yrx.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://gky.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://nvr.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://rpn.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://trw.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://azh.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hes.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://zly.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://emr.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://abd.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://ook.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://esb.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://pog.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://chb.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://rdq.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iuc.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://eef.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://ajc.gzhubu.top

[B09] break 与 continue
来源：http://qfs.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://abx.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fkt.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfq.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzv.yj20258.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adr.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pne.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wrn.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujf.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://kkk.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dqe.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lkp.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dzd.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qhd.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gmb.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oib.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xdt.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rdt.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://ljh.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://qtx.sysykeji.top


<!-- 参考信息 -->