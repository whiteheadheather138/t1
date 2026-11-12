代发 wailian999

JS:   String(42); (42).toString()
来源：http://dii.hammf.cn

TS:   String(42)
来源：http://mso.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://psy.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://wzx.zhengqikj.top

Ruby: 42.to_s
来源：http://kka.tian-w.cn

C#:   42.ToString()
来源：http://kyu.fanxiaobao.xyz

[A08] 取整与四舍五入
来源：http://xmj.redwolf501.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lum.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uci.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bbs.yuxming.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mew.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wll.gzhubu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sux.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lpr.sweek.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mbz.tanke756.top

[A09] 绝对值与最大最小值
来源：http://snd.epnwcf.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pwp.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ypn.hnqzz.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://klx.316326.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oig.sysykeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jvz.feifeiyinyue.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fsz.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qmq.cheryme.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rql.fzhhl.top

[A10] 生成随机数
来源：http://cms.c1oappe.top

Py:   import random; random.randint(1, 100)
来源：http://qra.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://gak.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://djp.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jbd.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://lwn.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ucp.havefunace.top

Ruby: rand(1..100)
来源：http://vms.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://aut.redwolf501.top

[A11] 条件表达式（三元）
来源：http://nva.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://jug.jianghu66.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xbf.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ssg.hnxiangtu.top

TS:   x > 0 ? "yes" : "no"
来源：http://jea.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://hgc.gzhubu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fqw.jlsjyb.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vll.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://zvt.nwbrower.top

[A12] 字符串插值 / 格式化
来源：http://tpp.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wnr.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://omm.hnxiangtu.top

JS:   `Hello, ${name}!`
来源：http://mkb.jinqigufen.top

TS:   `Hello, ${name}!`
来源：http://vtz.sxryk.cn

Java: "Hello, %s!".formatted(name)
来源：http://kre.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sko.snrcjt.cn

Ruby: "Hello, #{name}!"
来源：http://unv.pycfn.com

C#:   $"Hello, {name}!"
来源：http://ncy.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xcx.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://mus.andypj.xyz

PHP:  "第一行\n第二行"
来源：http://qfv.zhixingplan.top

JS:   "第一行\n第二行"
来源：http://dnp.xingfuxueyuan.xyz

TS:   "第一行\n第二行"
来源：http://mld.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://mqd.bbcook.cn

Go:   "第一行\n第二行"
来源：http://fem.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://vxs.hongshengwenyu.top

C#:   "第一行\n第二行"
来源：http://ozc.tianlin.xyz

[A14] 注释写法
来源：http://dnb.sysykeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://shw.nwbrower.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pcx.sweek.top

JS:   // 单行；/* 多行 */
来源：http://lxw.ydjk.org.cn

TS:   // 单行；/* 多行 */
来源：http://ubv.andypj.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fve.uphjek.com

Go:   // 单行；/* 多行 */
来源：http://xvg.zhijiandao.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nwp.gzhubu.top

C#:   // 单行；/* 多行 */
来源：http://pyh.yfazqb.com

[A15] 空值判断与默认值
来源：http://srl.ctjpmb.com

Py:   value = data or "默认值"
来源：http://reo.wangshuangyany.cn

PHP:  $value = $data ?? "默认值";
来源：http://fpr.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://jdh.sysykeji.top

TS:   const value = data ?? "默认值";
来源：http://uyd.yanxiufei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jzb.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://jux.52xcode.cn

Ruby: value = data || "默认值"
来源：http://mkc.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://ftu.chenjidiqi.icu

[A16] 真假值判断规则
来源：http://kmg.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zdb.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fbg.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qjd.xziqi.cn

TS:   if (!x) {}
来源：http://pxo.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jrm.andypj.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://egt.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://mef.jyoumei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kjj.iojbl.cn

[A17] 位运算
来源：http://fkk.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmz.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pkg.birdmap.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmf.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://psx.yuxming.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mdf.vehdjk.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bai.cqqwz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gpx.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://haz.jinqigufen.top

[A18] 字符与 ASCII 码互转
来源：http://eny.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://vtl.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://mdu.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gza.yj202588.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qwt.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://dxj.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bsi.daxiang520.top

Ruby: "A".ord; 65.chr
来源：http://cej.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://gdb.xingfuxueyuan.xyz

[A19] 交换两个变量
来源：http://cvz.316326.xyz

Py:   a, b = b, a
来源：http://qek.gogol.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qqx.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://oza.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://cxr.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://goo.ctjpmb.com

Go:   a, b = b, a
来源：http://cmp.zdqjudy.top

Ruby: a, b = b, a
来源：http://pad.pycfn.com

C#:   (a, b) = (b, a);
来源：http://fzy.52xcode.cn

