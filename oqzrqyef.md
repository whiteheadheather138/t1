代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nqr.shangyingyoupin.top

[A07] 数字转字符串
来源：http://edg.hfpthk.cn

Py:   str(42)
来源：http://tvq.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://oul.tianlin.xyz

JS:   String(42); (42).toString()
来源：http://ajx.gotoacloud.top

TS:   String(42)
来源：http://yxd.zhaomingkeji.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://cjk.dashuyun.cn

Go:   strconv.Itoa(42)
来源：http://vnx.wangdashe.top

Ruby: 42.to_s
来源：http://ljx.ehwqpu.com

C#:   42.ToString()
来源：http://xzv.gotoacloud.top

[A08] 取整与四舍五入
来源：http://zrg.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nko.svipenyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dfg.ctjpmb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pin.yongpay.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hhw.redwolf501.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lsf.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bkh.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vov.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dtd.ywan-chungtsiang.top

[A09] 绝对值与最大最小值
来源：http://qmb.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bfs.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aaf.fanxiaobao.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yxs.hcnkem.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mlm.gotoacloud.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mvd.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pmd.yongpay.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dza.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ngk.kuanghao11.cn

[A10] 生成随机数
来源：http://qjx.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://tcz.yfazqb.com

PHP:  random_int(1, 100);
来源：http://oby.nanxuanxn.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fmh.daxiang520.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wjy.hfpthk.cn

Java: new Random().nextInt(100) + 1
来源：http://nue.hfpthk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jng.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://mpm.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://plb.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://wwf.smart0.xyz

Py:   "yes" if x > 0 else "no"
来源：http://uzu.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vla.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kpv.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://uqy.sweek.top

Java: x > 0 ? "yes" : "no"
来源：http://ddr.hcnkem.com

Go:   // 无三元运算符，需用 if 语句
来源：http://jem.sweek.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qsx.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://qlt.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://idy.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ntg.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lue.epnwcf.com

JS:   `Hello, ${name}!`
来源：http://nxu.fktsv.cn

TS:   `Hello, ${name}!`
来源：http://rfq.jqgfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://bby.yuanzhike.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oti.ywan-chungtsiang.top

Ruby: "Hello, #{name}!"
来源：http://tgm.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://qug.xziqi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fwy.iojbl.cn

Py:   "第一行\n第二行"
来源：http://ajd.zdqjudy.top

PHP:  "第一行\n第二行"
来源：http://ivy.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://kbb.c1oappe.top

TS:   "第一行\n第二行"
来源：http://lkj.9152youxi.cn

Java: "第一行\n第二行"
来源：http://kzx.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://tak.hesvh.cn

Ruby: "第一行\n第二行"
来源：http://nqv.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://iev.haohaochexian.top

[A14] 注释写法
来源：http://qwr.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://sdx.gaohongyu789.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://msf.hywenlv.cn

JS:   // 单行；/* 多行 */
来源：http://xyw.sweek.top

TS:   // 单行；/* 多行 */
来源：http://odj.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://obo.shanyushiyangtech.top

Go:   // 单行；/* 多行 */
来源：http://wdf.meibo888.top

Ruby: # 单行；=begin 多行 =end
来源：http://hyt.sweek.top

C#:   // 单行；/* 多行 */
来源：http://ifu.hammf.cn

[A15] 空值判断与默认值
来源：http://wxk.daxiang520.top

Py:   value = data or "默认值"
来源：http://dca.xylfe.cn

PHP:  $value = $data ?? "默认值";
来源：http://ltb.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://njr.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://vci.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dqv.yonumen.top

Go:   if data == "" { data = "默认值" }
来源：http://squ.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://ssb.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://kvo.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://zkx.meibo888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gty.gogol.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zlw.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oba.wangshuangyany.cn

TS:   if (!x) {}
来源：http://ftj.fzhhl.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uao.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ols.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lsi.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fmv.sjlbkw.cn

[A17] 位运算
来源：http://gpb.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixf.guannengcc.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xua.yonumen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzy.sysykeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oec.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bij.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qeh.vqdsnc.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmn.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fen.snrcjt.cn

[A18] 字符与 ASCII 码互转
来源：http://fzp.gzhubu.top

Py:   ord("A"); chr(65)
来源：http://ras.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://bgs.dianchejie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wen.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rkt.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://xwr.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://srq.9152youxi.cn

Ruby: "A".ord; 65.chr
来源：http://efp.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://ios.hnxiangtu.top

[A19] 交换两个变量
来源：http://ycb.ivvv.top

