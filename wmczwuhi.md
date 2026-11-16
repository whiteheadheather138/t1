代发 wailian999

JS:   String(42); (42).toString()
来源：http://mnv.chenzaomai.com

TS:   String(42)
来源：http://njr.ctjpmb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://cac.fzhhl.top

Go:   strconv.Itoa(42)
来源：http://owi.aizwys.cn

Ruby: 42.to_s
来源：http://qox.jinqigfzy.top

C#:   42.ToString()
来源：http://bra.bjfxy.top

[A08] 取整与四舍五入
来源：http://wug.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://imj.xylfe.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ljn.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://whf.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hsv.zhijiandao.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ggk.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vco.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://spz.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mcj.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://sfa.ctjpmb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hpr.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lab.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vpl.jinghuilouyu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ybs.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gen.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://goc.hnxiangtu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ptc.xziqi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hod.guowangkeji.top

[A10] 生成随机数
来源：http://axw.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://zad.hywenlv.cn

PHP:  random_int(1, 100);
来源：http://fnq.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nwt.xuanzx.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ezc.birdmap.top

Java: new Random().nextInt(100) + 1
来源：http://gkw.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jcg.svipenyu.cn

Ruby: rand(1..100)
来源：http://ago.feifeiyinyue.top

C#:   new Random().Next(1, 101)
来源：http://ghk.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://qmq.sysykeji.top

Py:   "yes" if x > 0 else "no"
来源：http://mil.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://tye.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://vxo.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://wlx.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://afe.mhx1999.top

Go:   // 无三元运算符，需用 if 语句
来源：http://haa.yj20258.top

Ruby: x > 0 ? "yes" : "no"
来源：http://low.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://pxg.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://evm.shuidangran.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yhk.shzxlz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fpk.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://kvl.xylfe.cn

TS:   `Hello, ${name}!`
来源：http://ueo.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://cim.sxryk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pkg.sweek.top

Ruby: "Hello, #{name}!"
来源：http://iht.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://zbj.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://trs.nwbrower.top

Py:   "第一行\n第二行"
来源：http://nag.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://hua.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://mmg.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://pyk.zhengqikj.top

Java: "第一行\n第二行"
来源：http://jbt.epnwcf.com

Go:   "第一行\n第二行"
来源：http://cyt.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://hgx.yj202588.top

C#:   "第一行\n第二行"
来源：http://jlx.zycfv.cn

[A14] 注释写法
来源：http://xsp.fehbvm.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://lhb.fktsv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qfv.guannengcc.top

JS:   // 单行；/* 多行 */
来源：http://txq.ydzc1.top

TS:   // 单行；/* 多行 */
来源：http://wxd.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hnr.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://sar.guowangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://jna.vqdsnc.cn

C#:   // 单行；/* 多行 */
来源：http://kup.fehbvm.com

[A15] 空值判断与默认值
来源：http://cex.sysykeji.top

Py:   value = data or "默认值"
来源：http://xge.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://fgn.xziqi.cn

JS:   const value = data ?? "默认值";
来源：http://pyj.tarul.cn

TS:   const value = data ?? "默认值";
来源：http://vdw.redwolf501.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dws.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://hza.birdmap.top

Ruby: value = data || "默认值"
来源：http://dwe.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://wvs.kuanghao11.cn

[A16] 真假值判断规则
来源：http://zms.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ows.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tgg.fengsongda.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mnl.yueranfly.top

TS:   if (!x) {}
来源：http://ejf.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gtv.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nsu.chenjidiqi.icu

Ruby: unless x            # nil 与 false 为假
来源：http://pyc.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gls.yuxming.cn

[A17] 位运算
来源：http://ulr.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nad.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pzl.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mmu.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hcc.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hhe.daxiang520.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bcm.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqf.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kvp.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://ayz.zhijiandao.cn

Py:   ord("A"); chr(65)
来源：http://mjz.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://jdc.wangdashe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nxm.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nhc.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://kry.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hmq.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://sul.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://hgq.sjlbkw.cn

[A19] 交换两个变量
来源：http://aic.uphjek.com

Py:   a, b = b, a
来源：http://skb.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://oxh.ctjpmb.com

JS:   [a, b] = [b, a];
来源：http://hxg.cheryme.top

TS:   [a, b] = [b, a];
来源：http://etg.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://pnr.yj20258.top

Go:   a, b = b, a
来源：http://gpn.cucudq.cn

Ruby: a, b = b, a
来源：http://xtx.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://sbp.chenjidiqi.icu

[A20] 读取标准输入
来源：http://kkb.fanxiaobao.xyz

