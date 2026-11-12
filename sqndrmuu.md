代发 wailian999

Ruby: value = data || "默认值"
来源：http://fza.ydzc1.top

C#:   var value = data ?? "默认值";
来源：http://hak.shangyingyoupin.top

[A16] 真假值判断规则
来源：http://zkx.bbcook.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://phs.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://abe.zhijiandao.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cix.tian-w.cn

TS:   if (!x) {}
来源：http://elx.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://trz.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://snu.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://aai.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://obl.daxiang520.top

[A17] 位运算
来源：http://ryk.jiagoushi.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nxf.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wza.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jvp.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kvg.feifeiyinyue.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mkx.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gdc.smart0.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kom.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://btj.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://swc.jqgufenzy.top

Py:   ord("A"); chr(65)
来源：http://tam.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://hvn.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vfd.vehdjk.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://chl.ydzc1.top

Java: (int) 'A'; (char) 65
来源：http://vqu.ctjpmb.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zes.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://owt.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://brd.xuanzx.com

[A19] 交换两个变量
来源：http://vou.hnqzz.top

Py:   a, b = b, a
来源：http://hbb.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qkx.mhx1999.top

JS:   [a, b] = [b, a];
来源：http://idc.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://ntg.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://pgh.ppjwa.cn

Go:   a, b = b, a
来源：http://zso.quarkkingdee.top

Ruby: a, b = b, a
来源：http://yvi.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://kfn.kuanghao11.cn

[A20] 读取标准输入
来源：http://lvc.zhengqikj.top

Py:   name = input("请输入：")
来源：http://nrm.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xpy.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jip.cdnleiting.top

TS:   // Node.js：readline 模块
来源：http://cpu.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://iwb.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cvu.epnwcf.com

Ruby: gets.chomp
来源：http://xww.ywan-chungtsiang.top

C#:   Console.ReadLine();
来源：http://ozi.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://neu.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://eoz.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dya.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://hem.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://fic.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://cia.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uhl.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://pga.zdqjudy.top

C#:   3.14159.ToString("F2")
来源：http://epu.iojbl.cn

[A22] 获取字符串长度
来源：http://fmi.hnqzz.top

Py:   len(s)
来源：http://eqf.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rph.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://thv.chenjidiqi.icu

TS:   s.length
来源：http://vtf.haohaochexian.top

Java: s.length()
来源：http://uue.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zmc.yuanzhike.top

Ruby: s.length
来源：http://vhf.yueranfly.top

C#:   s.Length
来源：http://awv.bjfxy.top

[A23] 大小写转换
来源：http://zsm.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qkv.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fko.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kxn.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://top.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ljz.zycfv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bey.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yne.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ucm.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://nlr.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tre.hfpthk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://psa.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lyk.52xcode.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tnu.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gpl.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://jlc.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sgo.tian-w.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tmo.zhoulong.xyz

[A25] 字符串比较
来源：http://oyd.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://enh.yuanzhike.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rvl.tianlin.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zsp.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iok.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cpf.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ibc.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xno.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tte.ydjk.org.cn

[A26] 类型转换总览
来源：http://kcv.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ddw.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nmi.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zao.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://gen.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mlo.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lwa.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gtq.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ike.gotoacloud.top

================================================================================
来源：http://mwe.tian-w.cn

B. 流程控制
来源：http://smv.vehdjk.com

================================================================================
来源：http://jmb.0kj1m.cn

[B01] 条件判断 if / else
来源：http://ils.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cko.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ock.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qlo.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://unf.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://wjf.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nci.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ehw.cheryme.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://urv.yongpay.top

[B02] 多分支 else if / elif
来源：http://hbl.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bvr.yueranfly.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uvd.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dlg.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slg.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmz.xziqi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qfu.redwolf501.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gsk.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iam.bbcook.cn

[B03] switch / match / case
来源：http://lua.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bjc.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nfy.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pfr.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rno.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://viy.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://efx.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://znn.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ena.quarkkingdee.top

[B04] for 计数循环
来源：http://gut.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://ino.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dkv.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pdp.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qhl.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pid.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ddk.yangfankeji.com

Ruby: 10.times { |i| puts i }
来源：http://lah.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zmx.uphjek.com

