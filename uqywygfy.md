代发 wailian999

JS:   String(42); (42).toString()
来源：http://kei.yanxiufei.cn

TS:   String(42)
来源：http://gnd.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uyv.hnxiangtu.top

Go:   strconv.Itoa(42)
来源：http://hqx.c1oappe.top

Ruby: 42.to_s
来源：http://eyh.iojbl.cn

C#:   42.ToString()
来源：http://byb.bbcook.cn

[A08] 取整与四舍五入
来源：http://yqc.jqgufenzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://phn.xylfe.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jrr.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uzd.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vsi.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nbe.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kuv.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wua.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jji.dianchejie.cn

[A09] 绝对值与最大最小值
来源：http://wks.jqgfzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rqk.tarul.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fte.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kij.haohaochexian.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rgv.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zor.hysaishi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qgy.52xcode.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wky.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rxm.zycfv.cn

[A10] 生成随机数
来源：http://syz.gotoacloud.top

Py:   import random; random.randint(1, 100)
来源：http://icj.ehwqpu.com

PHP:  random_int(1, 100);
来源：http://bca.jyoumei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lim.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hnh.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://lnq.wangdashe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ixg.sjlbkw.cn

Ruby: rand(1..100)
来源：http://riu.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://cgt.wangdashe.top

[A11] 条件表达式（三元）
来源：http://sgy.guannengcc.top

Py:   "yes" if x > 0 else "no"
来源：http://diq.yj20258.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xlm.zhaomingkeji.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://zul.shangyingyoupin.top

TS:   x > 0 ? "yes" : "no"
来源：http://fkk.daxiang520.top

Java: x > 0 ? "yes" : "no"
来源：http://lfu.havefunace.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zix.xylfe.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zaw.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://aoy.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://whr.jqgufenzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eqk.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mmh.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://vov.ehwqpu.com

TS:   `Hello, ${name}!`
来源：http://uak.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://vre.ehwqpu.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nqq.nanxuanxn.top

Ruby: "Hello, #{name}!"
来源：http://tdj.dashuyun.cn

C#:   $"Hello, {name}!"
来源：http://dlg.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://hug.iojbl.cn

Py:   "第一行\n第二行"
来源：http://aqp.sweek.top

PHP:  "第一行\n第二行"
来源：http://ljo.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://cig.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://ims.wangdashe.top

Java: "第一行\n第二行"
来源：http://biu.gzhubu.top

Go:   "第一行\n第二行"
来源：http://gns.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://dnr.aizwys.cn

C#:   "第一行\n第二行"
来源：http://pkx.sxryk.cn

[A14] 注释写法
来源：http://onc.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://oyn.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jau.fzhhl.top

JS:   // 单行；/* 多行 */
来源：http://dvz.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://arg.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ans.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://ldu.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://yro.chenjidiqi.icu

C#:   // 单行；/* 多行 */
来源：http://qhk.yonumen.top

[A15] 空值判断与默认值
来源：http://ifj.jianghu66.top

Py:   value = data or "默认值"
来源：http://ees.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://ymo.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://lpk.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://wyn.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tbe.9152youxi.cn

Go:   if data == "" { data = "默认值" }
来源：http://moy.xingfuxueyuan.xyz

Ruby: value = data || "默认值"
来源：http://ilb.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://kjo.meibo888.top

[A16] 真假值判断规则
来源：http://iqg.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pps.guowangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ehy.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mit.tianlin.xyz

TS:   if (!x) {}
来源：http://jgv.zhijiandao.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dzn.zhijiandao.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fun.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://lak.dianchejie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://izd.jiagoushi.top

[A17] 位运算
来源：http://fik.dianchejie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://duq.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yjg.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxy.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mwp.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dqt.xziqi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gpu.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hyg.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yxv.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://xcg.yj202588.top

Py:   ord("A"); chr(65)
来源：http://vma.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://cfy.shanyushiyangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wsh.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hlf.sjlbkw.cn

Java: (int) 'A'; (char) 65
来源：http://jvc.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ydi.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://jkc.ehwqpu.com

C#:   (int)'A'; (char)65
来源：http://pmc.cucudq.cn

[A19] 交换两个变量
来源：http://sah.zhixingplan.top

Py:   a, b = b, a
来源：http://hnq.jlsjyb.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://exn.cqqwz.cn

JS:   [a, b] = [b, a];
来源：http://rps.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://xny.zhixingplan.top

Java: int t = a; a = b; b = t;
来源：http://oxe.quarkkingdee.top

Go:   a, b = b, a
来源：http://mhu.vqdsnc.cn

