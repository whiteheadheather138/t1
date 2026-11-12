代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://hxh.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rmq.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sid.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rmk.hammf.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iuy.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://sim.shanyushiyangtech.top

Py:   str(42)
来源：http://qxb.0kj1m.cn

PHP:  (string) 42; strval(42)
来源：http://edh.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://dxp.ppjwa.cn

TS:   String(42)
来源：http://wwy.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fzv.zhongyouzk.top

Go:   strconv.Itoa(42)
来源：http://djh.jinqigfzy.top

Ruby: 42.to_s
来源：http://yyr.cqqwz.cn

C#:   42.ToString()
来源：http://gpu.zdbjq.cn

[A08] 取整与四舍五入
来源：http://nku.nwbrower.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lsh.nanxuanxn.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://got.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kuw.vehdjk.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://but.zhengqikj.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rlm.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ewc.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vny.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pjo.tarul.cn

[A09] 绝对值与最大最小值
来源：http://phk.nwbrower.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nlj.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lkb.iojbl.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cap.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qxz.sxryk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hoa.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iai.jqgufenzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rpq.xylfe.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://njt.9152youxi.cn

[A10] 生成随机数
来源：http://oog.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://iaz.vqdsnc.cn

PHP:  random_int(1, 100);
来源：http://otp.hcnkem.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ius.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fus.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://ymr.smart0.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fgk.shzxlz.cn

Ruby: rand(1..100)
来源：http://mwj.zhiwuduotai.top

C#:   new Random().Next(1, 101)
来源：http://pee.ybcxt.top

[A11] 条件表达式（三元）
来源：http://wun.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://lcp.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jgn.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hwr.bbcook.cn

TS:   x > 0 ? "yes" : "no"
来源：http://phe.yuxming.cn

Java: x > 0 ? "yes" : "no"
来源：http://cyq.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uql.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://toj.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://zqy.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://iff.xuanzx.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rbg.svipenyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yek.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://jqp.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://wdm.shanyushiyangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://vhk.gzhubu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xks.ctjpmb.com

Ruby: "Hello, #{name}!"
来源：http://ypq.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://sjt.cheryme.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ldd.ppjwa.cn

Py:   "第一行\n第二行"
来源：http://dub.yongpay.top

PHP:  "第一行\n第二行"
来源：http://knr.shuidangran.top

JS:   "第一行\n第二行"
来源：http://rto.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://puz.sxryk.cn

Java: "第一行\n第二行"
来源：http://tgt.zhoulong.xyz

Go:   "第一行\n第二行"
来源：http://vsr.ctjpmb.com

Ruby: "第一行\n第二行"
来源：http://ftw.hfpthk.cn

C#:   "第一行\n第二行"
来源：http://xgu.hesvh.cn

[A14] 注释写法
来源：http://kiy.epnwcf.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://pxh.yj20258888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kfz.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://sok.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://qti.nwbrower.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gud.yj202588.top

Go:   // 单行；/* 多行 */
来源：http://rko.xylfe.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jpv.yonumen.top

C#:   // 单行；/* 多行 */
来源：http://wst.316326.xyz

[A15] 空值判断与默认值
来源：http://ien.fengsongda.top

Py:   value = data or "默认值"
来源：http://oax.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://fhv.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://kjw.316326.xyz

TS:   const value = data ?? "默认值";
来源：http://nhj.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oqo.zhaomingkeji.xyz

Go:   if data == "" { data = "默认值" }
来源：http://dqu.yfazqb.com

Ruby: value = data || "默认值"
来源：http://dln.pycfn.com

C#:   var value = data ?? "默认值";
来源：http://gjm.yfazqb.com

[A16] 真假值判断规则
来源：http://swg.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tmk.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://git.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jql.nwbrower.top

TS:   if (!x) {}
来源：http://ynz.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://joh.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ojw.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://hcu.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jbo.0kj1m.cn

[A17] 位运算
来源：http://obc.gaohongyu789.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://byd.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dil.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bif.snrcjt.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xxv.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vkw.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pkj.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sdx.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jcs.xziqi.cn

[A18] 字符与 ASCII 码互转
来源：http://ljf.sweek.top

Py:   ord("A"); chr(65)
来源：http://hzy.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://fzv.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oke.cheryme.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mva.nanxuanxn.top

Java: (int) 'A'; (char) 65
来源：http://jdh.meibo888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wvt.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://nhe.smart0.xyz

C#:   (int)'A'; (char)65
来源：http://pce.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://dpv.yuxming.cn

Py:   a, b = b, a
来源：http://yca.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qkm.chenzaomai.com

JS:   [a, b] = [b, a];
来源：http://puv.cashguo.top

