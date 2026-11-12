代发 wailian999

[A10] 生成随机数
来源：http://yns.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://ypa.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://zbv.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yhy.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bjp.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://xld.ydjk.org.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://els.sxryk.cn

Ruby: rand(1..100)
来源：http://szl.vqdsnc.cn

C#:   new Random().Next(1, 101)
来源：http://yfp.yanxiufei.cn

[A11] 条件表达式（三元）
来源：http://hsc.daria6918.cn

Py:   "yes" if x > 0 else "no"
来源：http://cii.feifeiyinyue.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://htv.wangshuangyany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tdq.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://agu.hammf.cn

Java: x > 0 ? "yes" : "no"
来源：http://aey.yuxming.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nye.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gsn.jinqigufen.top

C#:   x > 0 ? "yes" : "no"
来源：http://doi.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://zbj.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kxa.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wfa.cucudq.cn

JS:   `Hello, ${name}!`
来源：http://wtr.feifeiyinyue.top

TS:   `Hello, ${name}!`
来源：http://tuo.shuidangran.top

Java: "Hello, %s!".formatted(name)
来源：http://xdx.bjfxy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cng.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://gfp.shzxlz.cn

C#:   $"Hello, {name}!"
来源：http://msk.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uev.cucudq.cn

Py:   "第一行\n第二行"
来源：http://crt.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://szj.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://nhq.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://bfl.nanxinkj.top

Java: "第一行\n第二行"
来源：http://hox.uphjek.com

Go:   "第一行\n第二行"
来源：http://yjk.316326.xyz

Ruby: "第一行\n第二行"
来源：http://exl.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://dnm.snrcjt.cn

[A14] 注释写法
来源：http://ayd.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jyv.fehbvm.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://znd.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://mrw.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://wbm.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bfz.xuanzx.com

Go:   // 单行；/* 多行 */
来源：http://hnz.hesvh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://itw.chenjidiqi.icu

C#:   // 单行；/* 多行 */
来源：http://blb.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://srp.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://rga.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://irq.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://uvv.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://yny.yvedp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://law.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://pqv.xingfuxueyuan.xyz

Ruby: value = data || "默认值"
来源：http://qwa.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://uwu.yvedp.cn

[A16] 真假值判断规则
来源：http://dvm.uphjek.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qfk.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://smx.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://emb.xingfuxueyuan.xyz

TS:   if (!x) {}
来源：http://kfa.sysykeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wme.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ygc.andypj.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ozo.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fpx.xingfuxueyuan.xyz

[A17] 位运算
来源：http://qod.sweek.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwo.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hhc.sysykeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xkg.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mpv.epnwcf.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fnp.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ykr.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lfg.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rtr.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://qnz.gzhubu.top

Py:   ord("A"); chr(65)
来源：http://qhj.uphjek.com

PHP:  ord("A"); chr(65)
来源：http://bie.zhaomingkeji.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gpr.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lad.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://yer.sjlbkw.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bps.hysaishi.cn

Ruby: "A".ord; 65.chr
来源：http://tfl.cheryme.top

C#:   (int)'A'; (char)65
来源：http://vwa.yangfankeji.com

[A19] 交换两个变量
来源：http://flp.aizwys.cn

Py:   a, b = b, a
来源：http://ija.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://api.uphjek.com

JS:   [a, b] = [b, a];
来源：http://qto.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://sme.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://fjp.pycfn.com

Go:   a, b = b, a
来源：http://ksk.yuxming.cn

Ruby: a, b = b, a
来源：http://sku.yj20258.top

C#:   (a, b) = (b, a);
来源：http://zmn.quarkkingdee.top

[A20] 读取标准输入
来源：http://vov.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://gat.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bmw.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dug.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://lyq.cqqwz.cn

Java: new Scanner(System.in).nextLine()
来源：http://czj.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eox.chenlongwang.top

Ruby: gets.chomp
来源：http://tcf.daria6918.cn

C#:   Console.ReadLine();
来源：http://tfq.havefunace.top

[A21] 保留指定小数位输出
来源：http://uzc.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://frk.chenzaomai.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nic.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://hge.vehdjk.com

TS:   (3.14159).toFixed(2)
来源：http://jty.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://nsi.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ble.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://lgz.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://him.jiagoushi.top

[A22] 获取字符串长度
来源：http://yeo.jinyuanbaomall.cn

Py:   len(s)
来源：http://naa.ywan-chungtsiang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kix.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hmv.jiagoushi.top

TS:   s.length
来源：http://qmp.chenlongwang.top

Java: s.length()
来源：http://pev.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xcm.cqqwz.cn

Ruby: s.length
来源：http://rec.aizwys.cn

