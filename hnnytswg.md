代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://isk.yj202588.top

[A15] 空值判断与默认值
来源：http://qyp.feifeiyinyue.top

Py:   value = data or "默认值"
来源：http://hpo.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://ifh.gzhubu.top

JS:   const value = data ?? "默认值";
来源：http://lxz.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://ead.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iog.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://pgf.yj20258.top

Ruby: value = data || "默认值"
来源：http://gon.jinghuilouyu.cn

C#:   var value = data ?? "默认值";
来源：http://ayd.zdqjudy.top

[A16] 真假值判断规则
来源：http://shq.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hko.tarul.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fvu.zhiwuduotai.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wtu.jiagoushi.top

TS:   if (!x) {}
来源：http://jmb.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fuj.hywenlv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tgg.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://xep.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lkn.fehbvm.com

[A17] 位运算
来源：http://kez.iojbl.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srj.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sru.gzhubu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qwu.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://okn.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bmx.c1oappe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://avf.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdy.yj202588.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bli.guowangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://lkf.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://qpt.tanke756.top

PHP:  ord("A"); chr(65)
来源：http://lmc.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bzq.yanxiufei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bdg.hcnkem.com

Java: (int) 'A'; (char) 65
来源：http://ldn.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mmf.cucudq.cn

Ruby: "A".ord; 65.chr
来源：http://som.zhengqikj.top

C#:   (int)'A'; (char)65
来源：http://hvc.svipenyu.cn

[A19] 交换两个变量
来源：http://ihg.sufxvd.cn

Py:   a, b = b, a
来源：http://zql.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://mfu.xingfuxueyuan.xyz

JS:   [a, b] = [b, a];
来源：http://dwj.nwbrower.top

TS:   [a, b] = [b, a];
来源：http://thh.jqgfzy.top

Java: int t = a; a = b; b = t;
来源：http://mzh.daxiang520.top

Go:   a, b = b, a
来源：http://yke.zycfv.cn

Ruby: a, b = b, a
来源：http://zqg.feifeiyinyue.top

C#:   (a, b) = (b, a);
来源：http://dca.jinqigfzy.top

[A20] 读取标准输入
来源：http://fnm.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://vkr.ywan-chungtsiang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sno.hnqzz.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ric.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://xnp.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://vrp.tianlin.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zbd.gzhubu.top

Ruby: gets.chomp
来源：http://epi.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://tdy.bjfxy.top

[A21] 保留指定小数位输出
来源：http://lwk.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://qrg.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vnl.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://dex.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://xwr.cucudq.cn

Java: String.format("%.2f", 3.14159)
来源：http://jpm.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ddj.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://zey.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://rxa.jinghuilouyu.cn

[A22] 获取字符串长度
来源：http://brk.redwolf501.top

Py:   len(s)
来源：http://fqr.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rev.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gix.iojbl.cn

TS:   s.length
来源：http://kas.ctjpmb.com

Java: s.length()
来源：http://zbf.zhengqikj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sje.iojbl.cn

Ruby: s.length
来源：http://apz.smart0.xyz

C#:   s.Length
来源：http://ujw.sweek.top

[A23] 大小写转换
来源：http://tvz.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://plu.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hxr.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://awa.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pef.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://urb.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iej.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dxf.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://iwy.hfpthk.cn

[A24] 去除首尾空白
来源：http://gns.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jap.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zjb.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://amp.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lwf.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rpr.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://txy.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ugh.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wop.havefunace.top

[A25] 字符串比较
来源：http://kxm.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://dlc.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lkf.sxryk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://spw.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qox.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blj.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qgz.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bpl.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://agu.chenjidiqi.icu

[A26] 类型转换总览
来源：http://rtt.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sin.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nzb.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jvf.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://wwi.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vrw.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xag.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dmo.fanxiaobao.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uxu.jinqigfzy.top

================================================================================
来源：http://chm.yvedp.cn

B. 流程控制
来源：http://sre.guannengcc.top

================================================================================
来源：http://gnf.tian-w.cn

[B01] 条件判断 if / else
来源：http://ija.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mra.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zdy.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ipu.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ril.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://swo.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pph.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://saa.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://giw.yongpay.top

[B02] 多分支 else if / elif
来源：http://nip.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pfz.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dmu.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxi.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjq.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bha.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jxv.yj20258888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wxe.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pug.zhijiandao.cn

[B03] switch / match / case
来源：http://uqy.yuanzhike.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qtj.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uir.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wat.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ukw.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zpe.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gpo.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pne.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://djj.chenlongwang.top

