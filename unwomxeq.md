代发 wailian999

JS:   String(42); (42).toString()
来源：http://lmu.tarul.cn

TS:   String(42)
来源：http://jly.smart0.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://mck.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://zqr.xuetiantiany.cn

Ruby: 42.to_s
来源：http://lau.fanxiaobao.xyz

C#:   42.ToString()
来源：http://vmq.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://laj.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wqz.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qjt.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://omg.tarul.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aka.ydjk.org.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jmk.fanxiaobao.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hsz.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tyj.ydzc1.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qbf.xylfe.cn

[A09] 绝对值与最大最小值
来源：http://rmq.yanxiufei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xtm.pycfn.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ekn.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://whq.yj20258.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rsj.zhijiandao.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uab.shzxlz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lzy.fehbvm.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bgm.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tbn.hnqzz.top

[A10] 生成随机数
来源：http://sxc.smart0.xyz

Py:   import random; random.randint(1, 100)
来源：http://rdr.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://aik.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cit.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gor.redwolf501.top

Java: new Random().nextInt(100) + 1
来源：http://vws.feifeiyinyue.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://amx.redwolf501.top

Ruby: rand(1..100)
来源：http://hvw.cqqwz.cn

C#:   new Random().Next(1, 101)
来源：http://xug.hesvh.cn

[A11] 条件表达式（三元）
来源：http://deu.ehwqpu.com

Py:   "yes" if x > 0 else "no"
来源：http://nxy.yanxiufei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://caa.iojbl.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bgj.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mlf.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://eor.wangshuangyany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mhx.zhaomingkeji.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://aep.nwbrower.top

C#:   x > 0 ? "yes" : "no"
来源：http://enq.sufxvd.cn

[A12] 字符串插值 / 格式化
来源：http://omz.nanxuanxn.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eqr.c1oappe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hrx.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://wcg.andypj.xyz

TS:   `Hello, ${name}!`
来源：http://bej.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://ijd.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jwi.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://rez.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://wvq.jinqigufen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://woj.bjfxy.top

Py:   "第一行\n第二行"
来源：http://jwy.snrcjt.cn

PHP:  "第一行\n第二行"
来源：http://yox.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://guf.yfazqb.com

TS:   "第一行\n第二行"
来源：http://law.guannengcc.top

Java: "第一行\n第二行"
来源：http://qxg.fehbvm.com

Go:   "第一行\n第二行"
来源：http://dkj.shanyushiyangkeji.top

Ruby: "第一行\n第二行"
来源：http://nyn.sweek.top

C#:   "第一行\n第二行"
来源：http://zef.tarul.cn

[A14] 注释写法
来源：http://rxg.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jea.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://npt.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://lnt.nwbrower.top

TS:   // 单行；/* 多行 */
来源：http://lrp.ctjpmb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vbv.cheryme.top

Go:   // 单行；/* 多行 */
来源：http://ogi.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tnj.bbcook.cn

C#:   // 单行；/* 多行 */
来源：http://yxp.zhoulong.xyz

[A15] 空值判断与默认值
来源：http://sgz.cdnleiting.top

Py:   value = data or "默认值"
来源：http://soa.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://hfv.vehdjk.com

JS:   const value = data ?? "默认值";
来源：http://muo.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://vfd.zhongyouzk.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wmv.sxryk.cn

Go:   if data == "" { data = "默认值" }
来源：http://ldy.feifeiyinyue.top

Ruby: value = data || "默认值"
来源：http://qlt.bbcook.cn

C#:   var value = data ?? "默认值";
来源：http://yuz.yueranfly.top

[A16] 真假值判断规则
来源：http://ptj.dianchejie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://htw.ehwqpu.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pyb.yj20258.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sll.xuetiantiany.cn

TS:   if (!x) {}
来源：http://nsh.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vks.jlsjyb.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bex.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fip.zdqjudy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gqp.feifeiyinyue.top

[A17] 位运算
来源：http://gmj.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tdh.cashguo.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rrv.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vrc.feifeiyinyue.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hgc.jqgfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bka.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yml.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sca.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbx.yvedp.cn

[A18] 字符与 ASCII 码互转
来源：http://kdo.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://yiu.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://szo.sxryk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vkr.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xll.pengpengdd.cyou

Java: (int) 'A'; (char) 65
来源：http://kvo.smart0.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://atv.shanyushiyangtech.top

Ruby: "A".ord; 65.chr
来源：http://eti.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://tqh.jinghuilouyu.cn

[A19] 交换两个变量
来源：http://gmr.yj20258888.top

Py:   a, b = b, a
来源：http://owu.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dsf.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://ejd.tanke756.top

TS:   [a, b] = [b, a];
来源：http://nip.chenjidiqi.icu

