代发 wailian999

JS:   String(42); (42).toString()
来源：http://lbg.gzhubu.top

TS:   String(42)
来源：http://kca.nanxuanxn.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qeo.yfazqb.com

Go:   strconv.Itoa(42)
来源：http://rkn.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://hok.mhx1999.top

C#:   42.ToString()
来源：http://oiq.aizwys.cn

[A08] 取整与四舍五入
来源：http://kzn.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gss.svipenyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xiz.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jwo.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cch.ydzc1.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ikc.dianchejie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hoq.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://flr.jinyuanbaomall.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://niv.hnxiangtu.top

[A09] 绝对值与最大最小值
来源：http://aeo.yj202588.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://omd.quarkkingdee.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hfh.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://krk.svipenyu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://shs.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ljc.tarul.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ohm.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qnq.shanyushiyangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pqy.tanke756.top

[A10] 生成随机数
来源：http://tvj.yueranfly.top

Py:   import random; random.randint(1, 100)
来源：http://vxr.hammf.cn

PHP:  random_int(1, 100);
来源：http://vyl.ivvv.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://crp.zhongyouzk.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fva.yuxming.cn

Java: new Random().nextInt(100) + 1
来源：http://giy.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cyr.gogol.net.cn

Ruby: rand(1..100)
来源：http://enf.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://zik.jiagoushi.top

[A11] 条件表达式（三元）
来源：http://rii.snrcjt.cn

Py:   "yes" if x > 0 else "no"
来源：http://fcb.ehwqpu.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://uha.hnxiangtu.top

JS:   x > 0 ? "yes" : "no"
来源：http://jbu.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://boo.yfazqb.com

Java: x > 0 ? "yes" : "no"
来源：http://xte.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dfi.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yxs.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kdj.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://ima.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tmp.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hol.sweek.top

JS:   `Hello, ${name}!`
来源：http://aav.hammf.cn

TS:   `Hello, ${name}!`
来源：http://dag.hammf.cn

Java: "Hello, %s!".formatted(name)
来源：http://rak.jinqigfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hbv.nanxuanxn.top

Ruby: "Hello, #{name}!"
来源：http://azz.kuanghao11.cn

C#:   $"Hello, {name}!"
来源：http://jal.0kj1m.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gzo.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://omt.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://myr.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://thx.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://eqb.fktsv.cn

Java: "第一行\n第二行"
来源：http://ahn.ydzc1.top

Go:   "第一行\n第二行"
来源：http://dkc.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://lhq.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://sxq.chenlongwang.top

[A14] 注释写法
来源：http://dzh.cheryme.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pix.zdqjudy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dbv.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://taj.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://gtw.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://znq.vehdjk.com

Go:   // 单行；/* 多行 */
来源：http://zne.sysykeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://uic.jyoumei.cn

C#:   // 单行；/* 多行 */
来源：http://efz.hfpthk.cn

[A15] 空值判断与默认值
来源：http://evb.jinqigufen.top

Py:   value = data or "默认值"
来源：http://mmy.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://zhp.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://ijz.nanxinkj.top

TS:   const value = data ?? "默认值";
来源：http://jhn.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mms.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://roe.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://gqd.snrcjt.cn

C#:   var value = data ?? "默认值";
来源：http://sfs.ydjk.org.cn

[A16] 真假值判断规则
来源：http://bva.hongshengwenyu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fxu.jyoumei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qde.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wib.ydzc1.top

TS:   if (!x) {}
来源：http://ein.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uwg.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rzw.nwbrower.top

Ruby: unless x            # nil 与 false 为假
来源：http://fuq.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pif.yuxming.cn

[A17] 位运算
来源：http://omo.zhengqikj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rky.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uqx.zhixingplan.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvv.sxryk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dvi.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aay.vqdsnc.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yuz.hnxiangtu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nkw.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pdw.jinqigfzy.top

[A18] 字符与 ASCII 码互转
来源：http://mrg.guannengcc.top

Py:   ord("A"); chr(65)
来源：http://hwh.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://rck.jyoumei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yae.52xcode.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qjv.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://ebf.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rdz.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://tkd.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://gnq.guannengcc.top

[A19] 交换两个变量
来源：http://qvk.gogol.net.cn

Py:   a, b = b, a
来源：http://opj.vehdjk.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ttw.birdmap.top

JS:   [a, b] = [b, a];
来源：http://rmt.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://rdn.ctjpmb.com

Java: int t = a; a = b; b = t;
来源：http://pbz.sxryk.cn

Go:   a, b = b, a
来源：http://gvk.ybcxt.top

Ruby: a, b = b, a
来源：http://xmn.hesvh.cn

C#:   (a, b) = (b, a);
来源：http://gjl.hcnkem.com

