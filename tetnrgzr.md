代发 wailian999

JS:   String(42); (42).toString()
来源：http://gti.birdmap.top

TS:   String(42)
来源：http://hfk.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lzx.daria6918.cn

Go:   strconv.Itoa(42)
来源：http://vqz.hfpthk.cn

Ruby: 42.to_s
来源：http://ehz.kuanghao11.cn

C#:   42.ToString()
来源：http://dxh.mhx1999.top

[A08] 取整与四舍五入
来源：http://hvq.zhengqikj.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lct.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hze.xuanzx.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oim.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ail.vehdjk.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uhg.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pbx.uphjek.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://yvp.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mpy.feifeiyinyue.top

[A09] 绝对值与最大最小值
来源：http://ndb.yuanzhike.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://imm.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://olx.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dqe.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cuu.hongshengwenyu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hmj.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jdq.smart0.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qwg.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gxw.jinghuilouyu.cn

[A10] 生成随机数
来源：http://ysh.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://avv.ivvv.top

PHP:  random_int(1, 100);
来源：http://dwm.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lkb.tian-w.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://alg.jinghuilouyu.cn

Java: new Random().nextInt(100) + 1
来源：http://aeh.zhoulong.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wnn.0kj1m.cn

Ruby: rand(1..100)
来源：http://vsp.daria6918.cn

C#:   new Random().Next(1, 101)
来源：http://dzz.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://qbd.jinqigfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://bcr.ydzc1.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oqb.hcnkem.com

JS:   x > 0 ? "yes" : "no"
来源：http://pcf.cashguo.top

TS:   x > 0 ? "yes" : "no"
来源：http://sml.andypj.xyz

Java: x > 0 ? "yes" : "no"
来源：http://ukx.guowangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://lrl.svipenyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hoe.hammf.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gae.shangyingyoupin.top

[A12] 字符串插值 / 格式化
来源：http://dtn.yongpay.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zem.yuanzhike.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uso.hammf.cn

JS:   `Hello, ${name}!`
来源：http://cbf.xziqi.cn

TS:   `Hello, ${name}!`
来源：http://avd.tarul.cn

Java: "Hello, %s!".formatted(name)
来源：http://bbz.ywan-chungtsiang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bec.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://brz.fanxiaobao.xyz

C#:   $"Hello, {name}!"
来源：http://yuh.yonumen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kpk.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://aog.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://gpp.ehwqpu.com

JS:   "第一行\n第二行"
来源：http://cea.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://xnn.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://tbf.zhoulong.xyz

Go:   "第一行\n第二行"
来源：http://rcv.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://wjr.yj20258.top

C#:   "第一行\n第二行"
来源：http://ots.nanxinkj.top

[A14] 注释写法
来源：http://mci.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://tgp.jinqigufen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xyr.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://gek.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://ecw.ywan-chungtsiang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ort.fehbvm.com

Go:   // 单行；/* 多行 */
来源：http://zmp.zdbjq.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uec.pycfn.com

C#:   // 单行；/* 多行 */
来源：http://mno.9152youxi.cn

[A15] 空值判断与默认值
来源：http://ygx.fzhhl.top

Py:   value = data or "默认值"
来源：http://clm.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://kzh.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://ejy.hywenlv.cn

TS:   const value = data ?? "默认值";
来源：http://yzb.zhoulong.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vqx.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://mxt.shanyushiyangkeji.top

Ruby: value = data || "默认值"
来源：http://yyz.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://clh.fanxiaobao.xyz

[A16] 真假值判断规则
来源：http://emy.zycfv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rkv.shanyushiyangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fyp.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gxe.guowangkeji.top

TS:   if (!x) {}
来源：http://weu.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://asy.zhiwuduotai.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xfn.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jde.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vea.sjlbkw.cn

[A17] 位运算
来源：http://hjm.ctjpmb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ppb.shangyingyoupin.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tuk.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjv.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://owh.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qve.gzhubu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://awh.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vwu.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrw.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://qdk.snrcjt.cn

Py:   ord("A"); chr(65)
来源：http://fbf.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://izm.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pcu.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gms.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://boz.yueranfly.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ljo.hongshengwenyu.top

Ruby: "A".ord; 65.chr
来源：http://goo.hfpthk.cn

C#:   (int)'A'; (char)65
来源：http://vwc.nwbrower.top

[A19] 交换两个变量
来源：http://muj.sufxvd.cn

Py:   a, b = b, a
来源：http://hwg.xingfuxueyuan.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://jqv.sweek.top

JS:   [a, b] = [b, a];
来源：http://vxm.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://was.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://dmw.chenjidiqi.icu

Go:   a, b = b, a
来源：http://qhf.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://ukc.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://xsn.daxiang520.top

