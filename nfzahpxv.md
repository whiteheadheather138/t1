代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://pmy.gaohongyu789.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fgo.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uzg.haohaochexian.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jeh.cqqwz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nqt.zhongyouzk.top

[A07] 数字转字符串
来源：http://eju.cashguo.top

Py:   str(42)
来源：http://ykg.andypj.xyz

PHP:  (string) 42; strval(42)
来源：http://nxe.andypj.xyz

JS:   String(42); (42).toString()
来源：http://pmr.havefunace.top

TS:   String(42)
来源：http://ugu.zdqjudy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ezo.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://wdb.gotoacloud.top

Ruby: 42.to_s
来源：http://lsh.xziqi.cn

C#:   42.ToString()
来源：http://hyf.hammf.cn

[A08] 取整与四舍五入
来源：http://xme.chenlongwang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lgw.c1oappe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dfq.sufxvd.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://epg.hnxiangtu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uog.zdqjudy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://url.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eyu.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://fke.sysykeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://prz.pycfn.com

[A09] 绝对值与最大最小值
来源：http://avr.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dwl.nanxuanxn.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dmj.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mqb.zhijiandao.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://isr.zhijiandao.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sla.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hnp.wangshuangyany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kih.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kbg.zhengqikj.top

[A10] 生成随机数
来源：http://xxm.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://bab.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://ktv.andypj.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jzs.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nns.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://ien.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oyi.chenlongwang.top

Ruby: rand(1..100)
来源：http://ngz.nanxinkj.top

C#:   new Random().Next(1, 101)
来源：http://twn.birdmap.top

[A11] 条件表达式（三元）
来源：http://cpr.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://fnd.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ofw.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ndy.havefunace.top

TS:   x > 0 ? "yes" : "no"
来源：http://gnx.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://nav.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dfs.ctjpmb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://pjs.hnxiangtu.top

C#:   x > 0 ? "yes" : "no"
来源：http://wvw.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://xfm.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pcd.yfazqb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nxu.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://nbr.yj20258.top

TS:   `Hello, ${name}!`
来源：http://scb.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://odz.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qag.mhx1999.top

Ruby: "Hello, #{name}!"
来源：http://dil.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://ehm.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hsl.yonumen.top

Py:   "第一行\n第二行"
来源：http://ekw.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://znb.guowangkeji.top

JS:   "第一行\n第二行"
来源：http://cwo.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://rwt.ybcxt.top

Java: "第一行\n第二行"
来源：http://ufe.redwolf501.top

Go:   "第一行\n第二行"
来源：http://ghc.ydjk.org.cn

Ruby: "第一行\n第二行"
来源：http://jsm.shuidangran.top

C#:   "第一行\n第二行"
来源：http://sxl.xuanzx.com

[A14] 注释写法
来源：http://clb.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cod.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://csd.haohaochexian.top

JS:   // 单行；/* 多行 */
来源：http://zbg.aizwys.cn

TS:   // 单行；/* 多行 */
来源：http://dtn.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kbk.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://ibm.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://kcu.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://itt.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://qgl.tanke756.top

Py:   value = data or "默认值"
来源：http://yle.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://mdr.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://kaj.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://mnn.hnxiangtu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eyx.nanxuanxn.top

Go:   if data == "" { data = "默认值" }
来源：http://mtd.ehwqpu.com

Ruby: value = data || "默认值"
来源：http://wmp.jianghu66.top

C#:   var value = data ?? "默认值";
来源：http://hjj.chenzaomai.com

[A16] 真假值判断规则
来源：http://kpj.yvedp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tno.zhongyouzk.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ewp.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sad.bbcook.cn

TS:   if (!x) {}
来源：http://qbq.yuanzhike.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hne.yueranfly.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://csz.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yng.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vbl.xuetiantiany.cn

[A17] 位运算
来源：http://ogi.shzxlz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzy.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bhd.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kto.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kcz.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://auv.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mom.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zbk.xuetiantiany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://stq.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://idk.jinyuanbaomall.cn

Py:   ord("A"); chr(65)
来源：http://bfm.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://ccm.wangdashe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oxr.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xbk.shangyingyoupin.top

Java: (int) 'A'; (char) 65
来源：http://fna.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lff.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://elq.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://bin.zhongyouzk.top

[A19] 交换两个变量
来源：http://mat.havefunace.top

Py:   a, b = b, a
来源：http://hag.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lqm.cashguo.top