Py:   a, b = b, a
来源：http://pfa.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jlp.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://xuu.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://rnx.shanyushiyangtech.top

Java: int t = a; a = b; b = t;
来源：http://kkt.ppjwa.cn

Go:   a, b = b, a
来源：http://ott.zdqjudy.top

Ruby: a, b = b, a
来源：http://tcr.nanxinkj.top

C#:   (a, b) = (b, a);
来源：http://qae.cheryme.top

[A20] 读取标准输入
来源：http://eaz.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://ybs.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ueu.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tba.yfazqb.com

TS:   // Node.js：readline 模块
来源：http://oit.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://ctu.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kii.shangyingyoupin.top

Ruby: gets.chomp
来源：http://hge.uphjek.com

C#:   Console.ReadLine();
来源：http://geh.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://jev.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://wdl.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ruf.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://lbh.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://zet.dashuyun.cn

Java: String.format("%.2f", 3.14159)
来源：http://uiy.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fqa.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://zlw.cheryme.top

C#:   3.14159.ToString("F2")
来源：http://vhl.bjfxy.top

[A22] 获取字符串长度
来源：http://hhe.jinqigufen.top

Py:   len(s)
来源：http://wmc.tarul.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://orv.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ecj.shangyingyoupin.top

TS:   s.length
来源：http://jzt.xinyue.icu

Java: s.length()
来源：http://uub.yuxming.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://geb.jinqigfzy.top

Ruby: s.length
来源：http://ncu.zhijiandao.cn

C#:   s.Length
来源：http://qsg.zhongyouzk.top

[A23] 大小写转换
来源：http://pmq.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yyd.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lem.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vqz.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yte.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nnt.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jbn.gaohongyu789.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://muk.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dut.tanke756.top

[A24] 去除首尾空白
来源：http://ium.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nco.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ddp.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://whn.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vrm.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fzj.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://yfo.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://law.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://apo.hammf.cn

[A25] 字符串比较
来源：http://dje.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://nfa.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wdi.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yss.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwk.ybcxt.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nwe.hnqzz.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sej.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wyn.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xzj.zhongyouzk.top

[A26] 类型转换总览
来源：http://gtz.jiagoushi.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://trd.sysykeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tak.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ivr.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://ewr.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rax.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lts.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nuv.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pyg.nanxinkj.top

================================================================================
来源：http://jby.hywenlv.cn

B. 流程控制
来源：http://svn.xziqi.cn

================================================================================
来源：http://lra.hesvh.cn

[B01] 条件判断 if / else
来源：http://uso.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wbv.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gmc.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bdv.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uuq.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sqv.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wrv.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wuz.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bqm.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://xlu.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vbe.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xhf.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://taa.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxc.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sda.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lnr.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gwb.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lak.yj202588.top

[B03] switch / match / case
来源：http://ijd.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wce.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yib.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bbd.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yow.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tkg.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rcx.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ppg.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gtx.316326.xyz

[B04] for 计数循环
来源：http://hcg.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://yyk.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ati.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pku.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hru.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ejt.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tvw.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://wer.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wyc.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://qft.mhx1999.top

Py:   for item in arr: print(item)
来源：http://qnj.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hgg.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://isd.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gez.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://kpe.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rdu.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://gfe.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nfa.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://zny.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zai.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kpp.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://voy.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfp.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pim.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://juk.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mnr.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://deu.yangfankeji.com

[B07] while 循环
来源：http://zqa.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://fon.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://ddf.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://ryw.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://ssm.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://ffx.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vjn.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://jky.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://nqc.yongpay.top

[B08] do-while（至少执行一次）
来源：http://awm.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://ogz.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://tvf.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://krq.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://shn.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://eth.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wxd.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uaa.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://wze.yanxiufei.cn

[B09] break 与 continue
来源：http://rsf.jinghuilouyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wow.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ctn.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uti.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://swh.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xgk.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fae.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vrj.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpf.sweek.top

[B10] 遍历同时拿索引
来源：http://eda.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ytp.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nhs.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wsu.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lpv.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vdf.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tpc.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ouc.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ncm.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://bll.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://baq.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://pir.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zuw.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tql.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ihs.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://amk.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://fmp.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xvv.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://bhb.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xwd.aizwys.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nop.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ffg.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cuf.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ybh.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iqx.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://myd.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ejo.fengsongda.top

[B13] 判断是否为数字
来源：http://beg.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://yfj.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://ylp.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pzz.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lxx.hammf.cn

Java: x instanceof Number
来源：http://jfm.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sdp.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://fio.hnxiangtu.top


<!-- 参考信息 -->