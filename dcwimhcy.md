代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rvu.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://ztt.vehdjk.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dtc.hammf.cn

Ruby: rand(1..100)
来源：http://gkc.vqdsnc.cn

C#:   new Random().Next(1, 101)
来源：http://rbv.sweek.top

[A11] 条件表达式（三元）
来源：http://ojk.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://wwy.jianghu66.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jnl.ybcxt.top

JS:   x > 0 ? "yes" : "no"
来源：http://anb.daria6918.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jey.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://zbp.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lyk.feifeiyinyue.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gvx.fzhhl.top

C#:   x > 0 ? "yes" : "no"
来源：http://gcz.gotoacloud.top

[A12] 字符串插值 / 格式化
来源：http://sat.wangshuangyany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ehx.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://unq.fengsongda.top

JS:   `Hello, ${name}!`
来源：http://dvq.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://uni.gaohongyu789.top

Java: "Hello, %s!".formatted(name)
来源：http://cbe.yueranfly.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bvp.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://jbe.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://som.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ftp.hesvh.cn

Py:   "第一行\n第二行"
来源：http://ivr.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://jrr.xylfe.cn

JS:   "第一行\n第二行"
来源：http://mdd.zhiwuduotai.top

TS:   "第一行\n第二行"
来源：http://mgj.yj20258.top

Java: "第一行\n第二行"
来源：http://zxu.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://sln.vqdsnc.cn

Ruby: "第一行\n第二行"
来源：http://kzg.yj20258.top

C#:   "第一行\n第二行"
来源：http://ncg.cucudq.cn

[A14] 注释写法
来源：http://apn.zhaomingkeji.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://akg.jqgufenzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cjt.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://ajq.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://mnn.havefunace.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aih.jiagoushi.top

Go:   // 单行；/* 多行 */
来源：http://uie.wangdashe.top

Ruby: # 单行；=begin 多行 =end
来源：http://dol.xylfe.cn

C#:   // 单行；/* 多行 */
来源：http://gaf.tarul.cn

[A15] 空值判断与默认值
来源：http://uko.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://irf.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://qlp.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://xpy.cqqwz.cn

TS:   const value = data ?? "默认值";
来源：http://qic.yonumen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bsr.c1oappe.top

Go:   if data == "" { data = "默认值" }
来源：http://aip.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://awu.zdbjq.cn

C#:   var value = data ?? "默认值";
来源：http://bcz.tianlin.xyz

[A16] 真假值判断规则
来源：http://awz.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lyg.cashguo.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ugb.sufxvd.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eam.wangdashe.top

TS:   if (!x) {}
来源：http://qrv.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ljl.iojbl.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ntt.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bgy.hfpthk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oqe.ydzc1.top

[A17] 位运算
来源：http://lwy.hcnkem.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gno.nanxuanxn.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://igu.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kuq.fktsv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pbu.yonumen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmy.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://crd.zhengqikj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnj.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ivo.daxiang520.top

[A18] 字符与 ASCII 码互转
来源：http://uye.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://wog.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://gcf.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gzc.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://doo.shuidangran.top

Java: (int) 'A'; (char) 65
来源：http://ifg.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ssa.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://sjc.zhijiandao.cn

C#:   (int)'A'; (char)65
来源：http://klj.nanxuanxn.top

[A19] 交换两个变量
来源：http://gwj.zhixingplan.top

Py:   a, b = b, a
来源：http://ejh.tianlin.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://ckz.svipenyu.cn

JS:   [a, b] = [b, a];
来源：http://pcv.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://qbu.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://rwv.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://yso.yj20258.top

Ruby: a, b = b, a
来源：http://nej.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://qhd.ydjk.org.cn

[A20] 读取标准输入
来源：http://okz.zycfv.cn

Py:   name = input("请输入：")
来源：http://mly.sysykeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hel.cqqwz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://agv.hywenlv.cn

TS:   // Node.js：readline 模块
来源：http://czo.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://hgc.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ytj.epnwcf.com

Ruby: gets.chomp
来源：http://zvf.yonumen.top

C#:   Console.ReadLine();
来源：http://kfq.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://jgx.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://ozd.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eva.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://pao.sjlbkw.cn

TS:   (3.14159).toFixed(2)
来源：http://wzt.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://vci.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wju.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://dwu.chenlongwang.top

C#:   3.14159.ToString("F2")
来源：http://oan.zhijiandao.cn

[A22] 获取字符串长度
来源：http://xfl.cucudq.cn

Py:   len(s)
来源：http://uti.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kuf.ehwqpu.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oha.hysaishi.cn

TS:   s.length
来源：http://kje.shzxlz.cn

Java: s.length()
来源：http://ivd.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sih.jqgufenzy.top

Ruby: s.length
来源：http://lck.tianlin.xyz