Java: int t = a; a = b; b = t;
来源：http://eha.yongpay.top

Go:   a, b = b, a
来源：http://ppm.hysaishi.cn

Ruby: a, b = b, a
来源：http://vdk.guowangkeji.top

C#:   (a, b) = (b, a);
来源：http://pap.aizwys.cn

[A20] 读取标准输入
来源：http://eju.guowangkeji.top

Py:   name = input("请输入：")
来源：http://ask.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wro.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pwy.pycfn.com

TS:   // Node.js：readline 模块
来源：http://gga.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://ybs.jinqigfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://szc.iojbl.cn

Ruby: gets.chomp
来源：http://zqw.ppjwa.cn

C#:   Console.ReadLine();
来源：http://nyk.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://mqu.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://wot.quarkkingdee.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ueb.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://wld.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://utb.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://jej.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dku.shanyushiyangtech.top

Ruby: format("%.2f", 3.14159)
来源：http://owa.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://svq.shzxlz.cn

[A22] 获取字符串长度
来源：http://yxb.hywenlv.cn

Py:   len(s)
来源：http://pzd.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pmf.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mzo.cucudq.cn

TS:   s.length
来源：http://ewh.aizwys.cn

Java: s.length()
来源：http://woe.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lqu.zhoulong.xyz

Ruby: s.length
来源：http://gyi.gotoacloud.top

C#:   s.Length
来源：http://pxm.xuanzx.com

[A23] 大小写转换
来源：http://umy.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ndi.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qdh.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://abs.meibo888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://maw.wangdashe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mzb.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jub.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://drb.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lik.wangdashe.top

[A24] 去除首尾空白
来源：http://usd.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://grj.c1oappe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lgb.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://whx.ybcxt.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ovq.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zrr.jqgfzy.top

Go:   strings.TrimSpace(s)
来源：http://byk.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tqi.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mtq.sysykeji.top

[A25] 字符串比较
来源：http://vrj.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://via.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fdf.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ree.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uwp.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://njp.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://roo.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dgg.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zdc.iojbl.cn

[A26] 类型转换总览
来源：http://nmr.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zko.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://udr.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hfx.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://bdn.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eon.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pjb.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://lpz.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lmb.bjfxy.top

================================================================================
来源：http://iaa.tian-w.cn

B. 流程控制
来源：http://mro.nanxinkj.top

================================================================================
来源：http://dxh.hnqzz.top

[B01] 条件判断 if / else
来源：http://bxd.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vml.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blm.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wzc.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pfj.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zzh.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jdx.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nsn.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vpu.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://cxi.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://axk.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tvm.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cin.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wqj.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvq.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ncp.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hot.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yle.gaohongyu789.top

[B03] switch / match / case
来源：http://cdj.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rlb.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tgh.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aco.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://riv.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mqh.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://psq.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bry.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pdz.gotoacloud.top

[B04] for 计数循环
来源：http://spc.316326.xyz

Py:   for i in range(10): print(i)
来源：http://vff.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dtx.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhc.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cnj.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uwo.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wkg.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://aqr.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cyq.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://ice.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://bkn.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pap.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eis.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wwa.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gcd.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://afr.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://vdz.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sgv.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://pgn.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lcr.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://snl.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpr.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wfo.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oyc.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://noa.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rqv.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aze.yvedp.cn

[B07] while 循环
来源：http://ptk.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://ntm.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://hjj.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://efq.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://jfy.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://kid.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jxo.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://wrp.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://juf.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://wyx.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://cym.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qip.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://bko.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://dtj.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://zfe.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nyj.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://kqa.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://sel.ivvv.top

[B09] break 与 continue
来源：http://oqr.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://esu.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ekm.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://znz.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lum.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpt.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sne.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zgu.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eqs.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://ugz.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fse.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iiw.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dpg.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nue.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://amj.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bng.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vjs.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ojv.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://jiq.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://zip.ivvv.top

PHP:  range(0, 10, 2);
来源：http://dpu.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yzd.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uji.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vou.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ejd.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://ifa.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fnr.zhoulong.xyz

[B12] 跳出多层循环
来源：http://xsv.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nug.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ltk.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bni.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fvh.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yiv.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pmy.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vpe.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rfd.hammf.cn

[B13] 判断是否为数字
来源：http://eav.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://izy.guannengcc.top

PHP:  is_numeric($x)
来源：http://cdu.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xmw.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oit.bjfxy.top

Java: x instanceof Number
来源：http://euv.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ber.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://xnj.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://npf.nwbrower.top

[B14] 判断值是否在集合内
来源：http://abb.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zbh.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lnj.bbcook.cn


<!-- 参考信息 -->