代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://efi.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gpl.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://urd.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xec.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://xkz.cdnleiting.top

Ruby: x.class; x.is_a?(Integer)
来源：http://apg.nwbrower.top

C#:   x.GetType().Name; x is int
来源：http://fjc.shanyushiyangkeji.top

[A05] 整数除法与取模
来源：http://oht.zhoulong.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nqw.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://djz.pycfn.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ytw.tianlin.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uag.hfpthk.cn

Java: 7 / 2; 7 % 2
来源：http://ari.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://nqe.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://kos.jiagoushi.top

C#:   7 / 2; 7 % 2
来源：http://zrn.feifeiyinyue.top

[A06] 字符串转数字
来源：http://gyx.jianghu66.top

Py:   int("42"); float("3.14")
来源：http://ain.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tqa.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cus.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ffe.ppjwa.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://scv.cucudq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pvj.jyoumei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ujm.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hry.jinqigufen.top

[A07] 数字转字符串
来源：http://qjy.zhaomingkeji.xyz

Py:   str(42)
来源：http://tas.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://xnn.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://qbd.sjlbkw.cn

TS:   String(42)
来源：http://jog.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lvn.jinqigufen.top

Go:   strconv.Itoa(42)
来源：http://raf.hongshengwenyu.top

Ruby: 42.to_s
来源：http://sda.gaohongyu789.top

C#:   42.ToString()
来源：http://ulg.sweek.top

[A08] 取整与四舍五入
来源：http://xvy.hfpthk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tzr.cashguo.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://brj.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vxz.pycfn.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://znw.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kqo.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jgc.jinqigufen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://omm.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rkx.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://euo.jinqigfzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gym.wangshuangyany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ipz.xuanzx.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://klh.iojbl.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wdj.nwbrower.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fnc.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mns.chenjidiqi.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nyh.tarul.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dbs.zdbjq.cn

[A10] 生成随机数
来源：http://crl.redwolf501.top

Py:   import random; random.randint(1, 100)
来源：http://pwp.tarul.cn

PHP:  random_int(1, 100);
来源：http://sda.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mvq.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uno.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://kag.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vgx.svipenyu.cn

Ruby: rand(1..100)
来源：http://iqu.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://ugz.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://onq.cucudq.cn

Py:   "yes" if x > 0 else "no"
来源：http://jmi.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zlt.epnwcf.com

JS:   x > 0 ? "yes" : "no"
来源：http://lvr.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mni.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://qgm.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://upy.yanxiufei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wtw.hesvh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gak.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://vst.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mdf.chenlongwang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://suw.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://jtr.gotoacloud.top

TS:   `Hello, ${name}!`
来源：http://uqf.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://kqc.jiagoushi.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sxp.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://gar.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://tpa.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ahf.dianchejie.cn

Py:   "第一行\n第二行"
来源：http://gcy.yongpay.top

PHP:  "第一行\n第二行"
来源：http://ftp.cashguo.top

JS:   "第一行\n第二行"
来源：http://tik.zycfv.cn

TS:   "第一行\n第二行"
来源：http://zid.zhaomingkeji.xyz

Java: "第一行\n第二行"
来源：http://dhf.fengsongda.top

Go:   "第一行\n第二行"
来源：http://ifz.hcnkem.com

Ruby: "第一行\n第二行"
来源：http://mwi.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://kaq.cheryme.top

[A14] 注释写法
来源：http://fvy.aizwys.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bgr.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kgt.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://xbz.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://hao.shanyushiyangtech.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bjh.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://hpf.ywan-chungtsiang.top

Ruby: # 单行；=begin 多行 =end
来源：http://rmw.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://xcn.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://utd.shzxlz.cn

Py:   value = data or "默认值"
来源：http://uma.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://keh.iojbl.cn

JS:   const value = data ?? "默认值";
来源：http://cwl.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://cpb.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://usm.yangfankeji.com

Go:   if data == "" { data = "默认值" }
来源：http://qbx.gzhubu.top

Ruby: value = data || "默认值"
来源：http://qts.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://qpf.jqgfzy.top

[A16] 真假值判断规则
来源：http://nmg.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vkr.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rjn.xinyue.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ufh.wangshuangyany.cn

TS:   if (!x) {}
来源：http://lno.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zuz.sysykeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wuy.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://pou.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ghh.cucudq.cn

[A17] 位运算
来源：http://pzn.ydzc1.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cua.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://atc.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smv.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://crc.zdbjq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ync.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://opf.hesvh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rpx.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nxp.nanxuanxn.top

[A18] 字符与 ASCII 码互转
来源：http://xof.meibo888.top

Py:   ord("A"); chr(65)
来源：http://etx.iojbl.cn

