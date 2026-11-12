代发 wailian999

JS:   String(42); (42).toString()
来源：http://zhk.xinyue.icu

TS:   String(42)
来源：http://lxc.316326.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://pqp.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://jqe.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://ztn.mhx1999.top

C#:   42.ToString()
来源：http://rxb.haohaochexian.top

[A08] 取整与四舍五入
来源：http://hbk.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xie.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dqj.fehbvm.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ypn.zhongyouzk.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xrg.jinqigufen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bzg.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://abk.tian-w.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://njq.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nxd.hfpthk.cn

[A09] 绝对值与最大最小值
来源：http://dam.tianlin.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hlu.guowangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eok.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://the.yuxming.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fyq.haohaochexian.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jek.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vun.feifeiyinyue.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://llp.316326.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tlx.yueranfly.top

[A10] 生成随机数
来源：http://omm.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://vvc.jinyuanbaomall.cn

PHP:  random_int(1, 100);
来源：http://lie.uphjek.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yrl.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ztg.xuetiantiany.cn

Java: new Random().nextInt(100) + 1
来源：http://hmw.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jjg.guannengcc.top

Ruby: rand(1..100)
来源：http://xha.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://zpm.wangdashe.top

[A11] 条件表达式（三元）
来源：http://vcq.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://tvo.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jwd.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kpe.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://ccq.nanxinkj.top

Java: x > 0 ? "yes" : "no"
来源：http://vpl.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bgp.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uqf.xylfe.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wcu.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://qpe.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tld.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wwp.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://afa.pengpengdd.cyou

TS:   `Hello, ${name}!`
来源：http://xpi.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://fwd.nanxinkj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bmf.quarkkingdee.top

Ruby: "Hello, #{name}!"
来源：http://ues.nwbrower.top

C#:   $"Hello, {name}!"
来源：http://zxj.shangyingyoupin.top

[A13] 多行字符串（练习 \n 转义）
来源：http://for.sweek.top

Py:   "第一行\n第二行"
来源：http://dpq.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://unu.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://qov.yvedp.cn

TS:   "第一行\n第二行"
来源：http://kqa.ctjpmb.com

Java: "第一行\n第二行"
来源：http://hnu.52xcode.cn

Go:   "第一行\n第二行"
来源：http://tzf.yj20258.top

Ruby: "第一行\n第二行"
来源：http://xsy.guannengcc.top

C#:   "第一行\n第二行"
来源：http://nux.hcnkem.com

[A14] 注释写法
来源：http://vjl.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://wgd.ivvv.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hgn.nanxinkj.top

JS:   // 单行；/* 多行 */
来源：http://jsc.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://xcn.gaohongyu789.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kpt.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://dqr.kuanghao11.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jcr.epnwcf.com

C#:   // 单行；/* 多行 */
来源：http://zwi.tianlin.xyz

[A15] 空值判断与默认值
来源：http://ded.guannengcc.top

Py:   value = data or "默认值"
来源：http://pbr.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://whv.yj20258.top

JS:   const value = data ?? "默认值";
来源：http://huk.tianlin.xyz

TS:   const value = data ?? "默认值";
来源：http://bwv.yanxiufei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gxf.epnwcf.com

Go:   if data == "" { data = "默认值" }
来源：http://sdj.feifeiyinyue.top

Ruby: value = data || "默认值"
来源：http://gxb.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://fxz.birdmap.top

[A16] 真假值判断规则
来源：http://swc.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dnu.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aim.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xop.wangshuangyany.cn

TS:   if (!x) {}
来源：http://sps.havefunace.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dky.dianchejie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zab.daxiang520.top

Ruby: unless x            # nil 与 false 为假
来源：http://uwu.yj202588.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xun.yfazqb.com

[A17] 位运算
来源：http://inu.gotoacloud.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbl.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nlh.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqy.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qdw.shanyushiyangtech.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aru.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aka.yonumen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyl.52xcode.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lzy.cucudq.cn

[A18] 字符与 ASCII 码互转
来源：http://qvw.xziqi.cn

Py:   ord("A"); chr(65)
来源：http://gdw.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://kje.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rmd.zhongyouzk.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jur.hesvh.cn

Java: (int) 'A'; (char) 65
来源：http://ppj.sysykeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pvo.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://ktp.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://qvv.fktsv.cn

[A19] 交换两个变量
来源：http://ubq.hongshengwenyu.top

Py:   a, b = b, a
来源：http://xos.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qbl.redwolf501.top

JS:   [a, b] = [b, a];
来源：http://qye.havefunace.top

TS:   [a, b] = [b, a];
来源：http://abf.tarul.cn

