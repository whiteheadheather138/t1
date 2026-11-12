代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://scl.uphjek.com

[A07] 数字转字符串
来源：http://yir.guowangkeji.top

Py:   str(42)
来源：http://hzk.cheryme.top

PHP:  (string) 42; strval(42)
来源：http://qrw.yonumen.top

JS:   String(42); (42).toString()
来源：http://ubf.xinyue.icu

TS:   String(42)
来源：http://wlj.jinghuilouyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ked.dianchejie.cn

Go:   strconv.Itoa(42)
来源：http://puc.xylfe.cn

Ruby: 42.to_s
来源：http://eus.yanxiufei.cn

C#:   42.ToString()
来源：http://yhf.yj202588.top

[A08] 取整与四舍五入
来源：http://mca.hammf.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://akj.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yrm.cheryme.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ryv.pengpengdd.cyou

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tdn.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xzb.xylfe.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mjy.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://izk.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mvc.wangshuangyany.cn

[A09] 绝对值与最大最小值
来源：http://oes.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gnn.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ues.jinghuilouyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eqv.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://apm.yuanzhike.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fop.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://slu.yj202588.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eab.vqdsnc.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lvd.daxiang520.top

[A10] 生成随机数
来源：http://zcn.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://fuh.redwolf501.top

PHP:  random_int(1, 100);
来源：http://trs.jiagoushi.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vqx.ppjwa.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ivn.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://vbe.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zqo.yuanzhike.top

Ruby: rand(1..100)
来源：http://pvc.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://tlc.yvedp.cn

[A11] 条件表达式（三元）
来源：http://xco.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://eqq.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zps.guannengcc.top

JS:   x > 0 ? "yes" : "no"
来源：http://srx.vqdsnc.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uqu.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://vwk.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://doq.iojbl.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pwh.ywan-chungtsiang.top

C#:   x > 0 ? "yes" : "no"
来源：http://tir.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://hsp.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wbe.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rsp.cucudq.cn

JS:   `Hello, ${name}!`
来源：http://uje.jinghuilouyu.cn

TS:   `Hello, ${name}!`
来源：http://cmj.jiagoushi.top

Java: "Hello, %s!".formatted(name)
来源：http://tnj.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bru.dianchejie.cn

Ruby: "Hello, #{name}!"
来源：http://ter.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://nue.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://cdt.yj202588.top

Py:   "第一行\n第二行"
来源：http://bqi.hysaishi.cn

PHP:  "第一行\n第二行"
来源：http://nxv.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://kns.gogol.net.cn

TS:   "第一行\n第二行"
来源：http://pcx.aizwys.cn

Java: "第一行\n第二行"
来源：http://lfo.hesvh.cn

Go:   "第一行\n第二行"
来源：http://vtu.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://lwd.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://eth.hammf.cn

[A14] 注释写法
来源：http://oxe.xuanzx.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://fai.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wye.gogol.net.cn

JS:   // 单行；/* 多行 */
来源：http://evy.iojbl.cn

TS:   // 单行；/* 多行 */
来源：http://gww.zhoulong.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wfl.yfazqb.com

Go:   // 单行；/* 多行 */
来源：http://vvk.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lnl.wangshuangyany.cn

C#:   // 单行；/* 多行 */
来源：http://ifg.chenjidiqi.icu

[A15] 空值判断与默认值
来源：http://zoi.ctjpmb.com

Py:   value = data or "默认值"
来源：http://wbb.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://vmm.yfazqb.com

JS:   const value = data ?? "默认值";
来源：http://ody.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://rxp.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rpv.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://srz.yongpay.top

Ruby: value = data || "默认值"
来源：http://yhe.jlsjyb.cn

C#:   var value = data ?? "默认值";
来源：http://ruh.gzhubu.top

[A16] 真假值判断规则
来源：http://uow.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qtw.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qau.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vmo.jyoumei.cn

TS:   if (!x) {}
来源：http://pic.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yto.dianchejie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bsy.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://apb.fehbvm.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://miq.yanxiufei.cn

[A17] 位运算
来源：http://njk.redwolf501.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yra.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ozo.jinqigfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xap.tanke756.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fwg.zhiwuduotai.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgy.chenzaomai.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xnb.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olt.tarul.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtm.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://hch.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://nxh.ydjk.org.cn

PHP:  ord("A"); chr(65)
来源：http://pzt.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://meh.zhongyouzk.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uez.yj202588.top

Java: (int) 'A'; (char) 65
来源：http://kpt.jinyuanbaomall.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zok.dianchejie.cn

Ruby: "A".ord; 65.chr
来源：http://qmu.zhengqikj.top

C#:   (int)'A'; (char)65
来源：http://inb.tanke756.top

[A19] 交换两个变量
来源：http://umm.tarul.cn

