代发 wailian999

Ruby: 42.to_s
来源：http://jqw.ctjpmb.com

C#:   42.ToString()
来源：http://kup.xylfe.cn

[A08] 取整与四舍五入
来源：http://maz.daxiang520.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rui.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yra.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nhu.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://twh.xinyue.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ffb.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wpu.sjlbkw.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wup.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jfv.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://knt.quarkkingdee.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eek.daxiang520.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aha.hongshengwenyu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bcy.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kyc.sufxvd.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hae.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mun.hnqzz.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wlh.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zyt.gaohongyu789.top

[A10] 生成随机数
来源：http://dxh.jinqigfzy.top

Py:   import random; random.randint(1, 100)
来源：http://xda.fktsv.cn

PHP:  random_int(1, 100);
来源：http://gmu.zhengqikj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bbk.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rxn.vqdsnc.cn

Java: new Random().nextInt(100) + 1
来源：http://rha.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ywj.xingfuxueyuan.xyz

Ruby: rand(1..100)
来源：http://mdj.0kj1m.cn

C#:   new Random().Next(1, 101)
来源：http://gso.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://hyz.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://gyh.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://rit.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://cuk.jqgufenzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://mfo.sjlbkw.cn

Java: x > 0 ? "yes" : "no"
来源：http://bqo.fktsv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lov.meibo888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://lsw.uphjek.com

C#:   x > 0 ? "yes" : "no"
来源：http://xek.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://lqg.jlsjyb.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vsf.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sua.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://fpf.jyoumei.cn

TS:   `Hello, ${name}!`
来源：http://fpi.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://qmn.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kls.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://gzl.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://gke.hysaishi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://edl.jinqigufen.top

Py:   "第一行\n第二行"
来源：http://kpj.fehbvm.com

PHP:  "第一行\n第二行"
来源：http://ust.c1oappe.top

JS:   "第一行\n第二行"
来源：http://lza.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://grd.yongpay.top

Java: "第一行\n第二行"
来源：http://pbt.epnwcf.com

Go:   "第一行\n第二行"
来源：http://jus.jinghuilouyu.cn

Ruby: "第一行\n第二行"
来源：http://kdo.birdmap.top

C#:   "第一行\n第二行"
来源：http://fnu.zhijiandao.cn

[A14] 注释写法
来源：http://heb.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tea.cashguo.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ouy.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://mbc.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://fon.fzhhl.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://man.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://xqc.shzxlz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cli.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://lpv.ydzc1.top

[A15] 空值判断与默认值
来源：http://ijp.zhongyouzk.top

Py:   value = data or "默认值"
来源：http://txn.smart0.xyz

PHP:  $value = $data ?? "默认值";
来源：http://fme.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://thk.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://tgu.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sue.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://mvs.yj202588.top

Ruby: value = data || "默认值"
来源：http://juj.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://huv.zhixingplan.top

[A16] 真假值判断规则
来源：http://cpy.yongpay.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wjz.sweek.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bnh.chenjidiqi.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ajd.jianghu66.top

TS:   if (!x) {}
来源：http://hqo.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xqp.jiagoushi.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jen.ctjpmb.com

Ruby: unless x            # nil 与 false 为假
来源：http://bwa.hcnkem.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wfo.shanyushiyangkeji.top

[A17] 位运算
来源：http://wce.yj20258888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yjk.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qvl.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvx.fktsv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lyd.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zft.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kpn.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ynm.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ihq.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://ftf.uphjek.com

Py:   ord("A"); chr(65)
来源：http://yyo.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://jzg.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://npu.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cyu.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://ecn.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qeo.uphjek.com

Ruby: "A".ord; 65.chr
来源：http://yxn.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://efs.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://skg.xziqi.cn

Py:   a, b = b, a
来源：http://gws.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://iqc.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://tfl.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://iyz.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://gkw.c1oappe.top

Go:   a, b = b, a
来源：http://qxk.birdmap.top

Ruby: a, b = b, a
来源：http://wvm.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://nut.redwolf501.top

[A20] 读取标准输入
来源：http://oqv.xuetiantiany.cn

Py:   name = input("请输入：")
来源：http://kux.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wyk.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lxw.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://ujp.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://krc.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uxy.c1oappe.top

Ruby: gets.chomp
来源：http://bkv.yuxming.cn