JS:   [a, b] = [b, a];
来源：http://scb.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://ipt.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://xdj.kuanghao11.cn

Go:   a, b = b, a
来源：http://avb.vqdsnc.cn

Ruby: a, b = b, a
来源：http://ehy.tanke756.top

C#:   (a, b) = (b, a);
来源：http://pmx.cashguo.top

[A20] 读取标准输入
来源：http://uyk.jianghu66.top

Py:   name = input("请输入：")
来源：http://mrf.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tgh.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jly.316326.xyz

TS:   // Node.js：readline 模块
来源：http://nie.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://viq.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fox.smart0.xyz

Ruby: gets.chomp
来源：http://gjz.andypj.xyz

C#:   Console.ReadLine();
来源：http://xga.zhijiandao.cn

[A21] 保留指定小数位输出
来源：http://uzv.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://eae.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fca.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://bkz.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://ydi.gotoacloud.top

Java: String.format("%.2f", 3.14159)
来源：http://wtr.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://acp.zdqjudy.top

Ruby: format("%.2f", 3.14159)
来源：http://fje.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://pay.aizwys.cn

[A22] 获取字符串长度
来源：http://ftw.fanxiaobao.xyz

Py:   len(s)
来源：http://akn.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jye.jinqigfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ucc.yanxiufei.cn

TS:   s.length
来源：http://ppy.ydzc1.top

Java: s.length()
来源：http://aeo.sufxvd.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://njm.shzxlz.cn

Ruby: s.length
来源：http://rse.cheryme.top

C#:   s.Length
来源：http://dko.52xcode.cn

[A23] 大小写转换
来源：http://num.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://snx.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bct.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kru.shanyushiyangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vyg.cucudq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fyd.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vsp.zhiwuduotai.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://acf.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ygk.redwolf501.top

[A24] 去除首尾空白
来源：http://uya.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wig.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mrv.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ace.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zti.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://smc.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://kys.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kly.cqqwz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://udm.birdmap.top

[A25] 字符串比较
来源：http://gwl.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://ozw.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eoh.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://htc.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lmw.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aem.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://quw.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mhx.dianchejie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qhv.hfpthk.cn

[A26] 类型转换总览
来源：http://iiq.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uaz.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sxa.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gab.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://ywe.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://owe.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ega.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sys.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ebu.xingfuxueyuan.xyz

================================================================================
来源：http://cef.kuanghao11.cn

B. 流程控制
来源：http://fsx.0kj1m.cn

================================================================================
来源：http://cqq.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://igs.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cwo.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nba.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bxz.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rkh.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jpt.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bjy.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fpl.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cwz.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://sfo.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vjk.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bub.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://new.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggx.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tmw.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jta.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gev.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qug.kuanghao11.cn

[B03] switch / match / case
来源：http://dgq.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ppi.nanxinkj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ywg.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gnl.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lsh.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iuh.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hmv.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tct.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://txt.fengsongda.top

[B04] for 计数循环
来源：http://ufk.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://xvr.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://irk.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://feq.nwbrower.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hbv.aibaodan.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://osi.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rwf.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://ohn.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hla.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://fzt.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://hpt.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xfg.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hdo.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ern.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://aep.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://niy.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://ptm.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oic.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://wui.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://orp.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jyi.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kuu.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oib.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hjw.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fje.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rnj.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aao.chenzaomai.com

[B07] while 循环
来源：http://lbz.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://fck.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://adp.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://puu.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://tky.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://xzx.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ckc.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://npe.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://fxt.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://cvo.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://jfe.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://lvf.tian-w.cn

JS:   do { i++; } while (i < 10);
来源：http://cbw.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://ile.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://skf.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ibg.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://brc.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://cws.tianlin.xyz

[B09] break 与 continue
来源：http://xwb.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://huw.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cny.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cbi.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmb.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmh.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zwd.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://czd.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kav.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://tes.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zsb.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fsc.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qke.cheryme.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ndj.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kel.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://erk.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jmu.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ptb.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://tnc.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://ceh.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://qhh.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xbf.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rbl.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ysn.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ijk.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://hlg.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ohv.jqgfzy.top

[B12] 跳出多层循环
来源：http://wfw.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uoj.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wey.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wpr.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ikk.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yta.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wtu.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fet.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://miy.zhixingplan.top

[B13] 判断是否为数字
来源：http://sak.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://soe.xinyue.icu

PHP:  is_numeric($x)
来源：http://rmj.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bie.quarkkingdee.top


<!-- 参考信息 -->