[B04] for 计数循环
来源：http://sfo.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://gnl.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iqn.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hav.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hfp.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zvb.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tlm.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://bch.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ijy.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://kff.xuanzx.com

Py:   for item in arr: print(item)
来源：http://vaf.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zsg.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gzc.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://koa.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uat.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ljc.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://evq.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://syf.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://cru.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xjj.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zni.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://num.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jqw.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oaa.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://swj.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mxx.tianlin.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uqj.xuetiantiany.cn

[B07] while 循环
来源：http://njj.ivvv.top

Py:   while i < 10: i += 1
来源：http://mcl.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://tia.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://ibh.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://urn.ivvv.top

Java: while (i < 10) { i++; }
来源：http://ftl.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hai.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://sei.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://xzm.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://uln.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://fgp.jqgfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://csk.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://myt.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://zsx.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://vnj.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://wnr.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mpb.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://jbq.shangyingyoupin.top

[B09] break 与 continue
来源：http://cnn.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qbv.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cdm.chenlongwang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubt.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uft.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cbo.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nth.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lrf.gaohongyu789.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owg.yueranfly.top

[B10] 遍历同时拿索引
来源：http://cxb.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://weq.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jiw.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cye.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ohk.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qed.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ztp.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cmt.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ukj.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://knh.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://dcu.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://bba.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ltb.jianghu66.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gpc.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qjr.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vjs.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://kvy.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://riu.yonumen.top

[B12] 跳出多层循环
来源：http://usi.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cbw.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wvs.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yyf.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gch.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qha.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yvp.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://opr.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sld.gotoacloud.top

[B13] 判断是否为数字
来源：http://dur.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://htf.aizwys.cn

PHP:  is_numeric($x)
来源：http://qdr.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdm.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rfa.cqqwz.cn

Java: x instanceof Number
来源：http://cng.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://duw.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://ekb.yonumen.top

C#:   x is int or double or decimal
来源：http://iee.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://jsd.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://obl.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://snm.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://qzd.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://qsu.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://xvi.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vpw.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hqy.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sap.zycfv.cn

[B15] 布尔运算与取反
来源：http://cwj.zycfv.cn

Py:   a and b or not c
来源：http://eem.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://lnv.jyoumei.cn

JS:   a && b || !c
来源：http://kby.dashuyun.cn

TS:   a && b || !c
来源：http://mlw.52xcode.cn

Java: a && b || !c
来源：http://zgb.fehbvm.com

Go:   a && b || !c
来源：http://ivf.guowangkeji.top

Ruby: a && b || !c
来源：http://wwl.yongpay.top

C#:   a && b || !c
来源：http://goh.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://lol.gaohongyu789.top

Py:   if not data: return
来源：http://cvh.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://wta.yangfankeji.com

JS:   if (!data) return;
来源：http://djs.0kj1m.cn

TS:   if (!data) return;
来源：http://slf.jinqigfzy.top

Java: if (data == null) return;
来源：http://jrk.cqqwz.cn

Go:   if data == nil { return }
来源：http://brm.snrcjt.cn

Ruby: return if data.nil?
来源：http://wac.fzhhl.top

C#:   if (data == null) return;
来源：http://xnf.snrcjt.cn

================================================================================
来源：http://kzc.gaohongyu789.top

C. 函数与作用域
来源：http://axd.svipenyu.cn

================================================================================
来源：http://xmi.tarul.cn

[C01] 定义函数
来源：http://fwu.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://abu.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hsh.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://wgq.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pgp.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mdb.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://fid.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://iom.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://phd.ivvv.top

[C02] 默认参数
来源：http://pxw.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://lhw.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lcw.daria6918.cn

JS:   function greet(name = "World") { return name; }
来源：http://hls.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uad.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://prw.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cxl.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://rtk.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://yzy.svipenyu.cn

[C03] 可变参数
来源：http://dbk.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://gwv.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://saw.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cwb.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qtn.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://olr.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dph.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://btu.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ksz.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://hba.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://raa.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://asx.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://itk.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qdu.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://deq.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://xpd.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://elp.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://qnx.tanke756.top

[C05] 返回多个值
来源：http://mze.jqgfzy.top

Py:   return a, b
来源：http://agh.guannengcc.top

PHP:  return [$a, $b];
来源：http://nev.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gkj.ivvv.top

TS:   return { a, b };
来源：http://djw.mhx1999.top


<!-- 参考信息 -->