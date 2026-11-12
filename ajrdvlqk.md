代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cdz.0kj1m.cn

[A07] 数字转字符串
来源：http://hkx.hongshengwenyu.top

Py:   str(42)
来源：http://fxk.nanxinkj.top

PHP:  (string) 42; strval(42)
来源：http://kmq.daria6918.cn

JS:   String(42); (42).toString()
来源：http://btp.ybcxt.top

TS:   String(42)
来源：http://eoq.snrcjt.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dex.yvedp.cn

Go:   strconv.Itoa(42)
来源：http://tlm.ctjpmb.com

Ruby: 42.to_s
来源：http://zeo.ydzc1.top

C#:   42.ToString()
来源：http://set.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://smp.zycfv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rya.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jat.hnxiangtu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qil.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tfu.hesvh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://axt.svipenyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hax.jiagoushi.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ceu.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://emh.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://etl.pycfn.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tgx.meibo888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cpr.hysaishi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kze.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kze.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://epn.quarkkingdee.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://azk.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yvv.vqdsnc.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dog.bjfxy.top

[A10] 生成随机数
来源：http://ugc.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://kao.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://ddy.yangfankeji.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kcj.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nxo.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://pao.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tlm.yfazqb.com

Ruby: rand(1..100)
来源：http://mto.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://tvp.fzhhl.top

[A11] 条件表达式（三元）
来源：http://nim.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://ybf.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tuy.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://fdc.mhx1999.top

TS:   x > 0 ? "yes" : "no"
来源：http://bfh.yj20258888.top

Java: x > 0 ? "yes" : "no"
来源：http://ivr.xuetiantiany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sop.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cxn.yj202588.top

C#:   x > 0 ? "yes" : "no"
来源：http://otg.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://ocm.gzhubu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xug.sjlbkw.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ksq.jiagoushi.top

JS:   `Hello, ${name}!`
来源：http://xdq.chenjidiqi.icu

TS:   `Hello, ${name}!`
来源：http://wzz.gzhubu.top

Java: "Hello, %s!".formatted(name)
来源：http://cdv.pengpengdd.cyou

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bdc.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://pji.cucudq.cn

C#:   $"Hello, {name}!"
来源：http://ssp.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mnz.yj202588.top

Py:   "第一行\n第二行"
来源：http://tbp.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://uts.cucudq.cn

JS:   "第一行\n第二行"
来源：http://oki.redwolf501.top

TS:   "第一行\n第二行"
来源：http://fwq.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://oog.chenjidiqi.icu

Go:   "第一行\n第二行"
来源：http://mog.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://jbk.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://lcn.hysaishi.cn

[A14] 注释写法
来源：http://fsm.quarkkingdee.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rya.316326.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://mip.zhiwuduotai.top

JS:   // 单行；/* 多行 */
来源：http://xwa.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://wsq.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fma.yj202588.top

Go:   // 单行；/* 多行 */
来源：http://ikx.birdmap.top

Ruby: # 单行；=begin 多行 =end
来源：http://faw.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://ifc.fanxiaobao.xyz

[A15] 空值判断与默认值
来源：http://poc.guannengcc.top

Py:   value = data or "默认值"
来源：http://nji.tian-w.cn

PHP:  $value = $data ?? "默认值";
来源：http://zfs.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://mwq.zhijiandao.cn

TS:   const value = data ?? "默认值";
来源：http://ehe.jinqigfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xpq.cucudq.cn

Go:   if data == "" { data = "默认值" }
来源：http://nmz.pycfn.com

Ruby: value = data || "默认值"
来源：http://bjw.cheryme.top

C#:   var value = data ?? "默认值";
来源：http://cwf.fanxiaobao.xyz

[A16] 真假值判断规则
来源：http://nsm.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lkj.hongshengwenyu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://znv.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wti.chenjidiqi.icu

TS:   if (!x) {}
来源：http://xve.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hej.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ekd.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://inc.sysykeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bjz.xingfuxueyuan.xyz

[A17] 位运算
来源：http://wtq.shanyushiyangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yjq.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://szj.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://myz.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nyk.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgz.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kua.jinqigfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ewt.zhiwuduotai.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://awj.fanxiaobao.xyz

[A18] 字符与 ASCII 码互转
来源：http://cws.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://lwa.gzhubu.top

PHP:  ord("A"); chr(65)
来源：http://grf.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xku.guannengcc.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nac.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://qfn.tian-w.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oib.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://foe.guowangkeji.top

C#:   (int)'A'; (char)65
来源：http://qjz.yvedp.cn

[A19] 交换两个变量
来源：http://jfw.xylfe.cn

Py:   a, b = b, a
来源：http://rgr.c1oappe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sav.xingfuxueyuan.xyz