[B05] 遍历数组 / 列表
来源：http://iyy.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://mpa.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://unr.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gyz.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wen.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rpm.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dju.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://btf.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://suq.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://smt.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cgf.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mza.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://akr.uphjek.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ste.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xky.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ppv.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xnk.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qqe.redwolf501.top

[B07] while 循环
来源：http://lbz.wangdashe.top

Py:   while i < 10: i += 1
来源：http://djd.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mqc.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://crr.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://pzp.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://zyu.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lcd.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://oue.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://nji.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://ryg.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://els.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xtz.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://dnq.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://xjq.xylfe.cn

Java: do { i++; } while (i < 10);
来源：http://noa.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dmp.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://suk.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://lmo.zhengqikj.top

[B09] break 与 continue
来源：http://nnz.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bdg.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jfn.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ikm.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wsd.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cmg.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mau.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fcv.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyr.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://nzy.yuxming.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yvv.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tac.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nxk.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fri.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nxt.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mvq.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sfx.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://koo.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://uqg.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://opg.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://rom.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ulf.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cxd.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jmj.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nzd.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://icg.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yih.cheryme.top

[B12] 跳出多层循环
来源：http://pbw.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lpc.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oru.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ndd.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hsa.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mqf.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dpp.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pxk.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ntp.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://swl.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://rlx.cashguo.top

PHP:  is_numeric($x)
来源：http://txk.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqy.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xds.hnqzz.top

Java: x instanceof Number
来源：http://nkw.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nnq.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://dcg.zycfv.cn

C#:   x is int or double or decimal
来源：http://upf.shuidangran.top

[B14] 判断值是否在集合内
来源：http://eth.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://syc.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zta.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://fdx.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://dmb.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ndz.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wpl.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://qlp.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://reu.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://jui.xziqi.cn

Py:   a and b or not c
来源：http://ein.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://jug.c1oappe.top

JS:   a && b || !c
来源：http://ojs.nanxinkj.top

TS:   a && b || !c
来源：http://lay.ppjwa.cn

Java: a && b || !c
来源：http://kjb.uphjek.com

Go:   a && b || !c
来源：http://rym.yanxiufei.cn

Ruby: a && b || !c
来源：http://zwv.sjlbkw.cn

C#:   a && b || !c
来源：http://vfx.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qfa.yonumen.top

Py:   if not data: return
来源：http://tca.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://wdr.zhiwuduotai.top

JS:   if (!data) return;
来源：http://lsd.haohaochexian.top

TS:   if (!data) return;
来源：http://yay.sjlbkw.cn

Java: if (data == null) return;
来源：http://ljk.pycfn.com

Go:   if data == nil { return }
来源：http://fdv.zhixingplan.top

Ruby: return if data.nil?
来源：http://lgi.zhoulong.xyz

C#:   if (data == null) return;
来源：http://tce.chenlongwang.top

================================================================================
来源：http://whj.shanyushiyangtech.top

C. 函数与作用域
来源：http://edj.tarul.cn

================================================================================
来源：http://giw.hongshengwenyu.top

[C01] 定义函数
来源：http://ubc.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://unj.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vlf.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://mnn.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qfn.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://buq.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://uyp.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://fzc.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://klx.yangfankeji.com

[C02] 默认参数
来源：http://hxy.uphjek.com

Py:   def greet(name="World"): return name
来源：http://obp.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cjd.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://pav.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nbk.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vmp.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hhe.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://occ.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://lkh.guannengcc.top

[C03] 可变参数
来源：http://jgo.havefunace.top

Py:   def total(*args): return sum(args)
来源：http://jub.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qqc.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xbj.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qgd.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ypo.fzhhl.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rwc.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://qcw.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vkh.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://dqc.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jvt.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oon.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kin.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qtl.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://zcn.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://ggw.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://tof.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://zpm.0kj1m.cn

[C05] 返回多个值
来源：http://jlg.zhengqikj.top

Py:   return a, b
来源：http://uff.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://nzr.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tzu.0kj1m.cn

TS:   return { a, b };
来源：http://fqd.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nhd.cucudq.cn

Go:   return a, b
来源：http://dok.yfazqb.com

Ruby: return a, b
来源：http://hqi.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://nwx.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://gll.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://qqb.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pzy.hammf.cn

JS:   const square = x => x * x;
来源：http://jnb.yj20258888.top


<!-- 参考信息 -->