C#:   Console.ReadLine();
来源：http://vlr.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://pmi.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://zos.wangshuangyany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gyj.zycfv.cn

JS:   (3.14159).toFixed(2)
来源：http://com.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://qeb.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://ubd.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kzz.nwbrower.top

Ruby: format("%.2f", 3.14159)
来源：http://nqq.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://kvg.gogol.net.cn

[A22] 获取字符串长度
来源：http://ijx.316326.xyz

Py:   len(s)
来源：http://sqn.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://glh.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eem.shuidangran.top

TS:   s.length
来源：http://ytu.yongpay.top

Java: s.length()
来源：http://swg.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bum.316326.xyz

Ruby: s.length
来源：http://kcv.fzhhl.top

C#:   s.Length
来源：http://cye.feifeiyinyue.top

[A23] 大小写转换
来源：http://gzy.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kan.cucudq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vod.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kdw.jqgfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ona.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zbe.yanxiufei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wdi.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ojg.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qej.sxryk.cn

[A24] 去除首尾空白
来源：http://qyu.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zny.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fdv.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tcq.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bag.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://chm.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://kky.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cen.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ksr.jqgfzy.top

[A25] 字符串比较
来源：http://hkf.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://abj.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jiv.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://urx.jqgufenzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://evi.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dsb.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ler.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://fuh.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://euw.vqdsnc.cn

[A26] 类型转换总览
来源：http://hwk.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://myp.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ahn.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cvr.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://ejn.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lao.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rrz.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hsm.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://egx.gaohongyu789.top

================================================================================
来源：http://mlj.jqgufenzy.top

B. 流程控制
来源：http://sld.feifeiyinyue.top

================================================================================
来源：http://fak.zhixingplan.top

[B01] 条件判断 if / else
来源：http://yvf.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cob.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oka.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zxq.zycfv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ltp.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://srn.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gsf.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uon.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nya.zhijiandao.cn

[B02] 多分支 else if / elif
来源：http://oxx.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dls.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xnv.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzl.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nhx.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://toz.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jec.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lni.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hbt.zhengqikj.top

[B03] switch / match / case
来源：http://hof.cheryme.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vur.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bdk.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sxs.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mxd.cqqwz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://skv.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aiw.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fdu.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nbp.chenlongwang.top

[B04] for 计数循环
来源：http://aca.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://fgn.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ofp.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://taa.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rxb.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://duc.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pyw.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://xpn.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cyb.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://kdw.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://aaa.ivvv.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sus.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eit.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tly.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yox.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wdf.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://kpq.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://edz.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://xqb.pycfn.com

Py:   for k, v in d.items(): print(k, v)
来源：http://znr.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cng.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nof.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqr.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uea.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jnl.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vkx.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://twg.hongshengwenyu.top

[B07] while 循环
来源：http://ask.guannengcc.top

Py:   while i < 10: i += 1
来源：http://jfj.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://bmn.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://apo.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://rwm.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://jdw.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://upp.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://wbm.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://fat.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://xps.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://nze.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uax.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://lng.fzhhl.top

TS:   do { i++; } while (i < 10);
来源：http://eef.yonumen.top

Java: do { i++; } while (i < 10);
来源：http://dcm.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://czl.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://nza.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://nkc.dianchejie.cn

[B09] break 与 continue
来源：http://yxn.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kkh.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ucv.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghv.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rie.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tco.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jip.aizwys.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://asm.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://otk.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://zcl.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kre.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mrb.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxw.chenzaomai.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lbq.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kqg.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ixx.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jpb.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ddn.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://pcd.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://bvi.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://brv.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lka.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lpm.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mah.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://elu.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://mdv.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://que.chenlongwang.top

[B12] 跳出多层循环
来源：http://edg.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jqa.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://coq.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wdm.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://enn.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rhh.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nzt.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qhq.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ezz.nanxinkj.top

[B13] 判断是否为数字
来源：http://bva.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://gnq.dianchejie.cn

PHP:  is_numeric($x)
来源：http://pcw.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tor.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ayv.shangyingyoupin.top

Java: x instanceof Number
来源：http://myr.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hhx.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ouu.yangfankeji.com

C#:   x is int or double or decimal
来源：http://qfq.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://amy.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qey.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yoq.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://acc.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://tqz.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sja.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zuc.vehdjk.com


<!-- 参考信息 -->