Ruby: a, b = b, a
来源：http://izb.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://mfk.yfazqb.com

[A20] 读取标准输入
来源：http://djw.sysykeji.top

Py:   name = input("请输入：")
来源：http://ekt.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://pnr.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ads.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://dvp.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://exn.shanyushiyangtech.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://knp.hongshengwenyu.top

Ruby: gets.chomp
来源：http://vty.9152youxi.cn

C#:   Console.ReadLine();
来源：http://pfl.xylfe.cn

[A21] 保留指定小数位输出
来源：http://xfb.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://ojo.xinyue.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tnr.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://fdf.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://jrp.cheryme.top

Java: String.format("%.2f", 3.14159)
来源：http://yev.cqqwz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jfw.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://nrd.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://khk.jqgufenzy.top

[A22] 获取字符串长度
来源：http://bbx.daria6918.cn

Py:   len(s)
来源：http://xyx.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qfc.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://opa.gaohongyu789.top

TS:   s.length
来源：http://rln.havefunace.top

Java: s.length()
来源：http://mmg.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dxb.epnwcf.com

Ruby: s.length
来源：http://rza.birdmap.top

C#:   s.Length
来源：http://jll.jianghu66.top

[A23] 大小写转换
来源：http://hxo.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://iys.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nxx.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zyn.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://huf.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lty.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wun.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xte.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vkz.cqqwz.cn

[A24] 去除首尾空白
来源：http://svv.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ajm.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yhc.yfazqb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hqy.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://huj.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ulh.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://zno.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://apv.hnxiangtu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oef.shangyingyoupin.top

[A25] 字符串比较
来源：http://zub.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://rul.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eiz.gogol.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zpl.xylfe.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tcp.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nnf.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iur.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ckw.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jsr.havefunace.top

[A26] 类型转换总览
来源：http://zfu.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://isn.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://epw.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://anu.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://uzq.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cxf.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aqw.0kj1m.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jlp.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rsr.nanxinkj.top

================================================================================
来源：http://pap.chenjidiqi.icu

B. 流程控制
来源：http://nev.c1oappe.top

================================================================================
来源：http://mkj.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://hfm.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://zig.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://erv.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://byo.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jfq.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ybh.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://isf.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zoo.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wve.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://rij.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sda.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xds.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://upq.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpy.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyc.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jhz.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ooq.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kab.jinqigufen.top

[B03] switch / match / case
来源：http://rhr.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://adm.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fmg.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ysh.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wyp.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tyh.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qxb.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wpg.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tet.mhx1999.top

[B04] for 计数循环
来源：http://imn.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://ybr.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qhc.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ydq.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pom.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gkf.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://raa.cashguo.top

Ruby: 10.times { |i| puts i }
来源：http://xct.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hup.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://mfz.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://xom.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ocg.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ytu.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cfr.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mcm.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hhi.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://ibu.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lup.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://utc.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wab.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fxk.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ory.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qmj.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbv.nanxuanxn.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ren.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dgn.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eym.aibaodan.cn

[B07] while 循环
来源：http://swi.andypj.xyz

Py:   while i < 10: i += 1
来源：http://yro.jianghu66.top

PHP:  while ($i < 10) { $i++; }
来源：http://mub.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://epy.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://xgx.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://yuk.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jnm.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://gtj.jyoumei.cn

C#:   while (i < 10) { i++; }
来源：http://jxf.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://gfq.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://qfv.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qde.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://ymz.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://wew.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://taq.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wgw.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://mwq.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://rwx.pycfn.com

[B09] break 与 continue
来源：http://ymo.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://duy.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pfb.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsb.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfd.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwg.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vkd.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vlm.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eho.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://oam.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iho.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vxl.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hmf.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://avo.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ziw.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gkl.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uzd.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wuf.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://gaf.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://ipc.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://yra.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eoh.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eja.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jii.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qyi.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://hjw.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jql.bbcook.cn

[B12] 跳出多层循环
来源：http://kcp.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kiy.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fjz.xingfuxueyuan.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sps.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dap.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eca.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://glt.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pxk.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gmx.redwolf501.top

[B13] 判断是否为数字
来源：http://skj.fzhhl.top

Py:   isinstance(x, (int, float))
来源：http://vkv.hesvh.cn

PHP:  is_numeric($x)
来源：http://xzf.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tis.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://stk.jqgfzy.top

Java: x instanceof Number
来源：http://nht.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eph.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://mkf.hammf.cn

C#:   x is int or double or decimal
来源：http://tgc.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://zqv.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kvt.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://agq.xingfuxueyuan.xyz


<!-- 参考信息 -->