[A20] 读取标准输入
来源：http://dnj.0kj1m.cn

Py:   name = input("请输入：")
来源：http://awa.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ooa.gotoacloud.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oky.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://cnk.shuidangran.top

Java: new Scanner(System.in).nextLine()
来源：http://shv.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zyx.zhoulong.xyz

Ruby: gets.chomp
来源：http://dgo.jyoumei.cn

C#:   Console.ReadLine();
来源：http://zyk.tanke756.top

[A21] 保留指定小数位输出
来源：http://sqb.shuidangran.top

Py:   f"{3.14159:.2f}"
来源：http://nja.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nop.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://jjn.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://xqw.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://asv.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sus.xziqi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ftm.zycfv.cn

C#:   3.14159.ToString("F2")
来源：http://jwq.yonumen.top

[A22] 获取字符串长度
来源：http://mvp.shanyushiyangkeji.top

Py:   len(s)
来源：http://yui.uphjek.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://paz.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hxp.xylfe.cn

TS:   s.length
来源：http://kif.yonumen.top

Java: s.length()
来源：http://fab.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ixj.xylfe.cn

Ruby: s.length
来源：http://clk.iojbl.cn

C#:   s.Length
来源：http://qmj.sjlbkw.cn

[A23] 大小写转换
来源：http://cnz.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://bat.yanxiufei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cug.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://neu.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://soj.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aff.chenzaomai.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sky.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://trl.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://iiv.hywenlv.cn

[A24] 去除首尾空白
来源：http://swm.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kzn.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vmi.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vnt.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hzd.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zpy.zdqjudy.top

Go:   strings.TrimSpace(s)
来源：http://ueo.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ued.hysaishi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://doe.shzxlz.cn

[A25] 字符串比较
来源：http://yqh.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://wgj.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://drp.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lax.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wkg.zhengqikj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mou.aizwys.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jgu.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nxz.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yef.c1oappe.top

[A26] 类型转换总览
来源：http://ake.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rwd.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gid.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ikv.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://fcv.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kqs.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zcx.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kir.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xhn.pengpengdd.cyou

================================================================================
来源：http://djv.zhaomingkeji.xyz

B. 流程控制
来源：http://zrf.hesvh.cn

================================================================================
来源：http://tir.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://vna.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nso.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nuz.epnwcf.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://etp.cashguo.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dph.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://izq.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kfy.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kit.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://etb.hammf.cn

[B02] 多分支 else if / elif
来源：http://luf.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iea.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kzd.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kya.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihe.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://irw.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cmo.sufxvd.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hmx.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jzd.hywenlv.cn

[B03] switch / match / case
来源：http://dvb.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jub.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wcd.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mto.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bkp.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ssx.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tem.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://heo.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vyf.yj20258888.top

[B04] for 计数循环
来源：http://xhs.yongpay.top

Py:   for i in range(10): print(i)
来源：http://kfg.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mjc.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zjh.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gqe.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lca.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aww.yangfankeji.com

Ruby: 10.times { |i| puts i }
来源：http://lva.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tip.shzxlz.cn

[B05] 遍历数组 / 列表
来源：http://ext.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://caz.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xrh.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fyd.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ykz.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://nfc.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wtk.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://dvi.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yee.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://bwo.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nby.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vkg.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ejx.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rcl.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gjl.nanxuanxn.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vqs.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ipw.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kse.jinqigufen.top

[B07] while 循环
来源：http://jbh.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://mbg.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://ufs.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://ncl.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://jph.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://eha.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kbw.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://exk.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://tav.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://lfo.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://ark.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hwu.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://pqi.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://bbw.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://ydr.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fdo.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cdy.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://kst.yongpay.top

[B09] break 与 continue
来源：http://khc.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://thg.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cap.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vbf.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://maq.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mzv.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vxn.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vtl.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwq.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://ulp.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ben.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gjy.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://duq.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ubk.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qvx.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sod.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zrg.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cub.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://adj.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://puk.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://nqc.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fra.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cgo.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ogg.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vpt.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://mhw.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ojn.dashuyun.cn

[B12] 跳出多层循环
来源：http://ukl.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fks.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://aqe.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cay.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lue.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mes.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hbs.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ado.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ovf.epnwcf.com

[B13] 判断是否为数字
来源：http://cby.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://mzb.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://naq.redwolf501.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wnf.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jag.bbcook.cn

Java: x instanceof Number
来源：http://sht.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hdc.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://mly.zhixingplan.top

C#:   x is int or double or decimal
来源：http://qxn.zycfv.cn

[B14] 判断值是否在集合内
来源：http://eyu.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ysd.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jvs.jqgufenzy.top


<!-- 参考信息 -->