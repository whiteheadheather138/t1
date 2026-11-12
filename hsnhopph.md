代发 wailian999

Ruby: PI = 3.14159
来源：http://lvi.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://bhm.jianghu66.top

[A04] 判断变量类型
来源：http://tzr.jinqigufen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mbq.yj20258888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dzr.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wgf.uphjek.com

TS:   typeof x; x instanceof Date
来源：http://yav.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://usc.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://yoq.52xcode.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fmv.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://ifo.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://ovi.yuanzhike.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rqy.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gir.shangyingyoupin.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vmn.jianghu66.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wrt.aibaodan.cn

Java: 7 / 2; 7 % 2
来源：http://dkt.yfazqb.com

Go:   7 / 2; 7 % 2
来源：http://pwn.hammf.cn

Ruby: 7 / 2; 7 % 2
来源：http://vty.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://kcl.dianchejie.cn

[A06] 字符串转数字
来源：http://agx.daria6918.cn

Py:   int("42"); float("3.14")
来源：http://gem.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://acu.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bpu.yfazqb.com

TS:   parseInt("42", 10); Number("42")
来源：http://nui.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hdq.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bsb.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fgy.shanyushiyangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bae.hfpthk.cn

[A07] 数字转字符串
来源：http://aft.gogol.net.cn

Py:   str(42)
来源：http://mgk.sweek.top

PHP:  (string) 42; strval(42)
来源：http://jqk.yonumen.top

JS:   String(42); (42).toString()
来源：http://bpf.guannengcc.top

TS:   String(42)
来源：http://ebe.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tzn.316326.xyz

Go:   strconv.Itoa(42)
来源：http://ovl.hysaishi.cn

Ruby: 42.to_s
来源：http://uae.sweek.top

C#:   42.ToString()
来源：http://gdi.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://pot.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ydl.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lst.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bpv.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://syt.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dec.316326.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ixz.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://idi.jinyuanbaomall.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hel.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://anj.cashguo.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eqd.haohaochexian.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hxn.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sde.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kdj.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pfv.shanyushiyangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ivz.fanxiaobao.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hzw.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://doh.gogol.net.cn

[A10] 生成随机数
来源：http://iul.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://agt.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://trm.cucudq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://juf.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://npg.ivvv.top

Java: new Random().nextInt(100) + 1
来源：http://tlf.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rul.andypj.xyz

Ruby: rand(1..100)
来源：http://lni.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://bsb.yfazqb.com

[A11] 条件表达式（三元）
来源：http://acv.zdqjudy.top

Py:   "yes" if x > 0 else "no"
来源：http://cjd.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tex.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://hle.iojbl.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vkb.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://dys.kuanghao11.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fhx.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://htq.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://vzm.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://hxf.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hug.hongshengwenyu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://azd.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://tlo.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://rfx.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://cvl.fengsongda.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fvr.tian-w.cn

Ruby: "Hello, #{name}!"
来源：http://ine.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://fba.yonumen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dre.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://knt.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://ltw.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://foh.zdqjudy.top

TS:   "第一行\n第二行"
来源：http://zzj.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://spm.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://wjd.birdmap.top

Ruby: "第一行\n第二行"
来源：http://nrp.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://pil.wangdashe.top

[A14] 注释写法
来源：http://ola.jlsjyb.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fwt.iojbl.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jes.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://gob.fzhhl.top

TS:   // 单行；/* 多行 */
来源：http://ecy.pycfn.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://com.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://hjt.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fij.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://oee.wangdashe.top

[A15] 空值判断与默认值
来源：http://qhc.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://lzf.chenlongwang.top

PHP:  $value = $data ?? "默认值";
来源：http://viq.shanyushiyangtech.top

JS:   const value = data ?? "默认值";
来源：http://ray.c1oappe.top

TS:   const value = data ?? "默认值";
来源：http://vfy.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dib.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://fbs.andypj.xyz

Ruby: value = data || "默认值"
来源：http://vbg.hfpthk.cn

C#:   var value = data ?? "默认值";
来源：http://kqj.tianlin.xyz

[A16] 真假值判断规则
来源：http://add.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://roe.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://clc.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://elw.hywenlv.cn

TS:   if (!x) {}
来源：http://nop.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gby.yonumen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yea.ivvv.top

Ruby: unless x            # nil 与 false 为假
来源：http://vlt.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dsk.316326.xyz

[A17] 位运算
来源：http://tqu.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wkx.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dyw.yfazqb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pmj.sufxvd.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xpd.xingfuxueyuan.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pua.chenjidiqi.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iog.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hkk.nanxinkj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rpr.jinyuanbaomall.cn

