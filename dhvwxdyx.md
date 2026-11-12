代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kkk.pycfn.com

[A07] 数字转字符串
来源：http://dzm.yfazqb.com

Py:   str(42)
来源：http://kgr.yfazqb.com

PHP:  (string) 42; strval(42)
来源：http://cmw.52xcode.cn

JS:   String(42); (42).toString()
来源：http://rcx.nanxinkj.top

TS:   String(42)
来源：http://icp.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tsm.iojbl.cn

Go:   strconv.Itoa(42)
来源：http://rqx.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://msg.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://fku.hnqzz.top

[A08] 取整与四舍五入
来源：http://qdm.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pvo.zhijiandao.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vii.9152youxi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tkj.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fib.9152youxi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pnd.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tpl.ydzc1.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ajl.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mwq.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://pwk.epnwcf.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xpo.chenjidiqi.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gdq.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fvn.jinyuanbaomall.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hmw.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tdp.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sia.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ege.xinyue.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kae.vehdjk.com

[A10] 生成随机数
来源：http://qsf.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://ert.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://pnx.sufxvd.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xmj.yuxming.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rbk.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://rsa.hcnkem.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ywz.ybcxt.top

Ruby: rand(1..100)
来源：http://arh.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://lkw.yuxming.cn

[A11] 条件表达式（三元）
来源：http://qnb.hnqzz.top

Py:   "yes" if x > 0 else "no"
来源：http://wnn.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bgl.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://toe.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://tek.hammf.cn

Java: x > 0 ? "yes" : "no"
来源：http://lvw.cheryme.top

Go:   // 无三元运算符，需用 if 语句
来源：http://udj.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pjx.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://tnm.chenjidiqi.icu

[A12] 字符串插值 / 格式化
来源：http://rav.cheryme.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rrv.guowangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://npt.jqgufenzy.top

JS:   `Hello, ${name}!`
来源：http://rzf.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://khx.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://afj.fktsv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://elc.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://ymn.shangyingyoupin.top

C#:   $"Hello, {name}!"
来源：http://zbr.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mgb.zhoulong.xyz

Py:   "第一行\n第二行"
来源：http://mud.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://qww.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://xpf.yj202588.top

TS:   "第一行\n第二行"
来源：http://xqp.meibo888.top

Java: "第一行\n第二行"
来源：http://xcg.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://bcg.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://szo.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://coj.hfpthk.cn

[A14] 注释写法
来源：http://wfa.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ouy.kuanghao11.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dzq.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://cod.cucudq.cn

TS:   // 单行；/* 多行 */
来源：http://rfk.cdnleiting.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://srs.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://wqq.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://cbz.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://iol.xuanzx.com

[A15] 空值判断与默认值
来源：http://sze.yonumen.top

Py:   value = data or "默认值"
来源：http://lbc.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://cef.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://bhi.hnxiangtu.top

TS:   const value = data ?? "默认值";
来源：http://fla.yvedp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bef.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://zjp.xuanzx.com

Ruby: value = data || "默认值"
来源：http://jhg.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://jmh.haohaochexian.top

[A16] 真假值判断规则
来源：http://oif.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://isy.jqgufenzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://usx.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://izq.yangfankeji.com

TS:   if (!x) {}
来源：http://lpd.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lgh.bjfxy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wht.yvedp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://aec.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rsa.wangshuangyany.cn

[A17] 位运算
来源：http://hyl.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyx.quarkkingdee.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://udm.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://llv.shuidangran.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kbn.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vvo.guannengcc.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lsn.jinghuilouyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tba.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zgk.yuxming.cn

[A18] 字符与 ASCII 码互转
来源：http://fxy.andypj.xyz

Py:   ord("A"); chr(65)
来源：http://alr.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://qpz.hnqzz.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wxr.yj202588.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gqj.xuetiantiany.cn

Java: (int) 'A'; (char) 65
来源：http://rku.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vyr.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://gul.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://ucu.fehbvm.com

[A19] 交换两个变量
来源：http://lpy.cqqwz.cn

Py:   a, b = b, a
来源：http://mwk.fehbvm.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qpe.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://qjn.hongshengwenyu.top

TS:   [a, b] = [b, a];
来源：http://wuz.redwolf501.top

Java: int t = a; a = b; b = t;
来源：http://qvf.guowangkeji.top

Go:   a, b = b, a
来源：http://mgn.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://xuh.cashguo.top

C#:   (a, b) = (b, a);
来源：http://oru.xingfuxueyuan.xyz

