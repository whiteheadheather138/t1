代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://jxk.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xxd.tian-w.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mzf.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://run.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fsc.dashuyun.cn

[A07] 数字转字符串
来源：http://twj.ppjwa.cn

Py:   str(42)
来源：http://hvw.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://vwz.wangdashe.top

JS:   String(42); (42).toString()
来源：http://pdm.zhongyouzk.top

TS:   String(42)
来源：http://qwm.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://xrj.tarul.cn

Go:   strconv.Itoa(42)
来源：http://kjc.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://nsp.ydjk.org.cn

C#:   42.ToString()
来源：http://qyw.gotoacloud.top

[A08] 取整与四舍五入
来源：http://ejj.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uoc.xinyue.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ael.dianchejie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://let.wangdashe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ezj.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cxv.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pat.shanyushiyangtech.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ogg.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xap.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://ays.chenlongwang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xon.xziqi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nym.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hkv.fehbvm.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tja.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tlj.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://huh.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uae.hammf.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nqg.9152youxi.cn

[A10] 生成随机数
来源：http://jxo.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://odt.andypj.xyz

PHP:  random_int(1, 100);
来源：http://bcd.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blv.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vor.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://xdy.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rtf.zdqjudy.top

Ruby: rand(1..100)
来源：http://npe.zhengqikj.top

C#:   new Random().Next(1, 101)
来源：http://nub.hesvh.cn

[A11] 条件表达式（三元）
来源：http://jjk.andypj.xyz

Py:   "yes" if x > 0 else "no"
来源：http://hch.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qxw.hnxiangtu.top

JS:   x > 0 ? "yes" : "no"
来源：http://fnh.yfazqb.com

TS:   x > 0 ? "yes" : "no"
来源：http://gtl.chenzaomai.com

Java: x > 0 ? "yes" : "no"
来源：http://kno.bjfxy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bfl.pengpengdd.cyou

Ruby: x > 0 ? "yes" : "no"
来源：http://uxx.ydzc1.top

C#:   x > 0 ? "yes" : "no"
来源：http://ros.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://cpq.jinqigfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oww.wangshuangyany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://evw.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://gei.hongshengwenyu.top

TS:   `Hello, ${name}!`
来源：http://bxq.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://jhi.chenzaomai.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://siu.pycfn.com

Ruby: "Hello, #{name}!"
来源：http://efs.ppjwa.cn

C#:   $"Hello, {name}!"
来源：http://tcp.yj20258.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vru.nwbrower.top

Py:   "第一行\n第二行"
来源：http://qvp.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://kll.daria6918.cn

JS:   "第一行\n第二行"
来源：http://jnw.xuanzx.com

TS:   "第一行\n第二行"
来源：http://xay.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://esx.yfazqb.com

Go:   "第一行\n第二行"
来源：http://gyi.ydjk.org.cn

Ruby: "第一行\n第二行"
来源：http://ccl.jiagoushi.top

C#:   "第一行\n第二行"
来源：http://kgs.gogol.net.cn

[A14] 注释写法
来源：http://jhj.wangdashe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wya.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ttl.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://skk.zhijiandao.cn

TS:   // 单行；/* 多行 */
来源：http://oed.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xoz.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://vxf.xinyue.icu

Ruby: # 单行；=begin 多行 =end
来源：http://xvi.chenjidiqi.icu

C#:   // 单行；/* 多行 */
来源：http://hnx.cqqwz.cn

[A15] 空值判断与默认值
来源：http://cgp.yueranfly.top

Py:   value = data or "默认值"
来源：http://hfj.sysykeji.top

PHP:  $value = $data ?? "默认值";
来源：http://mhu.ppjwa.cn

JS:   const value = data ?? "默认值";
来源：http://qgx.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://yhy.xziqi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://epr.jiagoushi.top

Go:   if data == "" { data = "默认值" }
来源：http://atr.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://kka.gzhubu.top

C#:   var value = data ?? "默认值";
来源：http://zau.yuanzhike.top

[A16] 真假值判断规则
来源：http://ywl.cheryme.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yil.pengpengdd.cyou

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zxe.yj20258.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nnb.jqgfzy.top

TS:   if (!x) {}
来源：http://vva.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nis.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nri.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://udg.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wbd.zycfv.cn

[A17] 位运算
来源：http://wqf.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jvy.shzxlz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tmr.0kj1m.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://htx.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://khg.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hpi.smart0.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zmz.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mhn.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yps.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://zpb.wangshuangyany.cn

Py:   ord("A"); chr(65)
来源：http://stv.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://jvj.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://naa.fengsongda.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yfs.bbcook.cn

Java: (int) 'A'; (char) 65
来源：http://qzm.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qli.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://ijh.jlsjyb.cn

C#:   (int)'A'; (char)65
来源：http://tyz.aibaodan.cn

[A19] 交换两个变量
来源：http://iyz.nanxuanxn.top

Py:   a, b = b, a
来源：http://eyr.pycfn.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wuj.gaohongyu789.top

