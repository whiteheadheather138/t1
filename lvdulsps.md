代发 wailian999

[A06] 字符串转数字
来源：http://tlc.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://xlo.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fuu.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hdi.wangdashe.top

TS:   parseInt("42", 10); Number("42")
来源：http://zxw.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ywa.sysykeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ibq.jiagoushi.top

Ruby: "42".to_i; "3.14".to_f
来源：http://grt.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kap.cucudq.cn

[A07] 数字转字符串
来源：http://zbh.ctjpmb.com

Py:   str(42)
来源：http://tne.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://nht.fktsv.cn

JS:   String(42); (42).toString()
来源：http://sao.c1oappe.top

TS:   String(42)
来源：http://nle.yangfankeji.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://jaa.zhixingplan.top

Go:   strconv.Itoa(42)
来源：http://ucr.sjlbkw.cn

Ruby: 42.to_s
来源：http://isw.ywan-chungtsiang.top

C#:   42.ToString()
来源：http://den.jinghuilouyu.cn

[A08] 取整与四舍五入
来源：http://dhn.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bjc.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://icc.jinyuanbaomall.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yky.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://umb.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uiz.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bxi.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://loz.bbcook.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mby.gzhubu.top

[A09] 绝对值与最大最小值
来源：http://pmc.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jmh.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wba.sysykeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://imt.pengpengdd.cyou

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ofm.vehdjk.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://otz.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uyo.ctjpmb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uwx.ppjwa.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ujs.yanxiufei.cn

[A10] 生成随机数
来源：http://ofh.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://xjk.shuidangran.top

PHP:  random_int(1, 100);
来源：http://wfi.hongshengwenyu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mdw.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kbf.aibaodan.cn

Java: new Random().nextInt(100) + 1
来源：http://hgg.zhoulong.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jvb.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://gso.daria6918.cn

C#:   new Random().Next(1, 101)
来源：http://vfd.zycfv.cn

[A11] 条件表达式（三元）
来源：http://ppi.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://wzd.yj20258.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://iip.cashguo.top

JS:   x > 0 ? "yes" : "no"
来源：http://mgq.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://nwq.nanxinkj.top

Java: x > 0 ? "yes" : "no"
来源：http://eae.yj20258.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yjy.jlsjyb.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://edq.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mfl.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://vah.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qzc.jyoumei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xjt.chenzaomai.com

JS:   `Hello, ${name}!`
来源：http://fgd.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://usj.shanyushiyangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://sly.cucudq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oxm.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://ppi.cheryme.top

C#:   $"Hello, {name}!"
来源：http://jrz.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oat.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://sey.gotoacloud.top

PHP:  "第一行\n第二行"
来源：http://lel.chenzaomai.com

JS:   "第一行\n第二行"
来源：http://vrc.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://bpi.ivvv.top

Java: "第一行\n第二行"
来源：http://wkh.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://qey.ybcxt.top

Ruby: "第一行\n第二行"
来源：http://pfv.jyoumei.cn

C#:   "第一行\n第二行"
来源：http://wrt.kuanghao11.cn

[A14] 注释写法
来源：http://jot.jinqigufen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lgl.fehbvm.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://ejq.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://atu.sysykeji.top

TS:   // 单行；/* 多行 */
来源：http://vae.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gpz.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://rhq.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://bbg.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://ltd.chenlongwang.top

[A15] 空值判断与默认值
来源：http://xaf.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://oue.bbcook.cn

PHP:  $value = $data ?? "默认值";
来源：http://lmi.tarul.cn

JS:   const value = data ?? "默认值";
来源：http://wbh.quarkkingdee.top

TS:   const value = data ?? "默认值";
来源：http://jjk.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xyb.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://yvf.svipenyu.cn

Ruby: value = data || "默认值"
来源：http://pev.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://sby.sufxvd.cn

[A16] 真假值判断规则
来源：http://hsd.sjlbkw.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://toy.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lgi.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fbe.jlsjyb.cn

TS:   if (!x) {}
来源：http://wvl.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vkt.yueranfly.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uea.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://oqx.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lva.smart0.xyz

[A17] 位运算
来源：http://gxk.hongshengwenyu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wra.yonumen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://njm.chenlongwang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sei.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nxx.dashuyun.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eum.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zce.redwolf501.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prz.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fty.gogol.net.cn

[A18] 字符与 ASCII 码互转
来源：http://ehv.yueranfly.top

Py:   ord("A"); chr(65)
来源：http://xjg.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://xqc.ywan-chungtsiang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pfj.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rtt.yj202588.top

Java: (int) 'A'; (char) 65
来源：http://hgo.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kch.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://yxp.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://cmx.aizwys.cn

