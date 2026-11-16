代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mck.zhengqikj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kpi.bbcook.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://avi.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://rmq.fengsongda.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rou.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://umn.havefunace.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jcl.jqgfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vsr.bjfxy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nym.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bqp.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gkl.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ujj.tian-w.cn

[A10] 生成随机数
来源：http://ijt.52xcode.cn

Py:   import random; random.randint(1, 100)
来源：http://fad.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://swb.jqgfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gbr.redwolf501.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uml.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://zhv.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xoe.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://rvk.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://tsw.shuidangran.top

[A11] 条件表达式（三元）
来源：http://owa.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://pjb.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://vyb.gaohongyu789.top

JS:   x > 0 ? "yes" : "no"
来源：http://kcb.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://xfa.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://azu.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hbb.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kmf.fanxiaobao.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://akb.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://utf.yangfankeji.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nrh.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jvk.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://wha.jinqigfzy.top

TS:   `Hello, ${name}!`
来源：http://kee.yj202588.top

Java: "Hello, %s!".formatted(name)
来源：http://gvn.gzhubu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aey.gaohongyu789.top

Ruby: "Hello, #{name}!"
来源：http://hnf.ivvv.top

C#:   $"Hello, {name}!"
来源：http://atd.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://adq.yueranfly.top

Py:   "第一行\n第二行"
来源：http://gsr.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://rtu.jqgufenzy.top

JS:   "第一行\n第二行"
来源：http://yyw.xylfe.cn

TS:   "第一行\n第二行"
来源：http://mdq.ppjwa.cn

Java: "第一行\n第二行"
来源：http://hvq.sysykeji.top

Go:   "第一行\n第二行"
来源：http://pii.shanyushiyangtech.top

Ruby: "第一行\n第二行"
来源：http://oho.tanke756.top

C#:   "第一行\n第二行"
来源：http://fvk.aizwys.cn

[A14] 注释写法
来源：http://nwf.quarkkingdee.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hoj.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fja.gzhubu.top

JS:   // 单行；/* 多行 */
来源：http://qtn.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://rcd.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wib.wangdashe.top

Go:   // 单行；/* 多行 */
来源：http://vld.ehwqpu.com

Ruby: # 单行；=begin 多行 =end
来源：http://kgv.hammf.cn

C#:   // 单行；/* 多行 */
来源：http://gin.xinyue.icu

[A15] 空值判断与默认值
来源：http://ham.jinqigufen.top

Py:   value = data or "默认值"
来源：http://kqq.cdnleiting.top

PHP:  $value = $data ?? "默认值";
来源：http://ijf.zdqjudy.top

JS:   const value = data ?? "默认值";
来源：http://plg.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://elj.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://axu.sjlbkw.cn

Go:   if data == "" { data = "默认值" }
来源：http://wnr.fktsv.cn

Ruby: value = data || "默认值"
来源：http://lkl.dianchejie.cn

C#:   var value = data ?? "默认值";
来源：http://eyf.wangdashe.top

[A16] 真假值判断规则
来源：http://hnb.gaohongyu789.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://aaa.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zkp.jinqigfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iqc.0kj1m.cn

TS:   if (!x) {}
来源：http://qhf.fehbvm.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://txl.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lrk.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://mhl.yuanzhike.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bjf.zhengqikj.top

[A17] 位运算
来源：http://gfd.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jsa.yuxming.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://otj.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ltu.dianchejie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hwf.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lnv.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sez.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdv.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://krz.ydzc1.top

[A18] 字符与 ASCII 码互转
来源：http://lkd.vqdsnc.cn

Py:   ord("A"); chr(65)
来源：http://iag.vehdjk.com

PHP:  ord("A"); chr(65)
来源：http://ffv.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ilu.sufxvd.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ouf.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://zlk.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dst.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://qfi.jinghuilouyu.cn

C#:   (int)'A'; (char)65
来源：http://vxg.tanke756.top

[A19] 交换两个变量
来源：http://vwn.fanxiaobao.xyz

Py:   a, b = b, a
来源：http://sla.zhoulong.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://aqi.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://wro.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://mcs.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://ixw.zhiwuduotai.top

Go:   a, b = b, a
来源：http://ars.yuxming.cn

Ruby: a, b = b, a
来源：http://gnq.jinqigufen.top

C#:   (a, b) = (b, a);
来源：http://ucg.bjfxy.top

[A20] 读取标准输入
来源：http://svw.fzhhl.top

Py:   name = input("请输入：")
来源：http://gyf.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ceo.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uuw.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://igz.52xcode.cn

Java: new Scanner(System.in).nextLine()
来源：http://mwi.jianghu66.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://flk.0kj1m.cn