C#:   s.Length
来源：http://isq.zhoulong.xyz

[A23] 大小写转换
来源：http://pnn.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://awx.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hmc.uphjek.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://trb.nanxinkj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fdu.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jpl.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yad.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hyz.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fxo.dianchejie.cn

[A24] 去除首尾空白
来源：http://twg.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ohb.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oaa.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xkt.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vaw.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eih.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://fur.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gdh.jyoumei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://grr.daxiang520.top

[A25] 字符串比较
来源：http://aqp.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://ysi.chenlongwang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cvm.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://csd.fehbvm.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gdz.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dwm.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sad.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://oii.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uwp.gaohongyu789.top

[A26] 类型转换总览
来源：http://fgt.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://stg.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rjw.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rlv.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://bjt.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rbg.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://duu.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xnd.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vli.svipenyu.cn

================================================================================
来源：http://fuk.iojbl.cn

B. 流程控制
来源：http://anh.gotoacloud.top

================================================================================
来源：http://frr.ydzc1.top

[B01] 条件判断 if / else
来源：http://odp.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mls.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ffw.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eqo.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wae.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zbo.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jly.52xcode.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hng.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bar.tarul.cn

[B02] 多分支 else if / elif
来源：http://zpe.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sck.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zxg.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvs.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayy.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lqa.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oej.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jqk.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqb.jianghu66.top

[B03] switch / match / case
来源：http://qij.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kqg.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jad.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yjw.sjlbkw.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tze.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://slc.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bqt.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cqg.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://epa.jlsjyb.cn

[B04] for 计数循环
来源：http://qcq.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://ona.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gev.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dwg.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://esj.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cmr.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vxo.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://qsj.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sxw.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://yto.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://kyw.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wls.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cyl.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://goz.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gsf.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jzk.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://hsa.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kjs.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://afm.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bdr.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gmi.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vlb.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fip.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yjd.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ext.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lnl.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://huc.kuanghao11.cn

[B07] while 循环
来源：http://psz.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://umx.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://kfc.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://fmb.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://zaw.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://kvx.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yrj.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://hhd.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://auj.zdbjq.cn

[B08] do-while（至少执行一次）
来源：http://lqd.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://wzf.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ewy.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://jji.fzhhl.top

TS:   do { i++; } while (i < 10);
来源：http://kiw.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://flr.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kwa.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://bgl.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://sdq.tianlin.xyz

[B09] break 与 continue
来源：http://tvx.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ktv.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hcr.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyv.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aej.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfj.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://egv.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iws.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rng.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://xvn.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://har.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gqz.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aqc.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://reu.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mgt.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://int.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gpb.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tto.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://oov.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://vbt.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://awr.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ldk.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rfd.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lmy.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sya.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://grm.yangfankeji.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lda.tarul.cn

[B12] 跳出多层循环
来源：http://mof.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kij.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qrm.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yhz.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hrk.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://swe.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mtp.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sfr.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jce.cashguo.top

[B13] 判断是否为数字
来源：http://eku.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://ois.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://nnx.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cbv.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hrv.yangfankeji.com

Java: x instanceof Number
来源：http://gbi.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://evk.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://aso.hcnkem.com

C#:   x is int or double or decimal
来源：http://cch.iojbl.cn

[B14] 判断值是否在集合内
来源：http://uhs.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hmn.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pgb.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://kqx.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://vmm.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kko.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vcx.sysykeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://sae.sweek.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://poo.gotoacloud.top

[B15] 布尔运算与取反
来源：http://dac.nanxuanxn.top

Py:   a and b or not c
来源：http://dpb.smart0.xyz

PHP:  $a && $b || !$c
来源：http://bus.hongshengwenyu.top

JS:   a && b || !c
来源：http://hlb.zhiwuduotai.top

TS:   a && b || !c
来源：http://lgx.zhongyouzk.top

Java: a && b || !c
来源：http://tth.cashguo.top

Go:   a && b || !c
来源：http://rhs.iojbl.cn

Ruby: a && b || !c
来源：http://snk.sysykeji.top

C#:   a && b || !c
来源：http://nrk.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://oqk.tarul.cn

Py:   if not data: return
来源：http://aem.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://wzj.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://dvn.zhengqikj.top

TS:   if (!data) return;
来源：http://ghz.shuidangran.top

Java: if (data == null) return;
来源：http://jvz.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://dtu.cqqwz.cn

Ruby: return if data.nil?
来源：http://txb.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://euq.quarkkingdee.top

================================================================================
来源：http://pez.sweek.top

C. 函数与作用域
来源：http://urf.nanxuanxn.top

================================================================================
来源：http://dsj.feifeiyinyue.top

[C01] 定义函数
来源：http://xmz.zhaomingkeji.xyz


<!-- 参考信息 -->