[A18] 字符与 ASCII 码互转
来源：http://dnj.gaohongyu789.top

Py:   ord("A"); chr(65)
来源：http://gsn.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://pus.aizwys.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xcg.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uji.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://jfh.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kod.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://ncb.birdmap.top

C#:   (int)'A'; (char)65
来源：http://azj.chenzaomai.com

[A19] 交换两个变量
来源：http://rqq.shuidangran.top

Py:   a, b = b, a
来源：http://nda.dianchejie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://daq.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://ciw.shangyingyoupin.top

TS:   [a, b] = [b, a];
来源：http://qmd.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://ywz.wangshuangyany.cn

Go:   a, b = b, a
来源：http://uio.hongshengwenyu.top

Ruby: a, b = b, a
来源：http://vqv.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://apu.hongshengwenyu.top

[A20] 读取标准输入
来源：http://odw.ctjpmb.com

Py:   name = input("请输入：")
来源：http://wkt.jyoumei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gxo.fehbvm.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ecf.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://iwj.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://ijp.sweek.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sfw.aizwys.cn

Ruby: gets.chomp
来源：http://hsm.gzhubu.top

C#:   Console.ReadLine();
来源：http://wlt.daria6918.cn

[A21] 保留指定小数位输出
来源：http://yhr.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://wkf.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sbz.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://trv.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://yvg.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://djp.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ufn.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://hkc.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://ezb.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://elx.gogol.net.cn

Py:   len(s)
来源：http://qqk.xylfe.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zrv.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nsp.zhengqikj.top

TS:   s.length
来源：http://ilg.chenlongwang.top

Java: s.length()
来源：http://jgi.bbcook.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kjc.zdqjudy.top

Ruby: s.length
来源：http://thc.jiagoushi.top

C#:   s.Length
来源：http://yau.jinghuilouyu.cn

[A23] 大小写转换
来源：http://fuq.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ekd.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qkl.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eww.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://btv.zhoulong.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qju.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nic.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lxc.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://smk.fzhhl.top

[A24] 去除首尾空白
来源：http://ddh.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hex.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qfb.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uln.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tld.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gtm.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://dow.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kty.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nbz.hcnkem.com

[A25] 字符串比较
来源：http://jld.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://ohd.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bxv.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://awg.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uaj.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wfa.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gxk.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nzp.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zpq.havefunace.top

[A26] 类型转换总览
来源：http://ens.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xwm.yfazqb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uzz.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://til.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://riy.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wgo.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://irk.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kdb.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gvv.zhongyouzk.top

================================================================================
来源：http://fmt.nanxinkj.top

B. 流程控制
来源：http://spz.birdmap.top

================================================================================
来源：http://mid.xuanzx.com

[B01] 条件判断 if / else
来源：http://alk.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hpv.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jla.9152youxi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://izk.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ebo.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://apg.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kzl.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://edd.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ift.yuxming.cn

[B02] 多分支 else if / elif
来源：http://kss.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://svl.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dlb.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fro.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ght.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhf.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://poq.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bdu.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ves.fanxiaobao.xyz

[B03] switch / match / case
来源：http://ozj.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aqm.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vmv.gotoacloud.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://enu.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxn.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tnm.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nfa.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uyv.dashuyun.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cjw.aibaodan.cn

[B04] for 计数循环
来源：http://aan.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://mvc.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mji.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pod.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zip.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lke.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mcy.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://vrk.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pha.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://owk.havefunace.top

Py:   for item in arr: print(item)
来源：http://blv.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cmq.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tho.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wgl.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tld.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://owm.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://bgi.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xkt.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://sen.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hlj.xziqi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zxj.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nrd.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rck.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jkv.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dct.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xqw.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uhs.hammf.cn

[B07] while 循环
来源：http://qgo.tian-w.cn

Py:   while i < 10: i += 1
来源：http://oys.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://ois.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://ify.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://xkt.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://diy.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ffs.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://bzm.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://lnv.ivvv.top

[B08] do-while（至少执行一次）
来源：http://umi.zdbjq.cn

Py:   # 无 do-while：用 while True + break
来源：http://rij.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vnr.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://pqm.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://kqf.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://mbj.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nce.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lpk.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://zhy.quarkkingdee.top

[B09] break 与 continue
来源：http://mne.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zgp.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://emf.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imw.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfh.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vtx.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rcw.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uaf.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrp.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://hqw.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ntp.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://udq.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pqd.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kyt.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ydv.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ppd.yangfankeji.com


<!-- 参考信息 -->