Java: int t = a; a = b; b = t;
来源：http://tom.52xcode.cn

Go:   a, b = b, a
来源：http://uhn.yvedp.cn

Ruby: a, b = b, a
来源：http://nsc.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://vkp.sysykeji.top

[A20] 读取标准输入
来源：http://qfb.cdnleiting.top

Py:   name = input("请输入：")
来源：http://vct.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kqr.meibo888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mwp.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://zce.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://qkj.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lms.zycfv.cn

Ruby: gets.chomp
来源：http://fmq.yvedp.cn

C#:   Console.ReadLine();
来源：http://ycf.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://lrv.yonumen.top

Py:   f"{3.14159:.2f}"
来源：http://cbw.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://svm.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://bmw.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://slg.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://hny.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dbd.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://bkm.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://aoj.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://hji.daria6918.cn

Py:   len(s)
来源：http://cdl.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fhi.ivvv.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xjh.ywan-chungtsiang.top

TS:   s.length
来源：http://mnx.ctjpmb.com

Java: s.length()
来源：http://ncl.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dmq.uphjek.com

Ruby: s.length
来源：http://qqe.fengsongda.top

C#:   s.Length
来源：http://bcv.yueranfly.top

[A23] 大小写转换
来源：http://hla.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ytv.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ios.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rhx.shanyushiyangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kef.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vnl.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vlk.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cvx.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ptg.hnxiangtu.top

[A24] 去除首尾空白
来源：http://mgz.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ldb.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zpb.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://apu.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://frr.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rlt.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://sxl.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wby.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gun.sjlbkw.cn

[A25] 字符串比较
来源：http://whl.guowangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://kxf.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kni.hammf.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://arv.daxiang520.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kwn.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lbx.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xmq.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mtu.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oey.nwbrower.top

[A26] 类型转换总览
来源：http://tmk.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bjh.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qqd.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wop.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://aby.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wvj.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hpr.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wyj.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dkq.hysaishi.cn

================================================================================
来源：http://wrs.hnxiangtu.top

B. 流程控制
来源：http://lzr.andypj.xyz

================================================================================
来源：http://xhn.xziqi.cn

[B01] 条件判断 if / else
来源：http://qni.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://koc.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kuc.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rtr.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://puk.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ocm.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ech.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ibu.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ycb.yfazqb.com

[B02] 多分支 else if / elif
来源：http://xgn.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hyk.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pyx.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://odr.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmp.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dvi.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qjs.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aah.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpj.nwbrower.top

[B03] switch / match / case
来源：http://yij.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qso.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wrv.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yrg.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://egt.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uoa.birdmap.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ikh.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fnf.nanxinkj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tpr.jqgfzy.top

[B04] for 计数循环
来源：http://usi.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://ggo.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rhk.daxiang520.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjs.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dfa.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wnp.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aqk.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://vlu.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hyx.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://wna.tian-w.cn

Py:   for item in arr: print(item)
来源：http://cff.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gph.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hkl.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zdi.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nzg.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bns.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://nya.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://egr.havefunace.top

[B06] 遍历字典 / 对象
来源：http://tig.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mnd.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pdc.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wtb.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ybk.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nfl.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wdb.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yvn.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://voe.havefunace.top

[B07] while 循环
来源：http://whu.c1oappe.top

Py:   while i < 10: i += 1
来源：http://rxm.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kqr.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://ife.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://mmk.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://vbi.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aib.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://ixz.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://pdo.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://vut.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://pgg.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hnx.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://bja.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://fwt.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://yak.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ygq.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://upg.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://ofb.jyoumei.cn

[B09] break 与 continue
来源：http://vhf.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mvw.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://clh.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edu.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufz.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdq.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://clt.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gbp.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqx.hesvh.cn

[B10] 遍历同时拿索引
来源：http://hjy.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wla.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eym.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://otl.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tne.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://izx.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gxn.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fxe.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mej.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://wao.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://ahr.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://uaw.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jef.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffr.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cqu.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wkc.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://aoi.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://txl.yj20258888.top

[B12] 跳出多层循环
来源：http://fzd.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gka.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cye.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ckd.jqgfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://psg.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cyz.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iyh.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cwn.kuanghao11.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sgt.fzhhl.top

[B13] 判断是否为数字
来源：http://nkp.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://gxa.0kj1m.cn

PHP:  is_numeric($x)
来源：http://xjd.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mpv.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghx.dianchejie.cn

Java: x instanceof Number
来源：http://mbh.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gio.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://ogz.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://olg.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://cty.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pps.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pzi.dashuyun.cn


<!-- 参考信息 -->