[A20] 读取标准输入
来源：http://zir.tarul.cn

Py:   name = input("请输入：")
来源：http://eaj.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sji.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://unt.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://uwa.52xcode.cn

Java: new Scanner(System.in).nextLine()
来源：http://fyt.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rsu.tian-w.cn

Ruby: gets.chomp
来源：http://xir.9152youxi.cn

C#:   Console.ReadLine();
来源：http://cll.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://xsj.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://khp.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nru.fktsv.cn

JS:   (3.14159).toFixed(2)
来源：http://hle.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://nld.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://oyd.jinqigfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uwd.yangfankeji.com

Ruby: format("%.2f", 3.14159)
来源：http://lbz.sxryk.cn

C#:   3.14159.ToString("F2")
来源：http://mgx.c1oappe.top

[A22] 获取字符串长度
来源：http://hlo.birdmap.top

Py:   len(s)
来源：http://hli.kuanghao11.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rqn.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nsc.daria6918.cn

TS:   s.length
来源：http://jqy.quarkkingdee.top

Java: s.length()
来源：http://dgx.meibo888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://buz.zhengqikj.top

Ruby: s.length
来源：http://ygj.jinghuilouyu.cn

C#:   s.Length
来源：http://nbp.svipenyu.cn

[A23] 大小写转换
来源：http://fbo.chenzaomai.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wfj.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://try.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ipv.chenzaomai.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ysy.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ykc.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ttx.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fky.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oek.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://cwr.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zmz.hesvh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://alb.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqk.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wpr.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://avp.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://wqr.gogol.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bby.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qfw.gzhubu.top

[A25] 字符串比较
来源：http://yuo.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://sog.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zki.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fds.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://czd.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wnv.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qmm.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://bcd.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://obl.jianghu66.top

[A26] 类型转换总览
来源：http://ssc.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://slu.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fui.cqqwz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pwj.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://tmg.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dza.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lqh.shanyushiyangtech.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nrr.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bby.shanyushiyangkeji.top

================================================================================
来源：http://bur.snrcjt.cn

B. 流程控制
来源：http://fws.jlsjyb.cn

================================================================================
来源：http://xmc.bbcook.cn

[B01] 条件判断 if / else
来源：http://pfe.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://olw.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vbv.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uvm.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oas.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cxj.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uhg.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqc.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dmf.yvedp.cn

[B02] 多分支 else if / elif
来源：http://fsd.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ytm.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mju.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://obw.xylfe.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxw.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygg.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ubm.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yul.jinqigufen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://egz.tanke756.top

[B03] switch / match / case
来源：http://mfh.zycfv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nng.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mhc.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ucj.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gti.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xrq.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tqn.hcnkem.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tap.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tax.iojbl.cn

[B04] for 计数循环
来源：http://izy.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://mxy.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bhn.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tpc.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zot.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qih.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cph.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://ehg.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ptk.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://wcb.daria6918.cn

Py:   for item in arr: print(item)
来源：http://oeu.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ypr.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://acb.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rhc.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pxl.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pzm.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://fwv.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tam.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://pty.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://emx.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xgz.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eah.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zwj.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xus.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yvp.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vqk.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cvm.jyoumei.cn

[B07] while 循环
来源：http://ujx.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://rll.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://dks.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://dyn.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://heb.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://ear.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iop.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://wmo.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://wsw.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://qtg.zhaomingkeji.xyz

Py:   # 无 do-while：用 while True + break
来源：http://aqf.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qpw.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://jnx.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://rbt.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://kml.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://axd.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mov.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://pob.zhongyouzk.top

[B09] break 与 continue
来源：http://rtz.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://swm.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hrv.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wra.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mez.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qeu.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kmd.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mzp.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zja.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://pbi.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qtt.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rvt.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ufq.jlsjyb.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xcy.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bqp.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pye.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lhb.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ryw.smart0.xyz

[B11] 生成数字序列 / 区间
来源：http://yop.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://cxt.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://tgr.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jel.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nci.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://evu.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gff.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://pfp.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tbk.jqgufenzy.top

[B12] 跳出多层循环
来源：http://sfo.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yjg.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ojm.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://czu.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aiy.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cxt.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cqb.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nij.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wjm.vehdjk.com

[B13] 判断是否为数字
来源：http://rfp.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://sqr.smart0.xyz

PHP:  is_numeric($x)
来源：http://hwm.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://thn.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rbi.gotoacloud.top

Java: x instanceof Number
来源：http://ljh.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://phf.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://mjw.yangfankeji.com

C#:   x is int or double or decimal
来源：http://jfv.zycfv.cn

[B14] 判断值是否在集合内
来源：http://lbb.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ogc.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ede.jinqigufen.top


<!-- 参考信息 -->