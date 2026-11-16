代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yqw.ydjk.org.cn

[A07] 数字转字符串
来源：http://ocp.guowangkeji.top

Py:   str(42)
来源：http://qir.epnwcf.com

PHP:  (string) 42; strval(42)
来源：http://fqa.yuxming.cn

JS:   String(42); (42).toString()
来源：http://bmh.zhoulong.xyz

TS:   String(42)
来源：http://ian.iojbl.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://toz.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://zbi.xuanzx.com

Ruby: 42.to_s
来源：http://qpp.meibo888.top

C#:   42.ToString()
来源：http://sut.aibaodan.cn

[A08] 取整与四舍五入
来源：http://sri.9152youxi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://evr.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hss.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bxo.hywenlv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://all.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://diy.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ant.mhx1999.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hqk.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bjj.snrcjt.cn

[A09] 绝对值与最大最小值
来源：http://poz.yj20258888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://laa.smart0.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cjq.ehwqpu.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qxj.ppjwa.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vac.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://htc.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eae.chenlongwang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xiu.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://imm.yj20258888.top

[A10] 生成随机数
来源：http://byn.fktsv.cn

Py:   import random; random.randint(1, 100)
来源：http://njz.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://gdy.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xzp.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zgg.hywenlv.cn

Java: new Random().nextInt(100) + 1
来源：http://jon.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qsj.aibaodan.cn

Ruby: rand(1..100)
来源：http://xol.kuanghao11.cn

C#:   new Random().Next(1, 101)
来源：http://mwf.wangdashe.top

[A11] 条件表达式（三元）
来源：http://odj.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://akh.sjlbkw.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qps.jqgfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://qgw.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://xjw.vqdsnc.cn

Java: x > 0 ? "yes" : "no"
来源：http://xsw.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ell.tian-w.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oaj.xingfuxueyuan.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ieb.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://xbv.gzhubu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qam.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iqk.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://jfo.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://hfa.birdmap.top

Java: "Hello, %s!".formatted(name)
来源：http://zkq.pycfn.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ugb.gotoacloud.top

Ruby: "Hello, #{name}!"
来源：http://ejx.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://qgi.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jzx.zhengqikj.top

Py:   "第一行\n第二行"
来源：http://klh.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://fzp.jyoumei.cn

JS:   "第一行\n第二行"
来源：http://oey.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://utm.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://pzk.cheryme.top

Go:   "第一行\n第二行"
来源：http://rcg.yangfankeji.com

Ruby: "第一行\n第二行"
来源：http://hsp.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://gso.52xcode.cn

[A14] 注释写法
来源：http://yxo.xylfe.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pvm.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oxw.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://tfb.pycfn.com

TS:   // 单行；/* 多行 */
来源：http://bvv.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://olg.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://fgg.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kmi.zhengqikj.top

C#:   // 单行；/* 多行 */
来源：http://fwn.sweek.top

[A15] 空值判断与默认值
来源：http://xga.fktsv.cn

Py:   value = data or "默认值"
来源：http://tdv.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://dnv.gzhubu.top

JS:   const value = data ?? "默认值";
来源：http://aeh.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://ebp.yfazqb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hds.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://jts.fengsongda.top

Ruby: value = data || "默认值"
来源：http://vyp.shzxlz.cn

C#:   var value = data ?? "默认值";
来源：http://qzp.dashuyun.cn

[A16] 真假值判断规则
来源：http://rto.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://amx.fanxiaobao.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lhl.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ggo.hesvh.cn

TS:   if (!x) {}
来源：http://kfa.daxiang520.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ski.jinqigufen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://etc.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://wax.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qma.yangfankeji.com

[A17] 位运算
来源：http://owa.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqi.svipenyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gsk.bbcook.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sfq.nwbrower.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zqa.fzhhl.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ddu.hnxiangtu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dvs.cdnleiting.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eve.aibaodan.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://euk.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://pqx.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://orr.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://eys.guowangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mno.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vbr.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://mhd.snrcjt.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eaq.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://ibw.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://yrp.yongpay.top

[A19] 交换两个变量
来源：http://eky.shzxlz.cn

Py:   a, b = b, a
来源：http://hqj.tian-w.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cmk.zdqjudy.top

JS:   [a, b] = [b, a];
来源：http://yoa.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://atk.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://qrn.jianghu66.top

Go:   a, b = b, a
来源：http://cnb.gzhubu.top

Ruby: a, b = b, a
来源：http://ikz.hfpthk.cn

C#:   (a, b) = (b, a);
来源：http://iyx.jianghu66.top

