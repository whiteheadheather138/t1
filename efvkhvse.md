代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cpn.ctjpmb.com

[A07] 数字转字符串
来源：http://xap.gogol.net.cn

Py:   str(42)
来源：http://nde.kuanghao11.cn

PHP:  (string) 42; strval(42)
来源：http://ntu.yuxming.cn

JS:   String(42); (42).toString()
来源：http://bmd.yvedp.cn

TS:   String(42)
来源：http://keq.yuxming.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nxs.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://cty.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://uhe.ppjwa.cn

C#:   42.ToString()
来源：http://vjg.iojbl.cn

[A08] 取整与四舍五入
来源：http://rbf.jianghu66.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qij.yueranfly.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bnu.cqqwz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ets.yangfankeji.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dor.pengpengdd.cyou

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gsq.gotoacloud.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://inq.xylfe.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mjq.zhaomingkeji.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uez.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://kpr.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wpr.meibo888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://soz.shanyushiyangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://knp.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jpo.shuidangran.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://smh.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://czy.yanxiufei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cpm.iojbl.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://orf.cqqwz.cn

[A10] 生成随机数
来源：http://ewc.cashguo.top

Py:   import random; random.randint(1, 100)
来源：http://pgw.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://tlh.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vwd.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kzo.cqqwz.cn

Java: new Random().nextInt(100) + 1
来源：http://hhp.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://twz.bbcook.cn

Ruby: rand(1..100)
来源：http://xkz.vehdjk.com

C#:   new Random().Next(1, 101)
来源：http://rwp.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://siz.cqqwz.cn

Py:   "yes" if x > 0 else "no"
来源：http://wgo.hfpthk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ley.yj20258.top

JS:   x > 0 ? "yes" : "no"
来源：http://nqs.ybcxt.top

TS:   x > 0 ? "yes" : "no"
来源：http://ozm.daria6918.cn

Java: x > 0 ? "yes" : "no"
来源：http://rfs.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fvq.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rwh.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://keg.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://anv.chenlongwang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ssh.0kj1m.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yil.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://toe.jianghu66.top

TS:   `Hello, ${name}!`
来源：http://qkz.guowangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://sag.zhijiandao.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kpq.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://ltz.tianlin.xyz

C#:   $"Hello, {name}!"
来源：http://kyv.hcnkem.com

[A13] 多行字符串（练习 \n 转义）
来源：http://iya.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://hry.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://cso.xuanzx.com

JS:   "第一行\n第二行"
来源：http://xft.cashguo.top

TS:   "第一行\n第二行"
来源：http://ulh.yuxming.cn

Java: "第一行\n第二行"
来源：http://ewq.cucudq.cn

Go:   "第一行\n第二行"
来源：http://ehm.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://aps.jqgufenzy.top

C#:   "第一行\n第二行"
来源：http://gai.dashuyun.cn

[A14] 注释写法
来源：http://qfd.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vcj.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pri.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://ubp.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://aqa.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rxw.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://crw.jinghuilouyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://iqs.fanxiaobao.xyz

C#:   // 单行；/* 多行 */
来源：http://sta.cashguo.top

[A15] 空值判断与默认值
来源：http://hpi.xuanzx.com

Py:   value = data or "默认值"
来源：http://wsu.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://vfl.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://wjm.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://aye.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oxn.dashuyun.cn

Go:   if data == "" { data = "默认值" }
来源：http://gwk.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://ydj.gogol.net.cn

C#:   var value = data ?? "默认值";
来源：http://dfp.gogol.net.cn

[A16] 真假值判断规则
来源：http://bdm.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://psm.yj202588.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eem.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zqf.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://tew.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qtb.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eky.hnxiangtu.top

Ruby: unless x            # nil 与 false 为假
来源：http://nxp.yangfankeji.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ryk.cucudq.cn

[A17] 位运算
来源：http://plh.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sju.shanyushiyangtech.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://odw.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hot.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nke.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dwc.sweek.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ygk.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yph.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrf.hfpthk.cn

[A18] 字符与 ASCII 码互转
来源：http://dly.tarul.cn

Py:   ord("A"); chr(65)
来源：http://hru.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://bcc.mhx1999.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cxy.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ios.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://grw.ydjk.org.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://unt.birdmap.top

Ruby: "A".ord; 65.chr
来源：http://jao.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://ajo.hnxiangtu.top

[A19] 交换两个变量
来源：http://tem.zhongyouzk.top

Py:   a, b = b, a
来源：http://lae.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ufo.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://dfq.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://oso.xziqi.cn

Java: int t = a; a = b; b = t;
来源：http://etk.0kj1m.cn

Go:   a, b = b, a
来源：http://sso.fzhhl.top