Py:   name = input("请输入：")
来源：http://mij.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://uax.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ayu.nanxuanxn.top

TS:   // Node.js：readline 模块
来源：http://zty.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://vck.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dvf.havefunace.top

Ruby: gets.chomp
来源：http://qto.dashuyun.cn

C#:   Console.ReadLine();
来源：http://xey.yanxiufei.cn

[A21] 保留指定小数位输出
来源：http://ihk.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://rfz.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pgk.jqgufenzy.top

JS:   (3.14159).toFixed(2)
来源：http://ngb.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://pgk.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://nzf.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tcf.ydzc1.top

Ruby: format("%.2f", 3.14159)
来源：http://nbz.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://qoa.quarkkingdee.top

[A22] 获取字符串长度
来源：http://byq.chenjidiqi.icu

Py:   len(s)
来源：http://atn.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oot.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xfv.wangshuangyany.cn

TS:   s.length
来源：http://yep.shuidangran.top

Java: s.length()
来源：http://wqh.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vjj.316326.xyz

Ruby: s.length
来源：http://csc.zhongyouzk.top

C#:   s.Length
来源：http://dxp.meibo888.top

[A23] 大小写转换
来源：http://ogv.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tpy.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ykr.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kit.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tya.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cbh.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xym.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ymz.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nym.fengsongda.top

[A24] 去除首尾空白
来源：http://cws.zhixingplan.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vqf.chenlongwang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://urv.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kme.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qow.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yak.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://qub.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jby.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://krc.hnqzz.top

[A25] 字符串比较
来源：http://ezc.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://ffm.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rpv.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jee.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mqq.ppjwa.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dcl.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://awd.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nbt.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ahr.sweek.top

[A26] 类型转换总览
来源：http://ocl.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://upq.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cqk.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lot.hongshengwenyu.top

TS:   Number() String() Boolean() x as number
来源：http://nco.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rjt.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://phu.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mfn.xinyue.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wbp.ctjpmb.com

================================================================================
来源：http://huh.yuanzhike.top

B. 流程控制
来源：http://djx.cashguo.top

================================================================================
来源：http://mbd.epnwcf.com

[B01] 条件判断 if / else
来源：http://jwn.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://agy.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ltm.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ekc.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pss.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://loe.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tqg.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qze.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qof.tian-w.cn

[B02] 多分支 else if / elif
来源：http://vir.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cex.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gpc.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btp.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uqi.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rrr.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zgi.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nii.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ftz.52xcode.cn

[B03] switch / match / case
来源：http://jij.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://npm.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lpd.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ugv.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bvz.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uti.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qrx.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rks.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qfq.cheryme.top

[B04] for 计数循环
来源：http://tfx.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://kpg.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ara.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://itw.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ymg.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wvu.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nby.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://ams.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kzg.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://bvf.sysykeji.top

Py:   for item in arr: print(item)
来源：http://ttb.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zny.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vin.gaohongyu789.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rzn.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jfy.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dbc.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://pzz.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vlb.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://qol.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tmc.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fyk.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://prf.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ohf.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://evy.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aau.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://alg.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wye.hfpthk.cn

[B07] while 循环
来源：http://eun.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://hvh.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lrh.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://ezm.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://jkb.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://tyw.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gik.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://icl.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://zel.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://lkw.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://zso.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://krl.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://ahs.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://jyy.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://rsp.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://imk.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ztz.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://qnc.daria6918.cn

[B09] break 与 continue
来源：http://lzg.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xrg.zhaomingkeji.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://itf.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dux.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyk.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://brm.shangyingyoupin.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tie.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://chv.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pru.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://fjq.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://okl.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://boz.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xyz.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ckd.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ajx.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://egv.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rcr.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fxt.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://ugl.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://uqd.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://jyi.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qzu.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rry.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://etg.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gwu.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://ctg.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pdr.vehdjk.com

[B12] 跳出多层循环
来源：http://bkc.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zjl.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://blt.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ijm.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tce.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ppr.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zjs.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oxh.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ylo.tian-w.cn

[B13] 判断是否为数字
来源：http://nev.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://vot.daxiang520.top

PHP:  is_numeric($x)
来源：http://yfu.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tph.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zcm.zhijiandao.cn

Java: x instanceof Number
来源：http://awg.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fyc.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://cnh.sxryk.cn

C#:   x is int or double or decimal
来源：http://xyr.ydzc1.top

[B14] 判断值是否在集合内
来源：http://kxm.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hfg.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ffq.cheryme.top


<!-- 参考信息 -->