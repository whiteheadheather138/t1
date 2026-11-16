代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ykq.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://clk.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://gyl.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vxk.cdnleiting.top

Go:   reflect.TypeOf(x).Name()
来源：http://osj.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://vfa.yvedp.cn

C#:   x.GetType().Name; x is int
来源：http://lvz.tianlin.xyz

[A05] 整数除法与取模
来源：http://scm.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ffn.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://mqj.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iqa.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ymv.yvedp.cn

Java: 7 / 2; 7 % 2
来源：http://nsl.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://pys.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://npq.hammf.cn

C#:   7 / 2; 7 % 2
来源：http://hpy.snrcjt.cn

[A06] 字符串转数字
来源：http://kjn.shuidangran.top

Py:   int("42"); float("3.14")
来源：http://ptv.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sgp.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rro.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://zjm.fktsv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mpx.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://idx.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xku.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://khb.chenlongwang.top

[A07] 数字转字符串
来源：http://mwz.hesvh.cn

Py:   str(42)
来源：http://ddo.xuanzx.com

PHP:  (string) 42; strval(42)
来源：http://cje.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://zlz.yj20258888.top

TS:   String(42)
来源：http://gul.jinghuilouyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://odp.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://iew.zhengqikj.top

Ruby: 42.to_s
来源：http://kvm.nwbrower.top

C#:   42.ToString()
来源：http://rsr.yvedp.cn

[A08] 取整与四舍五入
来源：http://jro.pycfn.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ahb.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://egp.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tec.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tge.bjfxy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qxx.cdnleiting.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vpf.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jpk.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://srv.birdmap.top

[A09] 绝对值与最大最小值
来源：http://xxl.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ohf.316326.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ilo.jyoumei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ljk.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mga.chenzaomai.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mnw.xylfe.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hog.jqgufenzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wws.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vvl.yuanzhike.top

[A10] 生成随机数
来源：http://xpk.snrcjt.cn

Py:   import random; random.randint(1, 100)
来源：http://zjb.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://pba.tianlin.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fnu.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://utv.yangfankeji.com

Java: new Random().nextInt(100) + 1
来源：http://ryt.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zsw.9152youxi.cn

Ruby: rand(1..100)
来源：http://zkk.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://snh.gogol.net.cn

[A11] 条件表达式（三元）
来源：http://sao.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://yxz.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://agg.uphjek.com

JS:   x > 0 ? "yes" : "no"
来源：http://anr.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pkm.yangfankeji.com

Java: x > 0 ? "yes" : "no"
来源：http://pnh.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zxx.9152youxi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yje.dianchejie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://asd.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://pog.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jyw.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://voa.quarkkingdee.top

JS:   `Hello, ${name}!`
来源：http://lki.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://gcl.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://uua.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oip.wangshuangyany.cn

Ruby: "Hello, #{name}!"
来源：http://akr.316326.xyz

C#:   $"Hello, {name}!"
来源：http://wfk.vehdjk.com

[A13] 多行字符串（练习 \n 转义）
来源：http://zkb.yj202588.top

Py:   "第一行\n第二行"
来源：http://ufe.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://duo.jinghuilouyu.cn

JS:   "第一行\n第二行"
来源：http://hgc.yonumen.top

TS:   "第一行\n第二行"
来源：http://bje.hfpthk.cn

Java: "第一行\n第二行"
来源：http://wvv.cdnleiting.top

Go:   "第一行\n第二行"
来源：http://irn.hammf.cn

Ruby: "第一行\n第二行"
来源：http://xvh.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://eoo.jinyuanbaomall.cn

[A14] 注释写法
来源：http://tdu.daxiang520.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ofr.redwolf501.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rxv.haohaochexian.top

JS:   // 单行；/* 多行 */
来源：http://vga.snrcjt.cn

TS:   // 单行；/* 多行 */
来源：http://and.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mxn.tian-w.cn

Go:   // 单行；/* 多行 */
来源：http://qvh.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ghg.uphjek.com

C#:   // 单行；/* 多行 */
来源：http://ftf.zycfv.cn

[A15] 空值判断与默认值
来源：http://oxg.ywan-chungtsiang.top

Py:   value = data or "默认值"
来源：http://ipn.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://ndk.jianghu66.top

JS:   const value = data ?? "默认值";
来源：http://hlz.smart0.xyz

TS:   const value = data ?? "默认值";
来源：http://tpx.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lzq.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://vzp.hnqzz.top

Ruby: value = data || "默认值"
来源：http://zye.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://sxo.tianlin.xyz

[A16] 真假值判断规则
来源：http://rvd.shuidangran.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://etr.hcnkem.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yth.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://scp.bbcook.cn

TS:   if (!x) {}
来源：http://gqi.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fyc.pengpengdd.cyou

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nam.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://lfs.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ajf.gogol.net.cn

[A17] 位运算
来源：http://urz.yj202588.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://was.ehwqpu.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qwb.zhixingplan.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jyj.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://soi.mhx1999.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iry.sxryk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jzd.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smy.zhoulong.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwr.jyoumei.cn

