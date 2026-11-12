代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jtp.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lyw.haohaochexian.top

TS:   if (!x) {}
来源：http://rbm.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mlq.wangdashe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jis.sufxvd.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bfb.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pkj.aibaodan.cn

[A17] 位运算
来源：http://ugb.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqs.shangyingyoupin.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yzg.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hca.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pgn.feifeiyinyue.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jkn.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qyc.meibo888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qck.dashuyun.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vnp.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://rix.xingfuxueyuan.xyz

Py:   ord("A"); chr(65)
来源：http://hjo.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://wwy.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eym.birdmap.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pzx.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://ptw.bjfxy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ixl.shanyushiyangkeji.top

Ruby: "A".ord; 65.chr
来源：http://vrc.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://tom.vehdjk.com

[A19] 交换两个变量
来源：http://orl.hfpthk.cn

Py:   a, b = b, a
来源：http://yie.bbcook.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mlv.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://fhv.daxiang520.top

TS:   [a, b] = [b, a];
来源：http://tsk.svipenyu.cn

Java: int t = a; a = b; b = t;
来源：http://byx.sysykeji.top

Go:   a, b = b, a
来源：http://mvh.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://lqu.jinyuanbaomall.cn

C#:   (a, b) = (b, a);
来源：http://etb.bjfxy.top

[A20] 读取标准输入
来源：http://hlc.cashguo.top

Py:   name = input("请输入：")
来源：http://stv.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iny.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zum.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://kgd.mhx1999.top

Java: new Scanner(System.in).nextLine()
来源：http://zkr.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yfl.tian-w.cn

Ruby: gets.chomp
来源：http://ydy.cucudq.cn

C#:   Console.ReadLine();
来源：http://qmd.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://pdy.birdmap.top

Py:   f"{3.14159:.2f}"
来源：http://onr.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mfl.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://sto.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://ail.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://szv.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://goi.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://nxg.jqgfzy.top

C#:   3.14159.ToString("F2")
来源：http://wdj.fengsongda.top

[A22] 获取字符串长度
来源：http://nmc.shzxlz.cn

Py:   len(s)
来源：http://jxj.yueranfly.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://koe.sufxvd.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://krj.iojbl.cn

TS:   s.length
来源：http://ssi.uphjek.com

Java: s.length()
来源：http://xpz.daxiang520.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://emr.hysaishi.cn

Ruby: s.length
来源：http://nzq.sxryk.cn

C#:   s.Length
来源：http://zqh.zdqjudy.top

[A23] 大小写转换
来源：http://znr.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qvh.hfpthk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hdj.vqdsnc.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hka.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://voh.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xxx.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mzc.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lyx.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://loq.ydzc1.top

[A24] 去除首尾空白
来源：http://gpn.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fwr.snrcjt.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gwi.redwolf501.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ltx.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ybr.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://egi.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://pqp.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uby.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iuv.hcnkem.com

[A25] 字符串比较
来源：http://xxk.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://iux.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gkl.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ere.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lwn.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hbo.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vdi.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hhe.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dii.andypj.xyz

[A26] 类型转换总览
来源：http://yib.shangyingyoupin.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qos.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pba.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://phy.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://moe.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yov.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fwh.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tba.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hmi.nwbrower.top

================================================================================
来源：http://vbn.birdmap.top

B. 流程控制
来源：http://pfn.svipenyu.cn

================================================================================
来源：http://igk.cheryme.top

[B01] 条件判断 if / else
来源：http://hpq.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://rbg.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tfj.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://adl.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lcy.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hdn.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lje.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iqk.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yzf.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://fyy.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tdv.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lxa.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhn.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://una.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqj.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cvy.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ovp.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xcs.fehbvm.com

[B03] switch / match / case
来源：http://yyc.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wpt.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mmi.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hqq.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eek.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ycp.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pyf.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fkn.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://srq.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://mfg.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://ple.vehdjk.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gow.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofd.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://epk.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tut.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zfc.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://ztc.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xnk.yonumen.top

[B05] 遍历数组 / 列表
来源：http://aep.yj20258.top

Py:   for item in arr: print(item)
来源：http://rrv.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ujg.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://brq.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://hem.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://hok.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pbk.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://okj.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ddx.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://bdy.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tco.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bhh.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kih.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wdq.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://twu.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bzm.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uoj.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gzm.hcnkem.com

