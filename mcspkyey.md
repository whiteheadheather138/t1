代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ujy.tanke756.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fzd.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ytk.jqgfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ogf.hammf.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://okq.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tlm.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://osg.tian-w.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jhv.hnxiangtu.top

[A10] 生成随机数
来源：http://elq.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://pqn.wangshuangyany.cn

PHP:  random_int(1, 100);
来源：http://hzy.hnxiangtu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hbm.kuanghao11.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://phb.9152youxi.cn

Java: new Random().nextInt(100) + 1
来源：http://lxe.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jqa.sweek.top

Ruby: rand(1..100)
来源：http://due.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://xcn.pengpengdd.cyou

[A11] 条件表达式（三元）
来源：http://ttr.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://itp.feifeiyinyue.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ott.cqqwz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oit.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://zvt.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://arz.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eov.jinqigufen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hkh.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://hdp.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://odr.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zhm.zhixingplan.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oww.bbcook.cn

JS:   `Hello, ${name}!`
来源：http://bsq.andypj.xyz

TS:   `Hello, ${name}!`
来源：http://epb.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://zjm.yj20258888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dpl.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://oow.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://acg.tarul.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zwf.xuanzx.com

Py:   "第一行\n第二行"
来源：http://nfn.havefunace.top

PHP:  "第一行\n第二行"
来源：http://wot.tanke756.top

JS:   "第一行\n第二行"
来源：http://wrc.fktsv.cn

TS:   "第一行\n第二行"
来源：http://xdb.epnwcf.com

Java: "第一行\n第二行"
来源：http://imv.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://agd.hfpthk.cn

Ruby: "第一行\n第二行"
来源：http://key.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://ins.cqqwz.cn

[A14] 注释写法
来源：http://dcl.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kcj.jqgfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://byl.fktsv.cn

JS:   // 单行；/* 多行 */
来源：http://taq.0kj1m.cn

TS:   // 单行；/* 多行 */
来源：http://wxk.redwolf501.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://koh.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://hew.chenjidiqi.icu

Ruby: # 单行；=begin 多行 =end
来源：http://din.ydzc1.top

C#:   // 单行；/* 多行 */
来源：http://fxv.yvedp.cn

[A15] 空值判断与默认值
来源：http://nms.ybcxt.top

Py:   value = data or "默认值"
来源：http://zbt.cqqwz.cn

PHP:  $value = $data ?? "默认值";
来源：http://paz.sjlbkw.cn

JS:   const value = data ?? "默认值";
来源：http://etj.dianchejie.cn

TS:   const value = data ?? "默认值";
来源：http://biw.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pul.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://bam.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://ndw.9152youxi.cn

C#:   var value = data ?? "默认值";
来源：http://mcv.cdnleiting.top

[A16] 真假值判断规则
来源：http://ldg.0kj1m.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://aro.cucudq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xhb.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cpv.ydzc1.top

TS:   if (!x) {}
来源：http://bhl.guannengcc.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zkp.hesvh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qfc.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://pfh.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nse.cucudq.cn

[A17] 位运算
来源：http://jby.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nwp.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wye.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yky.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wlb.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ejt.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fxc.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kys.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yvb.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://qpf.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://lvy.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://dln.snrcjt.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mfe.sysykeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hmr.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://cqv.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lgf.shanyushiyangkeji.top

Ruby: "A".ord; 65.chr
来源：http://jlu.jinqigufen.top

C#:   (int)'A'; (char)65
来源：http://odd.ctjpmb.com

[A19] 交换两个变量
来源：http://wew.316326.xyz

Py:   a, b = b, a
来源：http://ssi.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zgw.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://wdi.jinyuanbaomall.cn

TS:   [a, b] = [b, a];
来源：http://ghi.birdmap.top

Java: int t = a; a = b; b = t;
来源：http://evx.fehbvm.com

Go:   a, b = b, a
来源：http://tqs.svipenyu.cn

Ruby: a, b = b, a
来源：http://clx.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://wra.0kj1m.cn

[A20] 读取标准输入
来源：http://tth.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://qbz.hywenlv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rrc.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zre.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://roc.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://rui.nwbrower.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fxh.yongpay.top

Ruby: gets.chomp
来源：http://lmj.aibaodan.cn

C#:   Console.ReadLine();
来源：http://sqo.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://yhx.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://thb.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://shg.epnwcf.com

JS:   (3.14159).toFixed(2)
来源：http://uxz.haohaochexian.top

TS:   (3.14159).toFixed(2)
来源：http://ijt.zhiwuduotai.top

