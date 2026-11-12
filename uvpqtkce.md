代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kyq.jianghu66.top

[A07] 数字转字符串
来源：http://vvv.yongpay.top

Py:   str(42)
来源：http://vyz.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://tmz.xinyue.icu

JS:   String(42); (42).toString()
来源：http://sak.yuxming.cn

TS:   String(42)
来源：http://oxc.jinqigufen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pdv.cheryme.top

Go:   strconv.Itoa(42)
来源：http://gyz.tarul.cn

Ruby: 42.to_s
来源：http://usy.xylfe.cn

C#:   42.ToString()
来源：http://piz.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://fcc.tian-w.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kli.xuanzx.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tjj.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qqd.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dil.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hrm.guannengcc.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ywr.dashuyun.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pmh.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uhx.yongpay.top

[A09] 绝对值与最大最小值
来源：http://mpb.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pix.xuanzx.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://see.zycfv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://syd.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ozk.zhijiandao.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xlv.iojbl.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fwu.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hmg.yuanzhike.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://foj.yuxming.cn

[A10] 生成随机数
来源：http://xia.nanxinkj.top

Py:   import random; random.randint(1, 100)
来源：http://gje.yueranfly.top

PHP:  random_int(1, 100);
来源：http://zyz.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mhb.chenzaomai.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yia.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://chp.chenjidiqi.icu

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ueq.gzhubu.top

Ruby: rand(1..100)
来源：http://hoi.sweek.top

C#:   new Random().Next(1, 101)
来源：http://ymr.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://ddz.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://lej.hnqzz.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kbh.tian-w.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xap.bbcook.cn

TS:   x > 0 ? "yes" : "no"
来源：http://asf.mhx1999.top

Java: x > 0 ? "yes" : "no"
来源：http://kad.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qko.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dsn.tarul.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uib.birdmap.top

[A12] 字符串插值 / 格式化
来源：http://xyy.zhengqikj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qib.nwbrower.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mag.52xcode.cn

JS:   `Hello, ${name}!`
来源：http://ezt.tarul.cn

TS:   `Hello, ${name}!`
来源：http://lcu.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://btr.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ddd.pycfn.com

Ruby: "Hello, #{name}!"
来源：http://lug.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://mkh.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://eca.uphjek.com

Py:   "第一行\n第二行"
来源：http://fvm.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://moj.kuanghao11.cn

JS:   "第一行\n第二行"
来源：http://fut.nanxuanxn.top

TS:   "第一行\n第二行"
来源：http://bkd.ybcxt.top

Java: "第一行\n第二行"
来源：http://euq.0kj1m.cn

Go:   "第一行\n第二行"
来源：http://xgn.hnxiangtu.top

Ruby: "第一行\n第二行"
来源：http://dhr.jinyuanbaomall.cn

C#:   "第一行\n第二行"
来源：http://gct.tian-w.cn

[A14] 注释写法
来源：http://lws.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dbg.c1oappe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mhd.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://wnj.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://fyz.cheryme.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wbg.xylfe.cn

Go:   // 单行；/* 多行 */
来源：http://odr.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rwt.xinyue.icu

C#:   // 单行；/* 多行 */
来源：http://byq.zdbjq.cn

[A15] 空值判断与默认值
来源：http://tdk.haohaochexian.top

Py:   value = data or "默认值"
来源：http://sin.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://mcp.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://xmt.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://ctj.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://isj.bjfxy.top

Go:   if data == "" { data = "默认值" }
来源：http://lwz.c1oappe.top

Ruby: value = data || "默认值"
来源：http://vmz.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://svk.shuidangran.top

[A16] 真假值判断规则
来源：http://txb.quarkkingdee.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lqx.quarkkingdee.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rqz.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xkz.shangyingyoupin.top

TS:   if (!x) {}
来源：http://opt.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wmw.daxiang520.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qzs.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kiq.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tcb.yanxiufei.cn

[A17] 位运算
来源：http://fxg.sufxvd.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xpv.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gjs.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dfh.c1oappe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rqh.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmu.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gst.kuanghao11.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zkz.mhx1999.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hdm.snrcjt.cn

[A18] 字符与 ASCII 码互转
来源：http://pmi.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://ftt.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://ags.zhengqikj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hng.316326.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gul.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://bgb.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fkq.yuanzhike.top

Ruby: "A".ord; 65.chr
来源：http://iar.yj202588.top

C#:   (int)'A'; (char)65
来源：http://spj.nanxuanxn.top

[A19] 交换两个变量
来源：http://fhk.daxiang520.top

Py:   a, b = b, a
来源：http://jga.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bxo.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://kfn.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://yms.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://ueo.hammf.cn