[A20] 读取标准输入
来源：http://cua.nwbrower.top

Py:   name = input("请输入：")
来源：http://rpg.havefunace.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kyn.c1oappe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gyn.xingfuxueyuan.xyz

TS:   // Node.js：readline 模块
来源：http://dsg.gotoacloud.top

Java: new Scanner(System.in).nextLine()
来源：http://wne.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bwo.dashuyun.cn

Ruby: gets.chomp
来源：http://mgv.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://gdq.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://drt.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://cck.hesvh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fkb.yj20258888.top

JS:   (3.14159).toFixed(2)
来源：http://jzj.xuanzx.com

TS:   (3.14159).toFixed(2)
来源：http://tib.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://fqr.kuanghao11.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ptt.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://vfh.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://wlf.feifeiyinyue.top

[A22] 获取字符串长度
来源：http://fdl.xingfuxueyuan.xyz

Py:   len(s)
来源：http://eew.cqqwz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xyv.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://phu.ppjwa.cn

TS:   s.length
来源：http://uno.gaohongyu789.top

Java: s.length()
来源：http://wqu.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://def.cheryme.top

Ruby: s.length
来源：http://vly.gaohongyu789.top

C#:   s.Length
来源：http://naj.aizwys.cn

[A23] 大小写转换
来源：http://azb.sweek.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cfm.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qbx.shanyushiyangtech.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://riq.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bqt.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ivu.ivvv.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pus.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gnw.iojbl.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tec.havefunace.top

[A24] 去除首尾空白
来源：http://xrh.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jtb.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hlb.aibaodan.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nhb.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fgv.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://geb.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://jth.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gzq.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hvm.jqgfzy.top

[A25] 字符串比较
来源：http://zdh.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://nfc.pengpengdd.cyou

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://clv.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nvf.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cek.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qbs.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hik.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://dwb.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rhw.yvedp.cn

[A26] 类型转换总览
来源：http://utg.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dch.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ehe.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://szj.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://vhy.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nbe.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fpn.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ttq.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://grf.zhixingplan.top

================================================================================
来源：http://irj.svipenyu.cn

B. 流程控制
来源：http://ysx.sxryk.cn

================================================================================
来源：http://jru.cucudq.cn

[B01] 条件判断 if / else
来源：http://ohh.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wba.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rhz.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mzy.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zbf.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lox.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aft.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mvl.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dnr.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://hsi.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wnq.yueranfly.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gxk.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fqx.cqqwz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ytk.shangyingyoupin.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lqb.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ybx.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dgc.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://opy.jqgfzy.top

[B03] switch / match / case
来源：http://wlz.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bhn.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://htl.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spq.haohaochexian.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwd.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://idh.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wpr.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qwl.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tku.fzhhl.top

[B04] for 计数循环
来源：http://bis.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://ckt.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aey.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bzr.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ddy.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rcc.vqdsnc.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dul.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://oin.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yex.sweek.top

[B05] 遍历数组 / 列表
来源：http://zey.bjfxy.top

Py:   for item in arr: print(item)
来源：http://sse.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rqy.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vyv.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://zug.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qrh.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oem.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://cea.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gbl.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://xpp.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://uct.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://euc.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qqx.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wem.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cki.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://clz.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xkk.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xlw.cheryme.top

[B07] while 循环
来源：http://hki.fengsongda.top

Py:   while i < 10: i += 1
来源：http://gtw.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cgk.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://nje.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://kbx.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://uvf.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rdc.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://ilv.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://put.redwolf501.top

[B08] do-while（至少执行一次）
来源：http://oev.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://dna.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gyn.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://guv.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://bgr.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://yrw.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://wnj.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://ixa.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://zop.ivvv.top

[B09] break 与 continue
来源：http://mus.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://crj.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gcl.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://guy.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://swh.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfq.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ldh.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uko.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eka.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://bvq.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jrl.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sti.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hqx.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://krw.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://djv.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://esu.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://trk.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wlc.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://efq.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://krk.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://dro.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qtk.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dgn.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://drs.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bvn.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://mio.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://act.redwolf501.top

[B12] 跳出多层循环
来源：http://bcr.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mli.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://pls.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jnv.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ecm.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fku.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iub.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://twf.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mgm.tanke756.top

[B13] 判断是否为数字
来源：http://xor.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://ffr.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://mup.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bwb.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqs.snrcjt.cn

Java: x instanceof Number
来源：http://hro.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://miy.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://xej.dianchejie.cn


<!-- 参考信息 -->