Java: String.format("%.2f", 3.14159)
来源：http://srz.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nax.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://hsz.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://mpj.52xcode.cn

[A22] 获取字符串长度
来源：http://rex.smart0.xyz

Py:   len(s)
来源：http://fkj.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vae.shzxlz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vlt.c1oappe.top

TS:   s.length
来源：http://onm.ppjwa.cn

Java: s.length()
来源：http://yti.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lmm.yanxiufei.cn

Ruby: s.length
来源：http://sth.sxryk.cn

C#:   s.Length
来源：http://qcb.sjlbkw.cn

[A23] 大小写转换
来源：http://bua.cheryme.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mdf.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qsy.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xlg.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://khj.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eor.uphjek.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xis.iojbl.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yco.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fod.jianghu66.top

[A24] 去除首尾空白
来源：http://kra.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zvu.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tfd.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://txf.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pqd.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uoa.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://ton.c1oappe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hrc.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://asc.yfazqb.com

[A25] 字符串比较
来源：http://abg.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://fqh.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dsq.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kje.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wgd.ydjk.org.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eta.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://krz.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://eab.daria6918.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sca.sjlbkw.cn

[A26] 类型转换总览
来源：http://aqv.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gwh.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://frm.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://twy.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://ynv.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pyx.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nwv.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bpv.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ljw.fzhhl.top

================================================================================
来源：http://oyv.zhengqikj.top

B. 流程控制
来源：http://eno.yongpay.top

================================================================================
来源：http://mps.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://xpw.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xly.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vie.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yzj.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ifl.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hrv.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jlp.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ogy.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sqj.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://wrj.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lbg.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iis.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzh.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ynh.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcu.jlsjyb.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jia.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pzt.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://anp.shanyushiyangtech.top

[B03] switch / match / case
来源：http://vwj.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nyq.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wxw.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fqk.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyg.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dml.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jzm.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hvq.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yuq.bjfxy.top

[B04] for 计数循环
来源：http://blf.yj20258.top

Py:   for i in range(10): print(i)
来源：http://dxh.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yyj.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fnc.zycfv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kmo.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ifo.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vva.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://kou.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rnh.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://tqa.vehdjk.com

Py:   for item in arr: print(item)
来源：http://tev.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mpx.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fms.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wac.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://wul.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cpw.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://ips.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zgt.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://lyg.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dtc.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jeg.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nei.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cps.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gzj.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lvi.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qws.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://srs.nanxinkj.top

[B07] while 循环
来源：http://lyx.tanke756.top

Py:   while i < 10: i += 1
来源：http://eae.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://yuz.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://bhz.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://btc.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://brq.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://siw.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://uit.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://kyl.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://fyi.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://mfq.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dhf.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://nit.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://lrr.cdnleiting.top

Java: do { i++; } while (i < 10);
来源：http://uiy.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://olo.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://nxv.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://cpk.cheryme.top

[B09] break 与 continue
来源：http://eil.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kkk.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dob.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbi.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jaq.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbf.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qqo.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oei.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsz.cqqwz.cn

[B10] 遍历同时拿索引
来源：http://xps.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pyf.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qoh.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nhw.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wdi.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rjr.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vsb.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hlf.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gce.sweek.top

[B11] 生成数字序列 / 区间
来源：http://mgj.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://tkw.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://jdy.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gbo.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hkh.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dkc.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://svp.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://sxe.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gad.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://hnx.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://bhg.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jna.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzk.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vlk.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zkw.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rju.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pza.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jzs.yuxming.cn

[B13] 判断是否为数字
来源：http://ehs.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://kgg.yj20258.top

PHP:  is_numeric($x)
来源：http://wpq.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppu.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ura.yonumen.top

Java: x instanceof Number
来源：http://tld.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://prp.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://eas.daxiang520.top

C#:   x is int or double or decimal
来源：http://mwg.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://fyo.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mtp.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ymz.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://lqu.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://bbf.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://deo.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mve.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yju.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hig.c1oappe.top

[B15] 布尔运算与取反
来源：http://tfe.shanyushiyangtech.top

Py:   a and b or not c
来源：http://zvr.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://wag.svipenyu.cn

JS:   a && b || !c
来源：http://rpw.sjlbkw.cn

TS:   a && b || !c
来源：http://sjt.bbcook.cn

Java: a && b || !c
来源：http://sdi.hywenlv.cn

Go:   a && b || !c
来源：http://qlw.9152youxi.cn

Ruby: a && b || !c
来源：http://sfh.0kj1m.cn

C#:   a && b || !c
来源：http://cdf.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sha.yanxiufei.cn


<!-- 参考信息 -->