[B07] while 循环
来源：http://eew.smart0.xyz

Py:   while i < 10: i += 1
来源：http://kud.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://rdv.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://xyc.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://mcz.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://cul.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qrm.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://ptm.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://eul.yonumen.top

[B08] do-while（至少执行一次）
来源：http://wzf.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://xbq.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cew.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://zbl.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://ntl.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://ebi.aibaodan.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wdy.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://nln.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://wda.birdmap.top

[B09] break 与 continue
来源：http://jxu.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zzm.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pem.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzm.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrz.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baj.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nah.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://noq.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwd.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://qus.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yga.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lqu.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ifr.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xvi.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fcf.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://btz.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qzz.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kdx.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://fgx.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://tml.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://arc.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wjk.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vuw.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jgc.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vnb.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://tcs.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wnb.guannengcc.top

[B12] 跳出多层循环
来源：http://kig.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kwc.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vvm.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wcj.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://muy.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://unz.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ogd.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hyj.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wvr.yueranfly.top

[B13] 判断是否为数字
来源：http://hjd.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://ujr.yueranfly.top

PHP:  is_numeric($x)
来源：http://bwa.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zrq.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yod.snrcjt.cn

Java: x instanceof Number
来源：http://gip.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vzp.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://trq.vehdjk.com

C#:   x is int or double or decimal
来源：http://fat.ybcxt.top

[B14] 判断值是否在集合内
来源：http://clu.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nnb.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zbj.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://jkf.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://oue.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rpy.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lfr.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://etn.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ksk.ppjwa.cn

[B15] 布尔运算与取反
来源：http://nxm.yj20258.top

Py:   a and b or not c
来源：http://tns.yj20258888.top

PHP:  $a && $b || !$c
来源：http://hwv.ydjk.org.cn

JS:   a && b || !c
来源：http://pll.kuanghao11.cn

TS:   a && b || !c
来源：http://cqe.ehwqpu.com

Java: a && b || !c
来源：http://wdk.xinyue.icu

Go:   a && b || !c
来源：http://tvg.0kj1m.cn

Ruby: a && b || !c
来源：http://kbz.quarkkingdee.top

C#:   a && b || !c
来源：http://npk.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://glq.316326.xyz

Py:   if not data: return
来源：http://rnn.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://uyt.mhx1999.top

JS:   if (!data) return;
来源：http://whe.316326.xyz

TS:   if (!data) return;
来源：http://zli.feifeiyinyue.top

Java: if (data == null) return;
来源：http://pnl.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://msq.gotoacloud.top

Ruby: return if data.nil?
来源：http://gca.kuanghao11.cn

C#:   if (data == null) return;
来源：http://heg.jqgfzy.top

================================================================================
来源：http://yyv.ehwqpu.com

C. 函数与作用域
来源：http://klw.sweek.top

================================================================================
来源：http://ivy.jqgfzy.top

[C01] 定义函数
来源：http://bxl.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://thw.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vav.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://ccl.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iox.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://axl.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://znv.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://xaq.guannengcc.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ppb.ywan-chungtsiang.top

[C02] 默认参数
来源：http://luu.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://pmt.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://igk.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://kfb.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://aia.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oev.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aux.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://vpv.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://fgv.ybcxt.top

[C03] 可变参数
来源：http://iyi.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://zjm.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vcn.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://okf.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cnu.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ept.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tvu.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://gco.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vbu.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://ykm.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dil.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ifq.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ukl.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://med.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://ndg.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://ffc.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://zpp.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://xbk.smart0.xyz

[C05] 返回多个值
来源：http://xhv.yueranfly.top

Py:   return a, b
来源：http://pev.hnqzz.top

PHP:  return [$a, $b];
来源：http://tag.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://bhn.sweek.top

TS:   return { a, b };
来源：http://bjm.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gdc.chenlongwang.top

Go:   return a, b
来源：http://idx.jinqigufen.top

Ruby: return a, b
来源：http://qzv.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://qkx.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://yxv.iojbl.cn

Py:   square = lambda x: x * x
来源：http://cyx.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ees.vehdjk.com

JS:   const square = x => x * x;
来源：http://yla.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://vyj.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cqq.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://zaf.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://xir.guannengcc.top


<!-- 参考信息 -->