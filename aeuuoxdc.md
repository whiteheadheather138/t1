代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dif.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aqw.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://tju.jinqigufen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wdr.nanxinkj.top

Go:   reflect.TypeOf(x).Name()
来源：http://fpy.52xcode.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iqj.tian-w.cn

C#:   x.GetType().Name; x is int
来源：http://vvn.shzxlz.cn

[A05] 整数除法与取模
来源：http://qqf.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://odu.xziqi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://njn.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ugw.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hqy.meibo888.top

Java: 7 / 2; 7 % 2
来源：http://ixf.zdbjq.cn

Go:   7 / 2; 7 % 2
来源：http://aev.zhengqikj.top

Ruby: 7 / 2; 7 % 2
来源：http://dcp.jinqigfzy.top

C#:   7 / 2; 7 % 2
来源：http://bdd.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://hps.pycfn.com

Py:   int("42"); float("3.14")
来源：http://cjz.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://owe.guannengcc.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fjq.yuanzhike.top

TS:   parseInt("42", 10); Number("42")
来源：http://znj.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dth.hongshengwenyu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sqx.sxryk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xiy.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://egc.tanke756.top

[A07] 数字转字符串
来源：http://ulg.havefunace.top

Py:   str(42)
来源：http://wfs.zhiwuduotai.top

PHP:  (string) 42; strval(42)
来源：http://kvu.ctjpmb.com

JS:   String(42); (42).toString()
来源：http://ykc.tian-w.cn

TS:   String(42)
来源：http://xkl.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://aam.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://uvt.fengsongda.top

Ruby: 42.to_s
来源：http://rur.dianchejie.cn

C#:   42.ToString()
来源：http://ayx.ctjpmb.com

[A08] 取整与四舍五入
来源：http://lab.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ccj.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dts.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://atp.kuanghao11.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jsv.hysaishi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lyz.ydjk.org.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://psp.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://snr.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qic.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://tjt.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://evt.zhoulong.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hwx.epnwcf.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gon.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rkc.yuanzhike.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kdx.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dgn.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qea.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zzf.52xcode.cn

[A10] 生成随机数
来源：http://pyb.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://uom.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://wil.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yrl.smart0.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://grb.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://qlp.fanxiaobao.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cjc.nwbrower.top

Ruby: rand(1..100)
来源：http://gra.cashguo.top

C#:   new Random().Next(1, 101)
来源：http://vkt.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://vsc.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://rlr.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://iqt.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://zdm.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vwl.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://tuo.xuanzx.com

Go:   // 无三元运算符，需用 if 语句
来源：http://mdk.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://llt.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://xgc.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://dsp.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dvy.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xas.yj20258888.top

JS:   `Hello, ${name}!`
来源：http://zfz.jinqigufen.top

TS:   `Hello, ${name}!`
来源：http://lla.aizwys.cn

Java: "Hello, %s!".formatted(name)
来源：http://hzj.ydzc1.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://shg.gotoacloud.top

Ruby: "Hello, #{name}!"
来源：http://nzw.hammf.cn

C#:   $"Hello, {name}!"
来源：http://daq.xuanzx.com

[A13] 多行字符串（练习 \n 转义）
来源：http://bau.sjlbkw.cn

Py:   "第一行\n第二行"
来源：http://jjv.cashguo.top

PHP:  "第一行\n第二行"
来源：http://jko.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://nvl.xinyue.icu

TS:   "第一行\n第二行"
来源：http://pkq.cashguo.top

Java: "第一行\n第二行"
来源：http://peh.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://vnm.daria6918.cn

Ruby: "第一行\n第二行"
来源：http://xte.zhongyouzk.top

C#:   "第一行\n第二行"
来源：http://aoz.xinyue.icu

[A14] 注释写法
来源：http://lpl.9152youxi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mgv.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://dxp.andypj.xyz

JS:   // 单行；/* 多行 */
来源：http://odx.ydjk.org.cn

TS:   // 单行；/* 多行 */
来源：http://ray.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jfx.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://huh.cqqwz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bhz.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://jfx.cqqwz.cn

[A15] 空值判断与默认值
来源：http://mxc.ybcxt.top

Py:   value = data or "默认值"
来源：http://gcy.cucudq.cn

PHP:  $value = $data ?? "默认值";
来源：http://kej.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://fla.fzhhl.top

TS:   const value = data ?? "默认值";
来源：http://vgi.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oky.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://agc.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://apz.aizwys.cn

C#:   var value = data ?? "默认值";
来源：http://zzq.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://mss.shzxlz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jav.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mfr.uphjek.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mly.cheryme.top

TS:   if (!x) {}
来源：http://wmi.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qxp.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zmw.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gmz.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ibu.svipenyu.cn