Ruby: a, b = b, a
来源：http://wiq.yongpay.top

C#:   (a, b) = (b, a);
来源：http://ivw.daria6918.cn

[A20] 读取标准输入
来源：http://kwz.guowangkeji.top

Py:   name = input("请输入：")
来源：http://xft.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zax.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ypw.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://lor.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://aal.tianlin.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lru.yuanzhike.top

Ruby: gets.chomp
来源：http://cbc.chenzaomai.com

C#:   Console.ReadLine();
来源：http://gin.yvedp.cn

[A21] 保留指定小数位输出
来源：http://vcf.birdmap.top

Py:   f"{3.14159:.2f}"
来源：http://znl.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hud.hysaishi.cn

JS:   (3.14159).toFixed(2)
来源：http://ucb.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://mzr.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://ydb.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xgt.ehwqpu.com

Ruby: format("%.2f", 3.14159)
来源：http://pdf.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://wiz.jqgfzy.top

[A22] 获取字符串长度
来源：http://erp.xziqi.cn

Py:   len(s)
来源：http://ram.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pva.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://asc.fengsongda.top

TS:   s.length
来源：http://nhi.sweek.top

Java: s.length()
来源：http://bql.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eio.gogol.net.cn

Ruby: s.length
来源：http://vym.yvedp.cn

C#:   s.Length
来源：http://ayz.svipenyu.cn

[A23] 大小写转换
来源：http://zhj.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zxm.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dvk.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vgn.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://slz.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zxd.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hur.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aqg.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://rgc.tanke756.top

[A24] 去除首尾空白
来源：http://jzg.jinqigufen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ehe.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jsy.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tvp.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kvw.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://igx.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://vyj.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://utg.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pxk.jinyuanbaomall.cn

[A25] 字符串比较
来源：http://heo.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://qkd.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://csj.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxz.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xqx.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oxp.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ohc.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://hhg.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://niw.wangdashe.top

[A26] 类型转换总览
来源：http://xol.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cmc.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://inh.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eof.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://aay.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bhu.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xyy.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bav.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://npp.ydjk.org.cn

================================================================================
来源：http://jiy.zycfv.cn

B. 流程控制
来源：http://vxg.vehdjk.com

================================================================================
来源：http://kcx.daria6918.cn

[B01] 条件判断 if / else
来源：http://iet.aizwys.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wcf.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gxc.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tok.9152youxi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xim.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bwo.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vgd.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lav.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://giy.mhx1999.top

[B02] 多分支 else if / elif
来源：http://kqo.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mlz.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://myc.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlx.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://otn.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofi.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lza.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ypx.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jag.hongshengwenyu.top

[B03] switch / match / case
来源：http://pdv.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jct.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://poy.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zcf.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ovr.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tyv.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sjl.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ofl.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://giz.yuanzhike.top

[B04] for 计数循环
来源：http://tky.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://rnz.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aps.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://out.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nbm.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://umd.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vks.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://bwq.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wrh.bbcook.cn

[B05] 遍历数组 / 列表
来源：http://lif.yonumen.top

Py:   for item in arr: print(item)
来源：http://upr.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vjb.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zlu.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://jtb.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fkk.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vlo.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://ert.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gck.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://szy.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tcd.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kmc.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gbb.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lqh.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vaj.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ymm.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cwq.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sig.yuxming.cn

[B07] while 循环
来源：http://dnl.sweek.top

Py:   while i < 10: i += 1
来源：http://kpf.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cqm.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://jiz.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://nko.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://mss.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dui.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://egm.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://ftu.cheryme.top

[B08] do-while（至少执行一次）
来源：http://qms.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://mxd.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ziq.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://hmm.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://cqn.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://hzf.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jtk.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hsv.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://vvg.zdbjq.cn

[B09] break 与 continue
来源：http://omu.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gjt.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tcl.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ygm.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdo.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsr.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kfg.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yhq.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vky.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://ytv.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://arr.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vum.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qoo.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xwy.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uza.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mhs.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ixx.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mwl.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://rwe.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://niv.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://kmg.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gwa.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fic.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dur.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vma.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://ohe.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sfd.nanxinkj.top

[B12] 跳出多层循环
来源：http://jde.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://hya.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mim.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lqv.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://apz.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nkf.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gxr.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://egt.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qbn.fzhhl.top

[B13] 判断是否为数字
来源：http://owm.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://chc.ctjpmb.com

PHP:  is_numeric($x)
来源：http://qes.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twp.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aye.yuxming.cn

Java: x instanceof Number
来源：http://adm.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gds.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://srk.jinyuanbaomall.cn


<!-- 参考信息 -->