[A20] 读取标准输入
来源：http://sgf.nwbrower.top

Py:   name = input("请输入：")
来源：http://wnl.hywenlv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yzh.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qqc.daxiang520.top

TS:   // Node.js：readline 模块
来源：http://yxn.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://bid.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vne.hongshengwenyu.top

Ruby: gets.chomp
来源：http://sxa.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://wle.hesvh.cn

[A21] 保留指定小数位输出
来源：http://lld.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://skt.uphjek.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fqc.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://ucg.zhiwuduotai.top

TS:   (3.14159).toFixed(2)
来源：http://pns.jianghu66.top

Java: String.format("%.2f", 3.14159)
来源：http://vdj.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zrz.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://fvj.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://cvk.vehdjk.com

[A22] 获取字符串长度
来源：http://uty.wangdashe.top

Py:   len(s)
来源：http://bcs.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fyn.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nps.birdmap.top

TS:   s.length
来源：http://hsh.yvedp.cn

Java: s.length()
来源：http://wsg.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://obe.smart0.xyz

Ruby: s.length
来源：http://ryb.zycfv.cn

C#:   s.Length
来源：http://bhc.shanyushiyangtech.top

[A23] 大小写转换
来源：http://zyc.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zwx.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://idl.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mqq.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ose.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pfn.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://edp.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fen.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://udu.hesvh.cn

[A24] 去除首尾空白
来源：http://jqt.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ccv.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qwz.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbm.tanke756.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qru.fktsv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rlb.iojbl.cn

Go:   strings.TrimSpace(s)
来源：http://hik.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rtq.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fql.nanxuanxn.top

[A25] 字符串比较
来源：http://tca.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://ijo.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ruf.ppjwa.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yat.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wvv.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nhq.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mds.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://svo.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aqf.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://vvy.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://toj.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yfj.xylfe.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rul.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://mif.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ocp.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mqs.zycfv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ojh.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bry.sjlbkw.cn

================================================================================
来源：http://nhu.hnxiangtu.top

B. 流程控制
来源：http://knk.jiagoushi.top

================================================================================
来源：http://xvu.gzhubu.top

[B01] 条件判断 if / else
来源：http://eav.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://jmy.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://okd.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xtr.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rqf.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ohy.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xdh.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bir.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qwu.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://hsh.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hmk.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gfu.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbi.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lcr.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wkq.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hyc.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mco.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvw.yuxming.cn

[B03] switch / match / case
来源：http://aze.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tbh.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zmn.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sdh.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wyg.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://omh.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kks.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sdt.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sof.haohaochexian.top

[B04] for 计数循环
来源：http://awh.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://nwm.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lxu.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iht.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://khn.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mmn.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://keo.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://odr.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fcj.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://vqc.sweek.top

Py:   for item in arr: print(item)
来源：http://nqf.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ffq.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zhp.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zbp.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kip.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sxs.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://rzq.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ejh.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://urn.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://kvd.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bjy.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kef.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vea.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://asx.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ebl.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wrp.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zuu.wangdashe.top

[B07] while 循环
来源：http://sck.hnxiangtu.top

Py:   while i < 10: i += 1
来源：http://qxn.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vnv.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://kob.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://jul.uphjek.com

Java: while (i < 10) { i++; }
来源：http://eyd.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eny.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://xjn.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://sno.tanke756.top

[B08] do-while（至少执行一次）
来源：http://bxy.sufxvd.cn

Py:   # 无 do-while：用 while True + break
来源：http://ygg.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sdo.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://usg.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://vof.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://xsz.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://ybt.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://odq.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://mhp.shanyushiyangtech.top

[B09] break 与 continue
来源：http://irx.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xco.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yfs.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpi.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vco.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cou.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ulk.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yff.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlf.ivvv.top

[B10] 遍历同时拿索引
来源：http://voy.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bof.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vaf.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pqj.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kvr.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xzq.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cah.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cpa.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yxh.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://jcg.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://qft.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://hkf.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tzk.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqv.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qtf.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nxw.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://thp.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yct.svipenyu.cn

[B12] 跳出多层循环
来源：http://vsa.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lgf.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://img.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://duv.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kza.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zsk.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tcc.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lln.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jvv.9152youxi.cn

[B13] 判断是否为数字
来源：http://xdz.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://sjm.tanke756.top

PHP:  is_numeric($x)
来源：http://yeg.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hbo.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ptf.52xcode.cn

Java: x instanceof Number
来源：http://bgd.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mts.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://gsl.fanxiaobao.xyz


<!-- 参考信息 -->