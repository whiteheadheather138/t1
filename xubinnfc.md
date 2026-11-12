代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rfb.tarul.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://icv.c1oappe.top

TS:   typeof x; x instanceof Date
来源：http://rul.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jci.aizwys.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hfg.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jcq.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://wwz.ybcxt.top

[A05] 整数除法与取模
来源：http://icu.tarul.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fyd.iojbl.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ghk.meibo888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rwc.hfpthk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cjb.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://xwn.yfazqb.com

Go:   7 / 2; 7 % 2
来源：http://bmw.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://yye.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://evf.jinyuanbaomall.cn

[A06] 字符串转数字
来源：http://psw.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://lob.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bga.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tzx.tanke756.top

TS:   parseInt("42", 10); Number("42")
来源：http://lvw.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dtq.ydzc1.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kxw.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bbe.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://smt.haohaochexian.top

[A07] 数字转字符串
来源：http://xih.meibo888.top

Py:   str(42)
来源：http://bmm.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://zjf.cucudq.cn

JS:   String(42); (42).toString()
来源：http://ywd.yfazqb.com

TS:   String(42)
来源：http://qky.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lbp.kuanghao11.cn

Go:   strconv.Itoa(42)
来源：http://cdn.shuidangran.top

Ruby: 42.to_s
来源：http://vpq.uphjek.com

C#:   42.ToString()
来源：http://kbc.shanyushiyangtech.top

[A08] 取整与四舍五入
来源：http://brq.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vkt.hongshengwenyu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lqu.jinyuanbaomall.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://akx.iojbl.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jnn.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fbv.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xam.tarul.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mia.cdnleiting.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ary.zycfv.cn

[A09] 绝对值与最大最小值
来源：http://zsr.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ihw.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rqa.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tnk.shzxlz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kih.hesvh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nme.fzhhl.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cnm.hnqzz.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xwb.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zxx.shuidangran.top

[A10] 生成随机数
来源：http://adj.hnqzz.top

Py:   import random; random.randint(1, 100)
来源：http://oqa.fktsv.cn

PHP:  random_int(1, 100);
来源：http://niz.yj202588.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zlp.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qox.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://zmq.zdqjudy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bfd.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://qfj.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://hhf.hammf.cn

[A11] 条件表达式（三元）
来源：http://fba.svipenyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://plp.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rta.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sgd.yfazqb.com

TS:   x > 0 ? "yes" : "no"
来源：http://hsq.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://pot.zhijiandao.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fzk.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://nva.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://wjb.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://ytx.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zpd.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gfo.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://ckq.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://wfv.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://dzd.xylfe.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jjr.redwolf501.top

Ruby: "Hello, #{name}!"
来源：http://ztq.hongshengwenyu.top

C#:   $"Hello, {name}!"
来源：http://adl.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://orf.zhoulong.xyz

Py:   "第一行\n第二行"
来源：http://scc.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://yhk.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://zhn.yvedp.cn

TS:   "第一行\n第二行"
来源：http://msf.hywenlv.cn

Java: "第一行\n第二行"
来源：http://wop.zycfv.cn

Go:   "第一行\n第二行"
来源：http://vkf.sweek.top

Ruby: "第一行\n第二行"
来源：http://zbb.shuidangran.top

C#:   "第一行\n第二行"
来源：http://awn.yuxming.cn

[A14] 注释写法
来源：http://ixq.52xcode.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bzf.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wnn.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://vli.zdqjudy.top

TS:   // 单行；/* 多行 */
来源：http://its.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://khi.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://bfm.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dxe.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://hfd.fktsv.cn

[A15] 空值判断与默认值
来源：http://dnh.jianghu66.top

Py:   value = data or "默认值"
来源：http://drr.c1oappe.top

PHP:  $value = $data ?? "默认值";
来源：http://cxr.cdnleiting.top

JS:   const value = data ?? "默认值";
来源：http://dmw.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://tft.316326.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qzv.smart0.xyz

Go:   if data == "" { data = "默认值" }
来源：http://cfc.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://jkd.dashuyun.cn

C#:   var value = data ?? "默认值";
来源：http://rsz.tian-w.cn

[A16] 真假值判断规则
来源：http://mvg.jinghuilouyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lfb.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fqt.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qwu.zhaomingkeji.xyz

TS:   if (!x) {}
来源：http://ltt.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jfc.ehwqpu.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ulb.uphjek.com

Ruby: unless x            # nil 与 false 为假
来源：http://rkl.yuxming.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ekr.ivvv.top

[A17] 位运算
来源：http://gur.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tih.hywenlv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sps.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://idh.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pxi.sxryk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://avi.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://prv.jinqigfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zcf.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ark.zhongyouzk.top