PHP:  ord("A"); chr(65)
来源：http://miw.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://czw.cdnleiting.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xay.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://wec.xingfuxueyuan.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cbd.yj202588.top

Ruby: "A".ord; 65.chr
来源：http://sek.havefunace.top

C#:   (int)'A'; (char)65
来源：http://tta.jinqigfzy.top

[A19] 交换两个变量
来源：http://its.dianchejie.cn

Py:   a, b = b, a
来源：http://dqs.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ksg.chenlongwang.top

JS:   [a, b] = [b, a];
来源：http://bfl.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://hqs.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://vzr.fktsv.cn

Go:   a, b = b, a
来源：http://kvv.ivvv.top

Ruby: a, b = b, a
来源：http://uuv.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://lpe.yuanzhike.top

[A20] 读取标准输入
来源：http://xkk.xingfuxueyuan.xyz

Py:   name = input("请输入：")
来源：http://oib.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lzr.chenjidiqi.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rbr.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://llr.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://kig.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mot.jinqigfzy.top

Ruby: gets.chomp
来源：http://lrx.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://wlb.fzhhl.top

[A21] 保留指定小数位输出
来源：http://rdg.daria6918.cn

Py:   f"{3.14159:.2f}"
来源：http://vhn.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cna.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://hbs.fehbvm.com

TS:   (3.14159).toFixed(2)
来源：http://nna.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://keg.pycfn.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fwr.shzxlz.cn

Ruby: format("%.2f", 3.14159)
来源：http://mlu.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://tgk.wangdashe.top

[A22] 获取字符串长度
来源：http://kwo.cheryme.top

Py:   len(s)
来源：http://fvb.cheryme.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://smc.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mrv.vqdsnc.cn

TS:   s.length
来源：http://kbq.pycfn.com

Java: s.length()
来源：http://ohr.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rjo.snrcjt.cn

Ruby: s.length
来源：http://odv.hfpthk.cn

C#:   s.Length
来源：http://dlt.zycfv.cn

[A23] 大小写转换
来源：http://bbe.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://szx.ppjwa.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uke.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uhc.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dxg.316326.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wiv.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dza.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ckq.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tvo.svipenyu.cn

[A24] 去除首尾空白
来源：http://whk.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aez.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://otc.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vzl.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fwe.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fjv.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://vkn.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rnr.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ytg.wangshuangyany.cn

[A25] 字符串比较
来源：http://wtm.yuanzhike.top

Py:   s1 == s2; s1 != s2
来源：http://akv.nanxinkj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jqz.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bzi.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pvs.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://giu.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dmt.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ckq.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://klb.pycfn.com

[A26] 类型转换总览
来源：http://csf.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nkw.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fln.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sde.dianchejie.cn

TS:   Number() String() Boolean() x as number
来源：http://zdb.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ttf.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gtl.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ayq.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://app.xuanzx.com

================================================================================
来源：http://npy.svipenyu.cn

B. 流程控制
来源：http://snl.shangyingyoupin.top

================================================================================
来源：http://dth.haohaochexian.top

[B01] 条件判断 if / else
来源：http://zyw.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gzn.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kyo.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zup.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zrt.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ajb.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://suz.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lga.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cbi.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://wnw.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nrh.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xlc.pycfn.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oea.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jlm.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfx.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uix.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rjb.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qfw.smart0.xyz

[B03] switch / match / case
来源：http://aaj.cheryme.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ajy.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xng.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ixj.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iam.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xvv.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kpz.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://awh.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ssr.sysykeji.top

[B04] for 计数循环
来源：http://ygo.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://ydc.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ata.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ilg.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tmr.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kim.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tjl.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://cjo.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jxc.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://gzz.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://rop.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://use.xingfuxueyuan.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://abz.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pog.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://sjk.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fdp.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://beg.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kjj.tanke756.top

[B06] 遍历字典 / 对象
来源：http://ygn.pengpengdd.cyou

Py:   for k, v in d.items(): print(k, v)
来源：http://hej.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://see.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lei.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rkq.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bbt.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mdi.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rqq.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ohn.zhongyouzk.top

[B07] while 循环
来源：http://vhc.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://cit.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://arq.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://jfh.316326.xyz

TS:   while (i < 10) { i++; }
来源：http://rkn.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://xpb.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://exz.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://cpr.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://gkm.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://rjo.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://lcs.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lqc.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://nut.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://rlj.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://ups.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xmt.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tam.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://okw.c1oappe.top

[B09] break 与 continue
来源：http://emc.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cef.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gwi.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mlr.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpf.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhh.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pwt.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gta.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzo.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://czd.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bhn.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ozn.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ykh.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ihl.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xwn.c1oappe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://weu.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gpo.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fph.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://zwq.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://dam.wangdashe.top


<!-- 参考信息 -->