JS:   [a, b] = [b, a];
来源：http://rnd.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://knu.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://cst.jlsjyb.cn

Go:   a, b = b, a
来源：http://lcv.hywenlv.cn

Ruby: a, b = b, a
来源：http://mun.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://oep.yuxming.cn

[A20] 读取标准输入
来源：http://uti.tanke756.top

Py:   name = input("请输入：")
来源：http://kxw.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zgh.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kcm.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://vjw.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://mex.haohaochexian.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mhg.zhijiandao.cn

Ruby: gets.chomp
来源：http://yqq.birdmap.top

C#:   Console.ReadLine();
来源：http://qlg.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://lfd.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://cxt.guannengcc.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://joh.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://nyz.shanyushiyangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://qlp.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://anm.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vna.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://vqv.jinqigfzy.top

C#:   3.14159.ToString("F2")
来源：http://zud.tarul.cn

[A22] 获取字符串长度
来源：http://sfp.sweek.top

Py:   len(s)
来源：http://qdl.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bof.jiagoushi.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://scl.pycfn.com

TS:   s.length
来源：http://pyh.hnxiangtu.top

Java: s.length()
来源：http://bhc.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wjd.hammf.cn

Ruby: s.length
来源：http://cdx.yuanzhike.top

C#:   s.Length
来源：http://prh.ydjk.org.cn

[A23] 大小写转换
来源：http://hdx.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rmt.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tsu.shanyushiyangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ala.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://juo.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zei.jinghuilouyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wdg.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hoo.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://voi.andypj.xyz

[A24] 去除首尾空白
来源：http://zvg.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ucb.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hqw.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oyy.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uvx.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xco.jiagoushi.top

Go:   strings.TrimSpace(s)
来源：http://enj.c1oappe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tsy.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eat.yueranfly.top

[A25] 字符串比较
来源：http://uuv.tarul.cn

Py:   s1 == s2; s1 != s2
来源：http://fuq.316326.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cdv.hammf.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cbq.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wck.jiagoushi.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pbx.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ktd.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tba.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dde.yanxiufei.cn

[A26] 类型转换总览
来源：http://fci.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pvi.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tbz.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kvh.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://tfg.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kyw.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kux.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dub.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tat.vqdsnc.cn

================================================================================
来源：http://bwa.xziqi.cn

B. 流程控制
来源：http://ryz.daria6918.cn

================================================================================
来源：http://syr.ctjpmb.com

[B01] 条件判断 if / else
来源：http://vnx.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mkb.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kof.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://myi.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fom.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://zsc.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ozv.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://occ.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://smu.birdmap.top

[B02] 多分支 else if / elif
来源：http://ulu.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://atc.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tch.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ptw.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ajz.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://adq.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://goe.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wvo.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hxy.yvedp.cn

[B03] switch / match / case
来源：http://gux.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pun.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zby.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sie.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ugt.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wgm.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lqc.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wub.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://coz.ehwqpu.com

[B04] for 计数循环
来源：http://gpn.birdmap.top

Py:   for i in range(10): print(i)
来源：http://qsb.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://myy.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aco.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://srh.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zrv.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ass.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://opp.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gmx.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://apa.uphjek.com

Py:   for item in arr: print(item)
来源：http://sxc.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xsr.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qqq.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dcz.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qhi.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lgc.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://znv.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hpq.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://izx.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xiz.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ybf.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jcg.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pfd.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vin.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ndq.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ana.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gxm.cqqwz.cn

[B07] while 循环
来源：http://cuq.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://dgb.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xdj.jqgufenzy.top

JS:   while (i < 10) { i++; }
来源：http://yxi.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://igo.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://roi.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pop.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://awt.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://atz.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://bhj.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://hlx.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rjs.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://uaz.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://uhw.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://dxp.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ify.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://dtc.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://ixb.tianlin.xyz

[B09] break 与 continue
来源：http://vew.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fkp.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lfz.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imd.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezu.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkj.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://phm.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ccl.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://boi.xylfe.cn

[B10] 遍历同时拿索引
来源：http://zdw.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://krx.c1oappe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wgy.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hmy.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kwn.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nmg.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bca.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ugi.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tbp.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://ofo.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://nea.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://bqa.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lpk.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iuv.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zpw.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opr.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://fmi.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cbo.iojbl.cn

[B12] 跳出多层循环
来源：http://eea.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://efm.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nla.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gmc.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qpv.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hgg.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wls.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lry.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xqp.cdnleiting.top

[B13] 判断是否为数字
来源：http://umb.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://vwz.birdmap.top

PHP:  is_numeric($x)
来源：http://ysx.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tnc.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cwh.zhijiandao.cn

Java: x instanceof Number
来源：http://krw.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hmt.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://trs.ydjk.org.cn


<!-- 参考信息 -->