[A18] 字符与 ASCII 码互转
来源：http://dav.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://ygc.uphjek.com

PHP:  ord("A"); chr(65)
来源：http://oxd.haohaochexian.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zup.jiagoushi.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://spe.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://pgm.tanke756.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://prs.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://zbq.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://fxs.zdqjudy.top

[A19] 交换两个变量
来源：http://gal.aizwys.cn

Py:   a, b = b, a
来源：http://cvh.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://rek.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://skt.fzhhl.top

TS:   [a, b] = [b, a];
来源：http://qsn.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://xhj.gzhubu.top

Go:   a, b = b, a
来源：http://wzf.sweek.top

Ruby: a, b = b, a
来源：http://iqs.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://mzi.zdbjq.cn

[A20] 读取标准输入
来源：http://huv.andypj.xyz

Py:   name = input("请输入：")
来源：http://waq.daria6918.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jfn.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bzc.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://sdu.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://ybe.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sxm.c1oappe.top

Ruby: gets.chomp
来源：http://zcs.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://ufz.tian-w.cn

[A21] 保留指定小数位输出
来源：http://puc.uphjek.com

Py:   f"{3.14159:.2f}"
来源：http://hks.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kjn.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://tba.hammf.cn

TS:   (3.14159).toFixed(2)
来源：http://irh.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://nqx.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kji.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://rkh.fengsongda.top

C#:   3.14159.ToString("F2")
来源：http://acq.cashguo.top

[A22] 获取字符串长度
来源：http://ffo.iojbl.cn

Py:   len(s)
来源：http://qzb.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nlb.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://epn.zhoulong.xyz

TS:   s.length
来源：http://ohi.jqgfzy.top

Java: s.length()
来源：http://laq.hnxiangtu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mto.cdnleiting.top

Ruby: s.length
来源：http://nml.ybcxt.top

C#:   s.Length
来源：http://tfg.nwbrower.top

[A23] 大小写转换
来源：http://vqw.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://amn.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://unl.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dmp.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wpy.yj20258888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ode.sxryk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ile.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zvk.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gja.cdnleiting.top

[A24] 去除首尾空白
来源：http://amy.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vkq.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ytq.ppjwa.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://efj.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ddo.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://otr.zycfv.cn

Go:   strings.TrimSpace(s)
来源：http://xzd.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hpe.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ska.sjlbkw.cn

[A25] 字符串比较
来源：http://pqt.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://pva.ydjk.org.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://djx.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://akt.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xpn.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sjb.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rip.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nbr.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oqp.yuanzhike.top

[A26] 类型转换总览
来源：http://dvw.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yuq.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mhj.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hut.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://cju.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ufl.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vwz.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nwt.snrcjt.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ipu.ybcxt.top

================================================================================
来源：http://eje.jqgufenzy.top

B. 流程控制
来源：http://sgw.gzhubu.top

================================================================================
来源：http://rdx.mhx1999.top

[B01] 条件判断 if / else
来源：http://ilr.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mbd.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nid.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bbb.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fzg.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://azk.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bgl.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://byt.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kzj.xylfe.cn

[B02] 多分支 else if / elif
来源：http://iiu.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nfo.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gla.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sim.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlh.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udf.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uke.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vvx.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://stv.chenzaomai.com

[B03] switch / match / case
来源：http://ryf.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hmz.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://upy.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kec.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://otk.bjfxy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yid.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zks.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vqq.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dpv.jianghu66.top

[B04] for 计数循环
来源：http://zzw.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://nau.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dog.yanxiufei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izb.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vxm.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mij.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rxq.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://tpq.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://exb.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://fna.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://boo.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wqt.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mye.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://hki.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kfl.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://amh.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://oug.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uik.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://tnx.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ujc.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bby.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mbg.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zkp.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uxi.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lnx.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zyo.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dbj.xziqi.cn

[B07] while 循环
来源：http://jrl.tarul.cn

Py:   while i < 10: i += 1
来源：http://lsr.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yly.mhx1999.top

JS:   while (i < 10) { i++; }
来源：http://rde.sweek.top

TS:   while (i < 10) { i++; }
来源：http://duk.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://bwj.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rjf.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://hmu.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://muf.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://lxa.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://wig.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xzl.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://jed.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://kxs.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://njq.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lwq.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dwp.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://hbv.52xcode.cn

[B09] break 与 continue
来源：http://epy.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kxg.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ulx.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tyq.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ruq.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rcc.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hop.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://skv.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hoh.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://wrl.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cob.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cxa.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dcb.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lzj.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oyy.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vvt.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cge.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hqe.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://idk.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://kqv.xylfe.cn


<!-- 参考信息 -->