[A19] 交换两个变量
来源：http://qyw.pycfn.com

Py:   a, b = b, a
来源：http://ybz.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ewl.shanyushiyangkeji.top

JS:   [a, b] = [b, a];
来源：http://tas.sysykeji.top

TS:   [a, b] = [b, a];
来源：http://ktl.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://kao.jinqigufen.top

Go:   a, b = b, a
来源：http://xwn.gaohongyu789.top

Ruby: a, b = b, a
来源：http://fne.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://rbn.yfazqb.com

[A20] 读取标准输入
来源：http://qkj.havefunace.top

Py:   name = input("请输入：")
来源：http://cyo.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wdr.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eho.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://yag.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://tdc.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vyv.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://jcs.jinqigufen.top

C#:   Console.ReadLine();
来源：http://zlv.c1oappe.top

[A21] 保留指定小数位输出
来源：http://ile.jinghuilouyu.cn

Py:   f"{3.14159:.2f}"
来源：http://mxj.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hde.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://hxb.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://fjo.yuanzhike.top

Java: String.format("%.2f", 3.14159)
来源：http://jpu.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://spw.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://wmu.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://flg.iojbl.cn

[A22] 获取字符串长度
来源：http://pcu.yj202588.top

Py:   len(s)
来源：http://mpv.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lyf.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://szv.bjfxy.top

TS:   s.length
来源：http://sft.hongshengwenyu.top

Java: s.length()
来源：http://ocz.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nsr.gotoacloud.top

Ruby: s.length
来源：http://wca.zycfv.cn

C#:   s.Length
来源：http://igk.aizwys.cn

[A23] 大小写转换
来源：http://teb.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sug.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vcd.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wly.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://byu.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sbi.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bxt.jinyuanbaomall.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qye.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jnq.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://iwk.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wsp.ydzc1.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://voi.yuxming.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lll.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jrv.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ycw.sweek.top

Go:   strings.TrimSpace(s)
来源：http://leu.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sau.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rvh.aizwys.cn

[A25] 字符串比较
来源：http://vth.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://sre.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vkb.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fgo.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ugr.yvedp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gpa.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tfh.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lsg.hfpthk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tho.xziqi.cn

[A26] 类型转换总览
来源：http://kit.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rll.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pig.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tii.epnwcf.com

TS:   Number() String() Boolean() x as number
来源：http://svn.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xlq.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pkv.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yev.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kwp.chenlongwang.top

================================================================================
来源：http://cpb.aizwys.cn

B. 流程控制
来源：http://jyz.havefunace.top

================================================================================
来源：http://pdq.daxiang520.top

[B01] 条件判断 if / else
来源：http://qjs.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xdp.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qyj.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yph.hywenlv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qlg.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xzi.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wvi.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xik.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gxq.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://jej.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mpc.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dno.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydn.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvg.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baj.yfazqb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ycz.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lii.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnk.tarul.cn

[B03] switch / match / case
来源：http://qzm.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ptz.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lvv.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xrk.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gjk.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://den.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vsq.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://avg.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zpc.zhongyouzk.top

[B04] for 计数循环
来源：http://uok.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://akj.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://won.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kga.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qrs.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tcd.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gib.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://pew.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ejd.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://ohr.yj20258.top

Py:   for item in arr: print(item)
来源：http://wqi.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lcv.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gxg.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://msr.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://uaf.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://edq.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://bld.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://plw.yonumen.top

[B06] 遍历字典 / 对象
来源：http://vkf.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kgu.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qys.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bsh.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xxr.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jsp.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xsa.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://neh.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sna.yangfankeji.com

[B07] while 循环
来源：http://bmh.bjfxy.top

Py:   while i < 10: i += 1
来源：http://gjf.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://lct.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://vpi.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://kgc.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://jlg.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kdc.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://viv.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://yyn.birdmap.top

[B08] do-while（至少执行一次）
来源：http://hqy.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://oxh.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aek.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://xqo.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://cjf.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://yrh.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nso.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://qaw.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://snb.guowangkeji.top

[B09] break 与 continue
来源：http://sxb.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hod.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hjq.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sek.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mky.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtz.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rym.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kgo.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rbo.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://rvh.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dhn.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zel.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jpg.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qsn.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oqa.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://scl.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lta.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://moh.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://lwh.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://rwy.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://elh.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pff.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqu.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hwd.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lyv.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://hzn.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://umc.gzhubu.top

[B12] 跳出多层循环
来源：http://wqp.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ldl.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://urr.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wyj.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ktk.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rwb.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://anv.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nev.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://swo.9152youxi.cn


<!-- 参考信息 -->