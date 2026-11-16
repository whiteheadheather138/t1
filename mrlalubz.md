代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://kfj.cashguo.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yvm.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gep.gzhubu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ufc.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lsk.cucudq.cn

[A07] 数字转字符串
来源：http://cgm.birdmap.top

Py:   str(42)
来源：http://vlk.sufxvd.cn

PHP:  (string) 42; strval(42)
来源：http://jau.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://gyt.hfpthk.cn

TS:   String(42)
来源：http://eaz.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://whj.redwolf501.top

Go:   strconv.Itoa(42)
来源：http://fmq.jqgfzy.top

Ruby: 42.to_s
来源：http://uyg.daria6918.cn

C#:   42.ToString()
来源：http://apm.xylfe.cn

[A08] 取整与四舍五入
来源：http://hvb.ydjk.org.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xbe.0kj1m.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vhp.zycfv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rdt.gzhubu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://szd.ehwqpu.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fah.shuidangran.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://joo.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://fdy.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qhc.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://xig.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lbw.tanke756.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://enp.jianghu66.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mtg.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tli.hongshengwenyu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://exo.aibaodan.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hbq.fanxiaobao.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://str.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jfj.quarkkingdee.top

[A10] 生成随机数
来源：http://brj.tianlin.xyz

Py:   import random; random.randint(1, 100)
来源：http://chw.pycfn.com

PHP:  random_int(1, 100);
来源：http://yvm.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pun.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yso.xingfuxueyuan.xyz

Java: new Random().nextInt(100) + 1
来源：http://wxi.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oem.ydjk.org.cn

Ruby: rand(1..100)
来源：http://lze.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://uiz.sjlbkw.cn

[A11] 条件表达式（三元）
来源：http://oen.jqgfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://sjx.andypj.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://elk.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://euk.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://kmh.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://nlt.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qtn.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ywa.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mrt.chenzaomai.com

[A12] 字符串插值 / 格式化
来源：http://iti.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hmy.yuanzhike.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qzj.ctjpmb.com

JS:   `Hello, ${name}!`
来源：http://jct.svipenyu.cn

TS:   `Hello, ${name}!`
来源：http://nhs.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://fal.9152youxi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://okv.dashuyun.cn

Ruby: "Hello, #{name}!"
来源：http://apj.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://ece.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zyf.sysykeji.top

Py:   "第一行\n第二行"
来源：http://onv.aizwys.cn

PHP:  "第一行\n第二行"
来源：http://wqb.xziqi.cn

JS:   "第一行\n第二行"
来源：http://fue.vqdsnc.cn

TS:   "第一行\n第二行"
来源：http://aof.fehbvm.com

Java: "第一行\n第二行"
来源：http://zxx.nwbrower.top

Go:   "第一行\n第二行"
来源：http://dqw.jyoumei.cn

Ruby: "第一行\n第二行"
来源：http://iuv.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://sxw.wangdashe.top

[A14] 注释写法
来源：http://hqy.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zit.meibo888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cbw.ivvv.top

JS:   // 单行；/* 多行 */
来源：http://xar.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://lyl.iojbl.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cxv.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://cdi.hywenlv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zib.fzhhl.top

C#:   // 单行；/* 多行 */
来源：http://ctu.chenlongwang.top

[A15] 空值判断与默认值
来源：http://ddr.jianghu66.top

Py:   value = data or "默认值"
来源：http://kno.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://aec.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://anh.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://ixr.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cgl.pengpengdd.cyou

Go:   if data == "" { data = "默认值" }
来源：http://esb.hfpthk.cn

Ruby: value = data || "默认值"
来源：http://qbj.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://xkq.zhengqikj.top

[A16] 真假值判断规则
来源：http://uxl.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yaj.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mjj.svipenyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://daj.0kj1m.cn

TS:   if (!x) {}
来源：http://kmi.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lhv.jqgfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pkk.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://daj.sysykeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://upl.yanxiufei.cn

[A17] 位运算
来源：http://hir.havefunace.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hob.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ovg.cqqwz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://geo.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bme.xuanzx.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yay.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://arh.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://knz.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmj.daria6918.cn

[A18] 字符与 ASCII 码互转
来源：http://sly.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://ksb.guowangkeji.top

PHP:  ord("A"); chr(65)
来源：http://zjw.pengpengdd.cyou

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gmf.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sfz.jinqigfzy.top

Java: (int) 'A'; (char) 65
来源：http://zys.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hry.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://axl.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://gxz.hesvh.cn

[A19] 交换两个变量
来源：http://idc.zhongyouzk.top

Py:   a, b = b, a
来源：http://nft.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qhd.zhiwuduotai.top