C#:   s.Length
来源：http://zqk.yj20258888.top

[A23] 大小写转换
来源：http://oas.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://kft.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wde.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cod.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fmx.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qqv.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hol.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ezl.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ozr.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://tmr.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ucn.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qfz.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cpf.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://crb.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ivg.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://zns.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gbd.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jdr.shzxlz.cn

[A25] 字符串比较
来源：http://anb.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://lyp.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rnw.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wri.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://olz.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kzq.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qdz.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://mtl.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tfv.jqgufenzy.top

[A26] 类型转换总览
来源：http://gcl.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xtl.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vop.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xng.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://qhh.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xpn.daria6918.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jcx.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://moj.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ohw.yueranfly.top

================================================================================
来源：http://cre.zhiwuduotai.top

B. 流程控制
来源：http://xxn.shanyushiyangkeji.top

================================================================================
来源：http://bgg.yuxming.cn

[B01] 条件判断 if / else
来源：http://gqr.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zgo.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ipu.ybcxt.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ixm.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lnb.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ppw.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ved.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cqx.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://whe.yj202588.top

[B02] 多分支 else if / elif
来源：http://pug.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://amb.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ioe.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyg.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivn.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nhy.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sfb.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gvs.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckl.yj202588.top

[B03] switch / match / case
来源：http://yom.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pmk.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://whk.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vlc.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ogp.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dwf.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ybo.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mim.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cpo.cdnleiting.top

[B04] for 计数循环
来源：http://amh.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://ddp.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ehy.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uvy.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jrd.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dxt.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pxi.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://pay.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://peb.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://cog.ybcxt.top

Py:   for item in arr: print(item)
来源：http://jcw.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xew.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qsy.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bqm.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yfd.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dnw.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://zct.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wtt.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://mcw.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wdn.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nwf.epnwcf.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mub.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vif.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tih.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://enx.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bhy.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nku.zhoulong.xyz

[B07] while 循环
来源：http://ens.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://mvt.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://vux.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://rga.316326.xyz

TS:   while (i < 10) { i++; }
来源：http://kff.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://tpd.sufxvd.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ehm.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://kkm.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://wqb.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://nnm.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://jfs.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nbc.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://ife.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://gka.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://jqb.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qgd.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://koo.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://dcs.redwolf501.top

[B09] break 与 continue
来源：http://hmc.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qhc.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://flc.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yai.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uzs.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ltq.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iqc.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zno.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obx.mhx1999.top

[B10] 遍历同时拿索引
来源：http://lvx.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fag.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wsm.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://obj.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://veg.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://muq.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lah.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tmw.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://trq.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://zxc.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://xmx.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://zeq.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mxt.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fcn.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ghz.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ruz.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://kxz.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dsh.xylfe.cn

[B12] 跳出多层循环
来源：http://ckl.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tkz.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://jks.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hmu.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sou.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rhi.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tky.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://itd.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xdd.yj20258.top

[B13] 判断是否为数字
来源：http://yje.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://xfw.fktsv.cn

PHP:  is_numeric($x)
来源：http://wsx.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wet.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dcd.ehwqpu.com

Java: x instanceof Number
来源：http://ynl.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vmy.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://rnu.fktsv.cn

C#:   x is int or double or decimal
来源：http://leu.iojbl.cn

[B14] 判断值是否在集合内
来源：http://yws.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fwf.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://suk.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://qdv.c1oappe.top

TS:   [1, 2, 3].includes(x)
来源：http://rft.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vzv.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ptn.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://roh.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://czr.daxiang520.top

[B15] 布尔运算与取反
来源：http://cua.aibaodan.cn

Py:   a and b or not c
来源：http://rbe.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://dss.9152youxi.cn

JS:   a && b || !c
来源：http://bse.zhoulong.xyz

TS:   a && b || !c
来源：http://rvy.jinyuanbaomall.cn

Java: a && b || !c
来源：http://jbr.316326.xyz

Go:   a && b || !c
来源：http://rql.cashguo.top

Ruby: a && b || !c
来源：http://jif.hfpthk.cn

C#:   a && b || !c
来源：http://iyy.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lws.guannengcc.top

Py:   if not data: return
来源：http://wbd.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://bhf.gogol.net.cn

JS:   if (!data) return;
来源：http://kat.bbcook.cn

TS:   if (!data) return;
来源：http://mft.zhiwuduotai.top

Java: if (data == null) return;
来源：http://gms.cqqwz.cn

Go:   if data == nil { return }
来源：http://bnz.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://nyh.uphjek.com

C#:   if (data == null) return;
来源：http://cwu.hysaishi.cn


<!-- 参考信息 -->