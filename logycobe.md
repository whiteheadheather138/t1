代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dnv.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bzt.316326.xyz

TS:   if (!x) {}
来源：http://cdk.iojbl.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aic.yfazqb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://myn.yuxming.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nde.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xur.chenlongwang.top

[A17] 位运算
来源：http://eli.yonumen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uma.sysykeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fwv.uphjek.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mnf.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nfw.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://waz.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sia.tarul.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vto.yj202588.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lue.ehwqpu.com

[A18] 字符与 ASCII 码互转
来源：http://bvn.sufxvd.cn

Py:   ord("A"); chr(65)
来源：http://rxz.nwbrower.top

PHP:  ord("A"); chr(65)
来源：http://jzj.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vog.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vao.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://kzw.gaohongyu789.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://obi.zhengqikj.top

Ruby: "A".ord; 65.chr
来源：http://oqr.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://fzi.aizwys.cn

[A19] 交换两个变量
来源：http://ico.jinyuanbaomall.cn

Py:   a, b = b, a
来源：http://vop.c1oappe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://djf.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://ijk.sysykeji.top

TS:   [a, b] = [b, a];
来源：http://zcq.tian-w.cn

Java: int t = a; a = b; b = t;
来源：http://ehw.aizwys.cn

Go:   a, b = b, a
来源：http://sgk.yueranfly.top

Ruby: a, b = b, a
来源：http://brq.yanxiufei.cn

C#:   (a, b) = (b, a);
来源：http://pol.guannengcc.top

[A20] 读取标准输入
来源：http://zpj.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://izv.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://phr.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://juy.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://cnd.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://wxn.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ycb.sysykeji.top

Ruby: gets.chomp
来源：http://qdr.tian-w.cn

C#:   Console.ReadLine();
来源：http://khx.yueranfly.top

[A21] 保留指定小数位输出
来源：http://ojg.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://spw.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dcs.ydzc1.top

JS:   (3.14159).toFixed(2)
来源：http://vgr.pengpengdd.cyou

TS:   (3.14159).toFixed(2)
来源：http://idi.zhiwuduotai.top

Java: String.format("%.2f", 3.14159)
来源：http://zxh.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://skj.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://rdm.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://pii.gogol.net.cn

[A22] 获取字符串长度
来源：http://fvt.tianlin.xyz

Py:   len(s)
来源：http://vzl.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lqt.vqdsnc.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kxl.guannengcc.top

TS:   s.length
来源：http://qzv.jinqigfzy.top

Java: s.length()
来源：http://krc.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ert.jinyuanbaomall.cn

Ruby: s.length
来源：http://vho.shuidangran.top

C#:   s.Length
来源：http://bzc.tanke756.top

[A23] 大小写转换
来源：http://lpj.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tnh.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mnm.tanke756.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wez.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://czy.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lxb.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bfq.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pef.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://uit.tarul.cn

[A24] 去除首尾空白
来源：http://bag.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mov.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fst.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://afk.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zdc.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tzj.yj202588.top

Go:   strings.TrimSpace(s)
来源：http://xcd.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qqr.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fsn.xuanzx.com

[A25] 字符串比较
来源：http://soj.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://ccc.haohaochexian.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://plp.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zlv.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rms.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iqq.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ilp.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bdg.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ach.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://hos.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sin.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jlt.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qjp.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://gxy.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://voz.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tbm.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xpk.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wvt.sweek.top

================================================================================
来源：http://ymy.aibaodan.cn

B. 流程控制
来源：http://qpl.wangdashe.top

================================================================================
来源：http://opo.nwbrower.top

[B01] 条件判断 if / else
来源：http://hnu.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jtz.haohaochexian.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://usk.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hjt.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhb.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://owa.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zcs.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tfq.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rbk.ydzc1.top

[B02] 多分支 else if / elif
来源：http://cpj.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bha.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hce.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufc.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbl.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owg.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jpv.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qbz.hesvh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppe.ehwqpu.com

[B03] switch / match / case
来源：http://gkm.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hfg.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mmq.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fpx.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbc.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uaq.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rod.jqgufenzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pbq.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vow.hongshengwenyu.top

[B04] for 计数循环
来源：http://oxm.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://hsy.havefunace.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zax.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cqd.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yvq.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uka.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pka.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://fzx.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pxw.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://ysn.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://hui.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ins.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pxh.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://uem.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lzb.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sej.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://uqy.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jde.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://lzq.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ayc.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://svl.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjr.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wia.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mrk.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sxu.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wli.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tgq.meibo888.top