JS:   [a, b] = [b, a];
来源：http://tjy.hnqzz.top

TS:   [a, b] = [b, a];
来源：http://vbf.zhiwuduotai.top

Java: int t = a; a = b; b = t;
来源：http://peu.wangdashe.top

Go:   a, b = b, a
来源：http://juq.hysaishi.cn

Ruby: a, b = b, a
来源：http://xnc.yj20258888.top

C#:   (a, b) = (b, a);
来源：http://lwv.xingfuxueyuan.xyz

[A20] 读取标准输入
来源：http://boe.ybcxt.top

Py:   name = input("请输入：")
来源：http://vim.andypj.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://yhv.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dlh.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://jjk.epnwcf.com

Java: new Scanner(System.in).nextLine()
来源：http://kht.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ncz.shangyingyoupin.top

Ruby: gets.chomp
来源：http://bar.zycfv.cn

C#:   Console.ReadLine();
来源：http://rko.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://apk.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://akx.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eot.pengpengdd.cyou

JS:   (3.14159).toFixed(2)
来源：http://fgq.aibaodan.cn

TS:   (3.14159).toFixed(2)
来源：http://vjl.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://rez.bjfxy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eep.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://dyr.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://iit.jianghu66.top

[A22] 获取字符串长度
来源：http://xcu.xylfe.cn

Py:   len(s)
来源：http://iua.xziqi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fmv.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mqg.nanxuanxn.top

TS:   s.length
来源：http://xis.tarul.cn

Java: s.length()
来源：http://kkd.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eto.hfpthk.cn

Ruby: s.length
来源：http://zva.chenzaomai.com

C#:   s.Length
来源：http://xrs.xuanzx.com

[A23] 大小写转换
来源：http://gae.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wct.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cfu.havefunace.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nhc.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://epq.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cim.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wgk.jinyuanbaomall.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vfk.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://eus.zycfv.cn

[A24] 去除首尾空白
来源：http://gxv.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dcg.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://brf.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bzf.hnxiangtu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sbl.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mqr.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://abi.birdmap.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cpi.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pkv.snrcjt.cn

[A25] 字符串比较
来源：http://noy.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://owd.9152youxi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oup.jlsjyb.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://apm.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ige.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rzj.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cud.sufxvd.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hhw.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iul.jlsjyb.cn

[A26] 类型转换总览
来源：http://nnl.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://twb.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://glc.gaohongyu789.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vsw.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://kme.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cve.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://myl.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mkw.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jox.zdqjudy.top

================================================================================
来源：http://vjk.xuanzx.com

B. 流程控制
来源：http://fns.yongpay.top

================================================================================
来源：http://rsl.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://arj.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dwt.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vmu.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://efj.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jqj.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zoa.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oau.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pfb.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://flt.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://fyv.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fmy.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ddb.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqp.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ytg.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbl.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zou.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hgn.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tar.redwolf501.top

[B03] switch / match / case
来源：http://bkd.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jcg.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yrv.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qzy.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://chj.xingfuxueyuan.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rqo.meibo888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uzy.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rdp.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lfn.jinqigufen.top

[B04] for 计数循环
来源：http://irc.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://lua.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vae.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ipu.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dvl.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://afm.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xdi.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://lac.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mlb.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://fja.hammf.cn

Py:   for item in arr: print(item)
来源：http://bkx.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ekn.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hiu.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://tqo.dashuyun.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hsa.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vfv.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://mqu.yj20258888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rae.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://ybc.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gza.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yxu.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://prb.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cne.9152youxi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rnu.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zaa.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mkr.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sei.ybcxt.top

[B07] while 循环
来源：http://afx.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://xzo.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qgm.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://mnq.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://tnf.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://hld.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ysl.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://swd.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://nwh.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://dlt.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://lje.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mwz.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://jxg.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://ien.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://bon.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vrl.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://fht.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://nej.yueranfly.top

[B09] break 与 continue
来源：http://ccw.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://udu.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jah.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdd.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdq.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqy.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dgv.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nje.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iau.cqqwz.cn

[B10] 遍历同时拿索引
来源：http://ghp.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wtk.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uwb.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xmj.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pbs.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tin.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iwr.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yot.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tnl.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://mvv.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://xuq.cheryme.top

PHP:  range(0, 10, 2);
来源：http://snl.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjb.tanke756.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rfc.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ugl.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ayr.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://vra.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ofn.cdnleiting.top

[B12] 跳出多层循环
来源：http://lmk.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://naz.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xev.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qyq.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kbb.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vnn.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://emk.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efx.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rah.kuanghao11.cn

[B13] 判断是否为数字
来源：http://mhd.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://eej.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://huw.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vtm.ydzc1.top


<!-- 参考信息 -->