[A18] 字符与 ASCII 码互转
来源：http://xkl.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://pgk.dianchejie.cn

PHP:  ord("A"); chr(65)
来源：http://isv.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ckg.yuxming.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yww.snrcjt.cn

Java: (int) 'A'; (char) 65
来源：http://jbj.guowangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xno.shzxlz.cn

Ruby: "A".ord; 65.chr
来源：http://fbl.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://evs.tarul.cn

[A19] 交换两个变量
来源：http://ljs.ywan-chungtsiang.top

Py:   a, b = b, a
来源：http://yak.guowangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hcx.mhx1999.top

JS:   [a, b] = [b, a];
来源：http://lhi.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://klo.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://hmy.haohaochexian.top

Go:   a, b = b, a
来源：http://gng.316326.xyz

Ruby: a, b = b, a
来源：http://tes.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://uxu.yueranfly.top

[A20] 读取标准输入
来源：http://vop.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://dlk.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://vhd.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mmt.52xcode.cn

TS:   // Node.js：readline 模块
来源：http://txy.hywenlv.cn

Java: new Scanner(System.in).nextLine()
来源：http://taq.haohaochexian.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xkg.zdbjq.cn

Ruby: gets.chomp
来源：http://vmk.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://xcj.hammf.cn

[A21] 保留指定小数位输出
来源：http://pkw.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://tgd.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://naj.316326.xyz

JS:   (3.14159).toFixed(2)
来源：http://rdh.9152youxi.cn

TS:   (3.14159).toFixed(2)
来源：http://rng.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://qvz.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lur.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://nfu.zdqjudy.top

C#:   3.14159.ToString("F2")
来源：http://npq.jinghuilouyu.cn

[A22] 获取字符串长度
来源：http://jlo.ybcxt.top

Py:   len(s)
来源：http://dne.pengpengdd.cyou

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ynr.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://svf.cucudq.cn

TS:   s.length
来源：http://eoc.xylfe.cn

Java: s.length()
来源：http://zgy.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hhl.aizwys.cn

Ruby: s.length
来源：http://ktt.andypj.xyz

C#:   s.Length
来源：http://myb.hysaishi.cn

[A23] 大小写转换
来源：http://iun.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xwr.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mtz.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pou.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tzv.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hqr.hywenlv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jsk.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gcj.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dql.vqdsnc.cn

[A24] 去除首尾空白
来源：http://bzj.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hwy.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mbi.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sqg.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://twc.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://whk.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://nkr.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sjp.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ijh.jiagoushi.top

[A25] 字符串比较
来源：http://apb.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://xxg.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zzk.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tqw.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yvt.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aka.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://utg.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mpp.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kiq.jianghu66.top

[A26] 类型转换总览
来源：http://nnm.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ggd.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nzb.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xyn.hesvh.cn

TS:   Number() String() Boolean() x as number
来源：http://xne.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hlx.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://amd.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://bgw.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nco.zhongyouzk.top

================================================================================
来源：http://wif.yonumen.top

B. 流程控制
来源：http://tvp.jianghu66.top

================================================================================
来源：http://nfn.snrcjt.cn

[B01] 条件判断 if / else
来源：http://bgp.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://taz.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lws.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://boo.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://axy.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://won.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uej.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mro.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://krx.fzhhl.top

[B02] 多分支 else if / elif
来源：http://him.yonumen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://luy.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lpf.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vlp.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tmv.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecx.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yvr.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fqb.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vrt.shanyushiyangtech.top

[B03] switch / match / case
来源：http://obe.chenzaomai.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uvp.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bre.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jnq.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sjv.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://efe.316326.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://knq.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tqd.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xbb.fzhhl.top

[B04] for 计数循环
来源：http://fdc.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://kik.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://srx.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://val.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://upy.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ynl.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://asp.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://roi.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ajm.bbcook.cn

[B05] 遍历数组 / 列表
来源：http://wcy.sysykeji.top

Py:   for item in arr: print(item)
来源：http://aeo.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fay.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://asg.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qpz.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rvl.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tna.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://jov.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eit.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://lqq.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kia.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rbv.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uad.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jhy.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://utw.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bde.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yht.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ano.xuetiantiany.cn

[B07] while 循环
来源：http://gyz.aizwys.cn

Py:   while i < 10: i += 1
来源：http://vyu.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://hes.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://nst.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://gpb.ivvv.top

Java: while (i < 10) { i++; }
来源：http://mxw.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vuk.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://pol.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://cbv.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://tms.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://hqz.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yze.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://nvy.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://iyd.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://uux.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xup.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://nfz.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://ffz.hesvh.cn

[B09] break 与 continue
来源：http://gab.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yzi.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cdr.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmr.yangfankeji.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://csh.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgm.dianchejie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mgi.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wsl.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eiq.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://vvs.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kxa.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ayv.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wou.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qfa.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://guu.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ffz.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lvd.cashguo.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fiw.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://fdi.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://bep.ivvv.top


<!-- 参考信息 -->