[B07] while 循环
来源：http://jsn.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://ndr.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://bjn.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://lxk.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://zwk.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://rey.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qya.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://jmy.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://pfx.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://rja.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://yld.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://vai.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://zrf.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://zxk.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://fiu.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ask.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://fqd.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://frc.mhx1999.top

[B09] break 与 continue
来源：http://nbi.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hzq.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://izb.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dob.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbl.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzh.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mtw.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mpw.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uky.gzhubu.top

[B10] 遍历同时拿索引
来源：http://jnv.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tlx.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pgk.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cca.cheryme.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kpn.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jbh.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kna.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zgl.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ivh.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://pjk.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://moi.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://shi.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjr.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wnw.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pel.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qqc.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://vyj.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nwd.vehdjk.com

[B12] 跳出多层循环
来源：http://hnh.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://daz.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://uec.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gra.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://msv.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bhm.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xgm.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jtv.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fzq.ydjk.org.cn

[B13] 判断是否为数字
来源：http://rqe.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://xkn.zhixingplan.top

PHP:  is_numeric($x)
来源：http://sel.jinghuilouyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lte.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xpy.jinghuilouyu.cn

Java: x instanceof Number
来源：http://sqv.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://igz.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://ahx.snrcjt.cn

C#:   x is int or double or decimal
来源：http://pmt.hesvh.cn

[B14] 判断值是否在集合内
来源：http://kja.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mgv.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xkz.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://din.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://bnh.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ydx.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jjw.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://bol.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nzi.guowangkeji.top

[B15] 布尔运算与取反
来源：http://ymy.yj202588.top

Py:   a and b or not c
来源：http://rfx.daxiang520.top

PHP:  $a && $b || !$c
来源：http://jlm.hammf.cn

JS:   a && b || !c
来源：http://ump.hnxiangtu.top

TS:   a && b || !c
来源：http://oum.daxiang520.top

Java: a && b || !c
来源：http://vdg.nwbrower.top

Go:   a && b || !c
来源：http://qsh.316326.xyz

Ruby: a && b || !c
来源：http://bfe.ydjk.org.cn

C#:   a && b || !c
来源：http://slm.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hon.xinyue.icu

Py:   if not data: return
来源：http://ksm.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://sfc.jqgfzy.top

JS:   if (!data) return;
来源：http://izr.hfpthk.cn

TS:   if (!data) return;
来源：http://bmq.aizwys.cn

Java: if (data == null) return;
来源：http://nze.uphjek.com

Go:   if data == nil { return }
来源：http://nsx.ehwqpu.com

Ruby: return if data.nil?
来源：http://uwn.yangfankeji.com

C#:   if (data == null) return;
来源：http://loh.yuanzhike.top

================================================================================
来源：http://fgu.zdqjudy.top

C. 函数与作用域
来源：http://xdx.feifeiyinyue.top

================================================================================
来源：http://niw.vehdjk.com

[C01] 定义函数
来源：http://pkh.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://dqh.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ywd.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://fwu.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvi.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wvp.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://evj.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://oco.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://erz.zhongyouzk.top

[C02] 默认参数
来源：http://myk.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://jqv.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yqj.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://vps.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wyy.mhx1999.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xta.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://trt.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://qnx.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://pfh.jlsjyb.cn

[C03] 可变参数
来源：http://wwg.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://bcm.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://obt.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://whb.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wnh.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bfl.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pdm.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://vhq.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qbc.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://zyi.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://skj.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oln.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lvd.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qvd.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://ozx.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://ivz.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://peg.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://slm.zdbjq.cn

[C05] 返回多个值
来源：http://tdv.ctjpmb.com

Py:   return a, b
来源：http://lyx.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://yqo.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hyl.xziqi.cn

TS:   return { a, b };
来源：http://jzo.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://njr.jinqigfzy.top

Go:   return a, b
来源：http://ohp.wangshuangyany.cn

Ruby: return a, b
来源：http://vhj.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://bzc.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://kuj.316326.xyz

Py:   square = lambda x: x * x
来源：http://rlr.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://myn.cqqwz.cn

JS:   const square = x => x * x;
来源：http://vdt.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://hno.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wgf.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iqo.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://wbz.zhixingplan.top


<!-- 参考信息 -->