Py:   a, b = b, a
来源：http://eip.ybcxt.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ufx.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://mju.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://fln.ctjpmb.com

Java: int t = a; a = b; b = t;
来源：http://weo.pengpengdd.cyou

Go:   a, b = b, a
来源：http://isi.9152youxi.cn

Ruby: a, b = b, a
来源：http://lib.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://vvh.nwbrower.top

[A20] 读取标准输入
来源：http://hry.ctjpmb.com

Py:   name = input("请输入：")
来源：http://boh.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zcp.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ukm.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://ozx.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://xet.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uqw.yongpay.top

Ruby: gets.chomp
来源：http://quy.tianlin.xyz

C#:   Console.ReadLine();
来源：http://euv.feifeiyinyue.top

[A21] 保留指定小数位输出
来源：http://yaq.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://mth.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yvf.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://tja.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://rqu.ywan-chungtsiang.top

Java: String.format("%.2f", 3.14159)
来源：http://lgt.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ucu.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://ldt.hnxiangtu.top

C#:   3.14159.ToString("F2")
来源：http://qea.yanxiufei.cn

[A22] 获取字符串长度
来源：http://ajb.jinghuilouyu.cn

Py:   len(s)
来源：http://kcb.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://urf.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bdb.pengpengdd.cyou

TS:   s.length
来源：http://jns.zdqjudy.top

Java: s.length()
来源：http://uiw.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vtm.vqdsnc.cn

Ruby: s.length
来源：http://egx.yj20258.top

C#:   s.Length
来源：http://ziu.tarul.cn

[A23] 大小写转换
来源：http://gtl.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://dic.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ldw.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rmg.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wyt.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fqx.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aup.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nle.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uot.ppjwa.cn

[A24] 去除首尾空白
来源：http://yyt.iojbl.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://drk.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mao.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bvi.daria6918.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gtj.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bdp.yongpay.top

Go:   strings.TrimSpace(s)
来源：http://uqh.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cnm.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cde.gaohongyu789.top

[A25] 字符串比较
来源：http://jfj.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://pyh.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vvm.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wof.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yll.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://twt.snrcjt.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qso.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ukp.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://foz.bbcook.cn

[A26] 类型转换总览
来源：http://dcn.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jpm.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hsb.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uwm.vehdjk.com

TS:   Number() String() Boolean() x as number
来源：http://xan.nwbrower.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jar.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://izj.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://osc.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gjp.yuanzhike.top

================================================================================
来源：http://ves.shuidangran.top

B. 流程控制
来源：http://cim.ydjk.org.cn

================================================================================
来源：http://crm.yuxming.cn

[B01] 条件判断 if / else
来源：http://vxn.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bha.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qpo.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xay.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fyq.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://htz.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://trj.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kuq.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iql.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://ptj.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://plw.havefunace.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oju.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipx.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmj.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btr.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tvw.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pbg.daria6918.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://omd.vqdsnc.cn

[B03] switch / match / case
来源：http://usk.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kdx.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rjq.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cgw.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sah.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pnc.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kas.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bbw.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jcb.tianlin.xyz

[B04] for 计数循环
来源：http://hpn.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://syf.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wme.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgj.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kce.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ppm.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oou.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://zyt.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://khj.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://kqe.vehdjk.com

Py:   for item in arr: print(item)
来源：http://tkg.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cla.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jhx.tarul.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wdh.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vlt.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://goe.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://fyd.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ozk.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://nxo.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hil.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://png.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://grn.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aii.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pea.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nam.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mvf.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tbu.haohaochexian.top

[B07] while 循环
来源：http://ycw.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://txu.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://zeu.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://yts.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://bss.meibo888.top

Java: while (i < 10) { i++; }
来源：http://ymy.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dxe.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://qyf.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://zpo.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://oue.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://hiz.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ejr.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://fhb.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://khn.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://aib.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tvz.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cqh.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://eqq.c1oappe.top

[B09] break 与 continue
来源：http://fqm.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rdl.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nlo.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lcp.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbg.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgj.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wgl.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mdt.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ube.yueranfly.top

[B10] 遍历同时拿索引
来源：http://mjj.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mpk.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tpk.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bvv.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nvw.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hne.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zqg.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cox.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zuh.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://neh.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://otz.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://urz.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oxi.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ese.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wes.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gxr.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://hcw.dianchejie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://efa.yvedp.cn

[B12] 跳出多层循环
来源：http://dea.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://erq.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://qpn.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbx.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bwl.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qtk.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ttr.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wzf.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://opp.hywenlv.cn

[B13] 判断是否为数字
来源：http://lum.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://dsn.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://anp.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bpo.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xlh.daxiang520.top

Java: x instanceof Number
来源：http://kql.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://plh.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://tbu.0kj1m.cn


<!-- 参考信息 -->