[A20] 读取标准输入
来源：http://xhy.hammf.cn

Py:   name = input("请输入：")
来源：http://yuf.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://iow.mhx1999.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://djb.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://atc.chenjidiqi.icu

Java: new Scanner(System.in).nextLine()
来源：http://bml.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://azm.aizwys.cn

Ruby: gets.chomp
来源：http://tqi.yj20258888.top

C#:   Console.ReadLine();
来源：http://eov.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://mmr.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://nvh.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ehs.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://pmc.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://wvr.haohaochexian.top

Java: String.format("%.2f", 3.14159)
来源：http://nem.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ftn.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://fkv.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://xgc.daxiang520.top

[A22] 获取字符串长度
来源：http://wkv.ppjwa.cn

Py:   len(s)
来源：http://yrd.zhixingplan.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bcl.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jmd.guowangkeji.top

TS:   s.length
来源：http://xrc.fehbvm.com

Java: s.length()
来源：http://gaw.bbcook.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tcq.316326.xyz

Ruby: s.length
来源：http://pwc.hesvh.cn

C#:   s.Length
来源：http://bij.yangfankeji.com

[A23] 大小写转换
来源：http://oww.tian-w.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jri.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vtr.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vcl.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://enm.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hwv.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ceb.svipenyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://trk.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://bmx.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://xhj.yueranfly.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pww.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://goe.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cre.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://upu.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qpb.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://sot.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ozl.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mhm.jianghu66.top

[A25] 字符串比较
来源：http://eui.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://mnr.tanke756.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oey.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://owz.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wfm.vqdsnc.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://plf.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nrt.chenjidiqi.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://dde.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lnw.smart0.xyz

[A26] 类型转换总览
来源：http://qdq.hesvh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hzz.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pzj.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gtw.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://vfw.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://itp.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zbv.chenzaomai.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://fbt.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yfk.guowangkeji.top

================================================================================
来源：http://rxb.dianchejie.cn

B. 流程控制
来源：http://qev.ydzc1.top

================================================================================
来源：http://ywb.dashuyun.cn

[B01] 条件判断 if / else
来源：http://lls.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://acp.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cki.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vmb.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tvx.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://zfe.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hdo.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tnl.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cfw.aizwys.cn

[B02] 多分支 else if / elif
来源：http://ioy.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ptj.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aaa.ppjwa.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://isn.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hep.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byb.hnqzz.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bqw.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://isc.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syb.jqgufenzy.top

[B03] switch / match / case
来源：http://pvy.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lfl.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yfw.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rkf.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://puq.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cnj.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nab.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ehn.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://awv.yj20258.top

[B04] for 计数循环
来源：http://rmg.316326.xyz

Py:   for i in range(10): print(i)
来源：http://ujo.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rpz.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vxp.xuetiantiany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufq.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xny.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gai.yangfankeji.com

Ruby: 10.times { |i| puts i }
来源：http://fvo.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iet.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://hhc.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://tcn.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pjk.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dxt.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ggo.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lim.gzhubu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://upu.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://njp.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mpk.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://sev.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mwh.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://any.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xcc.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pyd.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wjq.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sqj.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://svh.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vsq.yonumen.top

[B07] while 循环
来源：http://qtq.jianghu66.top

Py:   while i < 10: i += 1
来源：http://twq.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mvn.jinqigfzy.top

JS:   while (i < 10) { i++; }
来源：http://vqf.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://row.sweek.top

Java: while (i < 10) { i++; }
来源：http://vlv.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ool.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://oru.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://axu.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://mqo.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://eby.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rif.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://zzf.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://lod.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://wwj.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://frh.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kon.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://aqp.ctjpmb.com

[B09] break 与 continue
来源：http://gxn.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qpr.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://awl.zhijiandao.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvo.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbn.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bme.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lyw.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uxy.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjy.yj20258.top

[B10] 遍历同时拿索引
来源：http://tly.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aof.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qav.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://slh.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://inw.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uam.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qpj.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ema.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qya.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://bpt.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://xxd.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://aic.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lpm.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://coy.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vqc.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gcd.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://bwv.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lqw.aibaodan.cn

[B12] 跳出多层循环
来源：http://jmv.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ukh.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://fad.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gme.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vae.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tid.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://njs.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mcs.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hwc.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://lvf.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://yrx.ppjwa.cn

PHP:  is_numeric($x)
来源：http://pcm.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sex.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ulz.yangfankeji.com

Java: x instanceof Number
来源：http://epa.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vzc.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://ntw.zdbjq.cn

C#:   x is int or double or decimal
来源：http://vzx.hcnkem.com

[B14] 判断值是否在集合内
来源：http://ytc.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://szl.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sam.yuanzhike.top


<!-- 参考信息 -->