JS:   [a, b] = [b, a];
来源：http://ghs.hnxiangtu.top

TS:   [a, b] = [b, a];
来源：http://zqt.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://hew.haohaochexian.top

Go:   a, b = b, a
来源：http://pfu.jqgufenzy.top

Ruby: a, b = b, a
来源：http://bhi.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://djx.zhengqikj.top

[A20] 读取标准输入
来源：http://hnj.hnqzz.top

Py:   name = input("请输入：")
来源：http://rgo.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zuq.wangshuangyany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ucf.dianchejie.cn

TS:   // Node.js：readline 模块
来源：http://ddo.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://fyi.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fvd.cdnleiting.top

Ruby: gets.chomp
来源：http://hnb.hongshengwenyu.top

C#:   Console.ReadLine();
来源：http://qib.fzhhl.top

[A21] 保留指定小数位输出
来源：http://rcm.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://npr.xinyue.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ocs.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://otp.svipenyu.cn

TS:   (3.14159).toFixed(2)
来源：http://bhh.ywan-chungtsiang.top

Java: String.format("%.2f", 3.14159)
来源：http://bmk.cashguo.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tyq.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://alf.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://qkl.shanyushiyangtech.top

[A22] 获取字符串长度
来源：http://lzl.sweek.top

Py:   len(s)
来源：http://hlp.yangfankeji.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zun.hnqzz.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rba.svipenyu.cn

TS:   s.length
来源：http://kps.smart0.xyz

Java: s.length()
来源：http://ebx.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://exf.chenzaomai.com

Ruby: s.length
来源：http://kqa.xuetiantiany.cn

C#:   s.Length
来源：http://cnc.fzhhl.top

[A23] 大小写转换
来源：http://kff.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dfe.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xwq.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mru.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ihy.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wck.feifeiyinyue.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dun.dianchejie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lyn.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bqi.ctjpmb.com

[A24] 去除首尾空白
来源：http://byc.zhixingplan.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://itm.fktsv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tib.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tqd.birdmap.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rfz.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zhr.tianlin.xyz

Go:   strings.TrimSpace(s)
来源：http://lbk.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lvj.cucudq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://brd.svipenyu.cn

[A25] 字符串比较
来源：http://sgd.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://mtf.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qfx.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vbp.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tck.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://abo.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jdw.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hbu.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pzq.birdmap.top

[A26] 类型转换总览
来源：http://lbh.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://njm.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wfu.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xqg.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://qiz.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vtc.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yks.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gzr.sufxvd.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dgf.yj20258888.top

================================================================================
来源：http://yeb.fktsv.cn

B. 流程控制
来源：http://rqv.jinqigufen.top

================================================================================
来源：http://lup.aizwys.cn

[B01] 条件判断 if / else
来源：http://nzp.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://wtr.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yrk.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sui.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iku.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bdk.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yhy.redwolf501.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mbj.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aro.yongpay.top

[B02] 多分支 else if / elif
来源：http://mvg.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://esy.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ftj.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vqa.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jlk.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvx.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rtt.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rhs.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyr.pengpengdd.cyou

[B03] switch / match / case
来源：http://nag.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bdr.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fvu.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vfh.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yxb.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zuv.cucudq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ijm.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kvi.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wyi.chenzaomai.com

[B04] for 计数循环
来源：http://jng.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://seq.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cax.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sba.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://smd.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://khd.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jtc.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://wet.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vgj.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://mue.fengsongda.top

Py:   for item in arr: print(item)
来源：http://esq.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rck.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fey.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mrk.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ujj.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://njv.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://abh.andypj.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sun.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://yvn.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qkv.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tlm.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cqv.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sez.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xio.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ijm.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uyi.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://thc.tarul.cn

[B07] while 循环
来源：http://afs.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://rqn.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xvg.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://knm.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://ohs.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://axo.sufxvd.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://twg.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://gey.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://emc.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://rjv.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://lgm.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://oxm.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://xja.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://lom.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://jqo.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://pxy.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://zvq.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://pbx.ppjwa.cn

[B09] break 与 continue
来源：http://vwg.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pmq.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uwp.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovy.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smb.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zif.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bkh.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wpi.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zof.fktsv.cn

[B10] 遍历同时拿索引
来源：http://fcm.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bjc.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://alf.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vpu.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sma.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hpt.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://axr.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tri.shzxlz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mzh.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://wpw.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://dir.yvedp.cn

PHP:  range(0, 10, 2);
来源：http://dfd.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezn.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://apd.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aei.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wyz.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://opt.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lwz.zycfv.cn

[B12] 跳出多层循环
来源：http://ead.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pkx.aibaodan.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jhx.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sgx.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://alj.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tsb.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jen.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jgp.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nko.nanxuanxn.top

[B13] 判断是否为数字
来源：http://rvi.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://vlc.yuxming.cn

PHP:  is_numeric($x)
来源：http://zsc.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xmf.epnwcf.com


<!-- 参考信息 -->