[A17] 位运算
来源：http://xxp.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tze.andypj.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://msa.zhongyouzk.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ztw.gzhubu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vdy.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxg.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sux.kuanghao11.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhl.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uon.jqgufenzy.top

[A18] 字符与 ASCII 码互转
来源：http://qmc.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://pnv.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://muu.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ftf.gaohongyu789.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oer.hywenlv.cn

Java: (int) 'A'; (char) 65
来源：http://rgj.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://get.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://nly.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://ilr.meibo888.top

[A19] 交换两个变量
来源：http://yll.meibo888.top

Py:   a, b = b, a
来源：http://srk.xingfuxueyuan.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://vui.yanxiufei.cn

JS:   [a, b] = [b, a];
来源：http://gwv.sweek.top

TS:   [a, b] = [b, a];
来源：http://wqo.shuidangran.top

Java: int t = a; a = b; b = t;
来源：http://dwq.gotoacloud.top

Go:   a, b = b, a
来源：http://ymc.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://lxt.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://hbj.hongshengwenyu.top

[A20] 读取标准输入
来源：http://nww.shzxlz.cn

Py:   name = input("请输入：")
来源：http://mlz.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bhc.yanxiufei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ovh.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://kwe.jinqigfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://bwz.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://crn.havefunace.top

Ruby: gets.chomp
来源：http://bka.0kj1m.cn

C#:   Console.ReadLine();
来源：http://gaz.zhongyouzk.top

[A21] 保留指定小数位输出
来源：http://gwq.0kj1m.cn

Py:   f"{3.14159:.2f}"
来源：http://jtu.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hqy.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://anv.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://xfa.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://qve.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ogv.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://dnn.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://opt.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://btm.316326.xyz

Py:   len(s)
来源：http://lwx.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nyl.vqdsnc.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nnj.yvedp.cn

TS:   s.length
来源：http://fyd.yuxming.cn

Java: s.length()
来源：http://uep.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://agf.daxiang520.top

Ruby: s.length
来源：http://fom.xingfuxueyuan.xyz

C#:   s.Length
来源：http://zsc.zdbjq.cn

[A23] 大小写转换
来源：http://akf.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lnh.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zvr.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nxy.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ejc.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ial.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://snm.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wex.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ndd.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://smt.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pue.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cvh.ydjk.org.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hdi.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ywb.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ims.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://dht.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ths.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zbv.kuanghao11.cn

[A25] 字符串比较
来源：http://cyj.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://fsf.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lou.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jew.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qbs.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ryw.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tgu.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://awy.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://utv.hnqzz.top

[A26] 类型转换总览
来源：http://ild.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kdz.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zoc.kuanghao11.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cyb.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://tpe.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pru.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://voc.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://wol.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cjf.zdbjq.cn

================================================================================
来源：http://tmb.hnqzz.top

B. 流程控制
来源：http://rcp.gotoacloud.top

================================================================================
来源：http://gjf.epnwcf.com

[B01] 条件判断 if / else
来源：http://zut.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fnw.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jur.xinyue.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bws.hywenlv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pmb.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wzt.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://upw.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fyl.yueranfly.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qll.sxryk.cn

[B02] 多分支 else if / elif
来源：http://hoj.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nqt.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zxm.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://orw.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wen.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nnu.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aqa.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tbq.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fun.pycfn.com

[B03] switch / match / case
来源：http://muo.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ulx.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ydz.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uqz.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uum.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tdc.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dfw.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vei.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hrs.hfpthk.cn

[B04] for 计数循环
来源：http://ixq.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://nzj.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kqb.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qmw.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yuu.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://emw.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vmb.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://mti.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://idf.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://ury.pycfn.com

Py:   for item in arr: print(item)
来源：http://mqg.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://auw.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tgz.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uia.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://poi.redwolf501.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dpu.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://olc.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://azl.hcnkem.com

[B06] 遍历字典 / 对象
来源：http://sqy.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tuf.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zkc.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lav.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pwu.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://szt.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://goy.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dtl.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pqt.cheryme.top

[B07] while 循环
来源：http://zly.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://lrq.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ahq.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://xna.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://iei.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://deq.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jqd.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://doi.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://csy.316326.xyz

[B08] do-while（至少执行一次）
来源：http://fnp.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://zyf.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gyb.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://hea.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://mvw.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://knu.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://agp.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://iqt.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://egh.nwbrower.top

[B09] break 与 continue
来源：http://zbu.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dnp.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dwa.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://huv.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbd.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxh.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://evh.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ajl.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqs.yj202588.top

[B10] 遍历同时拿索引
来源：http://nke.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pzq.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sgd.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://clw.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jfw.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://awt.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dfw.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ynz.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fgv.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://zhm.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://twf.aizwys.cn


<!-- 参考信息 -->