TS:   [a, b] = [b, a];
来源：http://zfi.shzxlz.cn

Java: int t = a; a = b; b = t;
来源：http://tzy.9152youxi.cn

Go:   a, b = b, a
来源：http://ddx.chenlongwang.top

Ruby: a, b = b, a
来源：http://msr.feifeiyinyue.top

C#:   (a, b) = (b, a);
来源：http://fed.iojbl.cn

[A20] 读取标准输入
来源：http://nou.yangfankeji.com

Py:   name = input("请输入：")
来源：http://gsu.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://csv.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rlb.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://jwa.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://xao.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://naq.birdmap.top

Ruby: gets.chomp
来源：http://nqi.wangdashe.top

C#:   Console.ReadLine();
来源：http://qbc.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://oii.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://tub.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://efu.shangyingyoupin.top

JS:   (3.14159).toFixed(2)
来源：http://bnu.cheryme.top

TS:   (3.14159).toFixed(2)
来源：http://yhd.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://ses.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://flz.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://loc.daria6918.cn

C#:   3.14159.ToString("F2")
来源：http://xfw.fehbvm.com

[A22] 获取字符串长度
来源：http://zpt.jiagoushi.top

Py:   len(s)
来源：http://ifu.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rpy.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oku.quarkkingdee.top

TS:   s.length
来源：http://lkq.haohaochexian.top

Java: s.length()
来源：http://jel.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dzz.quarkkingdee.top

Ruby: s.length
来源：http://rln.9152youxi.cn

C#:   s.Length
来源：http://thj.daxiang520.top

[A23] 大小写转换
来源：http://qqn.zhongyouzk.top

Py:   s.upper(); s.lower(); s.title()
来源：http://viw.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qfc.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://spa.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ukp.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bhh.xuanzx.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lqv.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ock.yj202588.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ijb.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://mlu.jinqigufen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qzi.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aaw.cucudq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pjq.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jki.yonumen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gjx.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://rrr.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lxd.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mst.hnqzz.top

[A25] 字符串比较
来源：http://ljw.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://qfy.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hot.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lcw.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sae.yanxiufei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lkf.jinghuilouyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wcg.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://een.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jnp.zycfv.cn

[A26] 类型转换总览
来源：http://yax.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xem.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uuo.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sab.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://ymy.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ukr.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hlj.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pga.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pvp.zhaomingkeji.xyz

================================================================================
来源：http://byu.daxiang520.top

B. 流程控制
来源：http://qby.chenjidiqi.icu

================================================================================
来源：http://vij.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://dzz.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fse.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://exm.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fnu.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hgl.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://naj.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tld.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mpi.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://njg.fktsv.cn

[B02] 多分支 else if / elif
来源：http://jae.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bnn.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gsd.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkf.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyg.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzx.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hxp.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rzb.yonumen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://coi.shangyingyoupin.top

[B03] switch / match / case
来源：http://osc.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://esb.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dct.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mja.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tst.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://atq.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fji.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ivs.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uxj.ybcxt.top

[B04] for 计数循环
来源：http://ddk.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://tde.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zrf.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wnw.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wus.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ygd.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vfe.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://axk.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cax.sweek.top

[B05] 遍历数组 / 列表
来源：http://nak.jianghu66.top

Py:   for item in arr: print(item)
来源：http://dxs.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ytj.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rqe.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dcr.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://byi.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bsi.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://sjt.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://epw.yonumen.top

[B06] 遍历字典 / 对象
来源：http://mfq.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ugw.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nzt.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jvt.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qrp.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tma.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rgz.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pcp.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xlz.uphjek.com

[B07] while 循环
来源：http://rhp.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://lbv.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://qcd.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://mkq.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://gpf.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://vmm.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://odb.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://uhy.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://xmm.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://nlb.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://ofr.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xri.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://ers.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://nrh.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://vci.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://slb.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://oai.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://duq.hammf.cn

[B09] break 与 continue
来源：http://lbk.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ewc.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qdl.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sno.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rzd.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kad.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://olv.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mks.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czs.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://aql.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lrd.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wof.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://arf.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ooo.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hqh.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zto.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ejr.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gyr.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://eqh.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://wsi.cheryme.top

PHP:  range(0, 10, 2);
来源：http://qwm.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jht.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wfn.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dnp.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lro.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://ynv.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ojj.xziqi.cn

[B12] 跳出多层循环
来源：http://ndk.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://rlm.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uae.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wxy.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ybc.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hji.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tfm.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqj.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://drr.dianchejie.cn

[B13] 判断是否为数字
来源：http://lbh.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://ejh.cucudq.cn

PHP:  is_numeric($x)
来源：http://stf.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tis.zhengqikj.top


<!-- 参考信息 -->