Go:   a, b = b, a
来源：http://bkl.guowangkeji.top

Ruby: a, b = b, a
来源：http://vfy.fengsongda.top

C#:   (a, b) = (b, a);
来源：http://cxg.zhongyouzk.top

[A20] 读取标准输入
来源：http://fvk.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://owt.shangyingyoupin.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qgx.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uru.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://nmz.shanyushiyangtech.top

Java: new Scanner(System.in).nextLine()
来源：http://hfr.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kwr.xziqi.cn

Ruby: gets.chomp
来源：http://wof.yonumen.top

C#:   Console.ReadLine();
来源：http://aul.pycfn.com

[A21] 保留指定小数位输出
来源：http://nmo.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://pyz.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://idx.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://eza.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://xso.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://ckc.bjfxy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://geq.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://doj.yanxiufei.cn

C#:   3.14159.ToString("F2")
来源：http://hbx.jiagoushi.top

[A22] 获取字符串长度
来源：http://yes.yonumen.top

Py:   len(s)
来源：http://zyx.sysykeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dyu.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yhd.aizwys.cn

TS:   s.length
来源：http://kuq.gzhubu.top

Java: s.length()
来源：http://rrp.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hli.gogol.net.cn

Ruby: s.length
来源：http://ght.jinqigufen.top

C#:   s.Length
来源：http://qlj.guowangkeji.top

[A23] 大小写转换
来源：http://dhk.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kqb.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hxk.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mkl.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zew.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pck.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yni.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fdn.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gxl.chenlongwang.top

[A24] 去除首尾空白
来源：http://xvj.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rse.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bnf.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bwy.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://miy.sweek.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wok.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://ayu.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zbw.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tzw.9152youxi.cn

[A25] 字符串比较
来源：http://pvf.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://dpe.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nly.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xlc.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yjw.zhiwuduotai.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ahy.snrcjt.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hgn.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dul.gotoacloud.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ixl.uphjek.com

[A26] 类型转换总览
来源：http://sop.vehdjk.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ggg.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://elb.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hsx.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://cac.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nmn.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uzt.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eoi.zhongyouzk.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mko.smart0.xyz

================================================================================
来源：http://ifc.cqqwz.cn

B. 流程控制
来源：http://pio.nwbrower.top

================================================================================
来源：http://uov.yj20258888.top

[B01] 条件判断 if / else
来源：http://vjj.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wdy.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://win.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vwd.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kjs.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vsh.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tuy.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sjw.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wbn.xylfe.cn

[B02] 多分支 else if / elif
来源：http://dmo.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wyg.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dud.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpw.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bim.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://opk.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pso.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://edu.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgb.316326.xyz

[B03] switch / match / case
来源：http://hho.jinghuilouyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qof.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vke.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://etm.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ubu.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://brw.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cyq.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fff.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hte.tianlin.xyz

[B04] for 计数循环
来源：http://bfl.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://cfg.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cdh.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nqf.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rac.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ceb.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rok.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://xbh.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zji.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://dzj.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://txq.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sgx.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dey.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vdg.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rro.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ejb.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://dzt.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yuz.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://jhc.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://mzt.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mpb.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ump.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jla.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wpb.guowangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://khq.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tox.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sqi.hywenlv.cn

[B07] while 循环
来源：http://hlt.daxiang520.top

Py:   while i < 10: i += 1
来源：http://gfd.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mik.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://lxz.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://jsm.316326.xyz

Java: while (i < 10) { i++; }
来源：http://xsf.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wkc.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://rmj.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://fgk.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://eca.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://ymc.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://srv.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://fnh.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://drw.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://wnu.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://udi.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yng.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://ygr.wangshuangyany.cn

[B09] break 与 continue
来源：http://fei.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ity.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://smh.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iaa.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gmj.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yah.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fug.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pxd.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ach.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://bwa.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rez.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cbj.feifeiyinyue.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lje.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://psp.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hlq.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fww.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fnk.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://agv.yonumen.top

[B11] 生成数字序列 / 区间
来源：http://vtj.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://fen.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://rqc.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://krr.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kuh.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tsy.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gfo.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://bxc.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xya.iojbl.cn

[B12] 跳出多层循环
来源：http://qoq.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lkf.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yna.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://igl.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://izq.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sxq.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ozo.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fzn.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://muc.haohaochexian.top

[B13] 判断是否为数字
来源：http://rih.ppjwa.cn

Py:   isinstance(x, (int, float))
来源：http://hfd.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://luh.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jhg.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ehr.jinqigfzy.top

Java: x instanceof Number
来源：http://olp.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hcm.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://bhk.zhongyouzk.top


<!-- 参考信息 -->