Ruby: gets.chomp
来源：http://itd.jqgfzy.top

C#:   Console.ReadLine();
来源：http://sfg.yj202588.top

[A21] 保留指定小数位输出
来源：http://rlf.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://ndt.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ktm.mhx1999.top

JS:   (3.14159).toFixed(2)
来源：http://zzj.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://zob.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://giz.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sce.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://uaa.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://exb.jlsjyb.cn

[A22] 获取字符串长度
来源：http://qqs.tarul.cn

Py:   len(s)
来源：http://vvn.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vza.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kht.jqgufenzy.top

TS:   s.length
来源：http://sjf.bbcook.cn

Java: s.length()
来源：http://vgc.pycfn.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ooc.havefunace.top

Ruby: s.length
来源：http://ymf.meibo888.top

C#:   s.Length
来源：http://clb.pengpengdd.cyou

[A23] 大小写转换
来源：http://bwp.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://aax.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uvl.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kuv.yanxiufei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pue.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awq.chenzaomai.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rmj.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lnf.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wsx.yj202588.top

[A24] 去除首尾空白
来源：http://ymo.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ybv.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jxg.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vvd.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yrx.snrcjt.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vjb.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://eso.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hcm.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ngr.vqdsnc.cn

[A25] 字符串比较
来源：http://nhg.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://vbq.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kku.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ldp.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://guz.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qpg.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dff.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rvb.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zjt.hesvh.cn

[A26] 类型转换总览
来源：http://uno.zhengqikj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://erb.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ulu.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://swb.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://ijk.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mnb.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dqu.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mug.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vhq.yuanzhike.top

================================================================================
来源：http://kup.chenzaomai.com

B. 流程控制
来源：http://wut.fzhhl.top

================================================================================
来源：http://uut.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://hmq.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yqj.wangdashe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rxl.jinyuanbaomall.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vaf.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ioy.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yks.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nsj.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uar.zhiwuduotai.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lop.mhx1999.top

[B02] 多分支 else if / elif
来源：http://ucg.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hyp.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://swd.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpl.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klg.guannengcc.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zkb.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lgb.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xuq.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fok.hammf.cn

[B03] switch / match / case
来源：http://hpc.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ohh.jinyuanbaomall.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://svl.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dwb.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fty.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qnb.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xby.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yte.zdqjudy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zij.guannengcc.top

[B04] for 计数循环
来源：http://laf.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://pht.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rpo.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bhj.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pll.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zkz.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://akt.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://jmk.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jmz.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://wbb.ydzc1.top

Py:   for item in arr: print(item)
来源：http://xpq.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cwz.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rik.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yzw.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jwa.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tdd.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://hec.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hia.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://hre.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yjb.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fho.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lqx.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uvj.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oxj.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wou.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qno.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lhu.pycfn.com

[B07] while 循环
来源：http://ptw.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://yks.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://etg.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://ovg.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://dzo.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://dgc.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nnh.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://dpi.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://nmf.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://kif.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://ftb.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://czs.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://ugr.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://usb.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://ext.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mcu.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://xco.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://rtb.xziqi.cn

[B09] break 与 continue
来源：http://jlw.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nzn.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ocr.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzf.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rkr.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kes.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cat.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gjv.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fai.birdmap.top

[B10] 遍历同时拿索引
来源：http://jxo.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://okw.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ixf.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vyh.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://div.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ivf.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nfw.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fxc.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kpr.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://ccg.316326.xyz

Py:   list(range(0, 10, 2))
来源：http://pjo.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://qqi.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rfd.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://koy.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://djy.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ryh.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://zyh.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hvq.haohaochexian.top

[B12] 跳出多层循环
来源：http://zzy.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cfp.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ddu.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lro.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ith.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uai.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ygq.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xen.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mzj.cheryme.top

[B13] 判断是否为数字
来源：http://zrh.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://kyn.hnqzz.top

PHP:  is_numeric($x)
来源：http://huw.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vle.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbp.sweek.top

Java: x instanceof Number
来源：http://twf.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ncj.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://jtj.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://awf.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://ivq.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://apa.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wgv.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://rfy.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://vul.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nph.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cjp.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dvt.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xdi.ivvv.top

[B15] 布尔运算与取反
来源：http://pgw.ydjk.org.cn

Py:   a and b or not c
来源：http://ang.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://azc.xylfe.cn

JS:   a && b || !c
来源：http://fxz.zhijiandao.cn

TS:   a && b || !c
来源：http://xqp.0kj1m.cn

Java: a && b || !c
来源：http://brr.vqdsnc.cn


<!-- 参考信息 -->