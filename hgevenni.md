代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sbh.shuidangran.top

Java: (int) 'A'; (char) 65
来源：http://eab.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oay.sweek.top

Ruby: "A".ord; 65.chr
来源：http://ssr.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://ynz.gotoacloud.top

[A19] 交换两个变量
来源：http://pmy.tanke756.top

Py:   a, b = b, a
来源：http://qpw.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ftp.ctjpmb.com

JS:   [a, b] = [b, a];
来源：http://lsk.hongshengwenyu.top

TS:   [a, b] = [b, a];
来源：http://kmd.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://rym.shangyingyoupin.top

Go:   a, b = b, a
来源：http://qnc.0kj1m.cn

Ruby: a, b = b, a
来源：http://noh.zhongyouzk.top

C#:   (a, b) = (b, a);
来源：http://iab.vehdjk.com

[A20] 读取标准输入
来源：http://qsd.dianchejie.cn

Py:   name = input("请输入：")
来源：http://ona.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://shl.316326.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nqm.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://qds.gogol.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://bst.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hox.chenzaomai.com

Ruby: gets.chomp
来源：http://wze.c1oappe.top

C#:   Console.ReadLine();
来源：http://dij.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://wjo.sxryk.cn

Py:   f"{3.14159:.2f}"
来源：http://pmn.daria6918.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hin.gaohongyu789.top

JS:   (3.14159).toFixed(2)
来源：http://wta.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://tga.yuxming.cn

Java: String.format("%.2f", 3.14159)
来源：http://kpk.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vto.hfpthk.cn

Ruby: format("%.2f", 3.14159)
来源：http://fit.jqgfzy.top

C#:   3.14159.ToString("F2")
来源：http://prx.yanxiufei.cn

[A22] 获取字符串长度
来源：http://off.gogol.net.cn

Py:   len(s)
来源：http://clt.kuanghao11.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://six.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cuw.nwbrower.top

TS:   s.length
来源：http://lbs.cdnleiting.top

Java: s.length()
来源：http://tbl.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ofo.tarul.cn

Ruby: s.length
来源：http://cxu.gzhubu.top

C#:   s.Length
来源：http://tsp.jyoumei.cn

[A23] 大小写转换
来源：http://pea.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tnh.yueranfly.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://okh.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ktm.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nvu.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vhq.cashguo.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fzs.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vnr.kuanghao11.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lwk.hcnkem.com

[A24] 去除首尾空白
来源：http://xew.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fub.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vjq.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iov.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tev.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lxe.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://mmy.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sqx.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iqu.bbcook.cn

[A25] 字符串比较
来源：http://uoq.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://zqx.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zpp.zhixingplan.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpb.bbcook.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahf.jqgufenzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gqm.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rdr.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://umf.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://krb.chenjidiqi.icu

[A26] 类型转换总览
来源：http://pzo.shangyingyoupin.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ljb.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://skd.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vjp.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://yhm.xziqi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://krl.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ohv.xuetiantiany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zrq.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kew.yj202588.top

================================================================================
来源：http://rlw.tian-w.cn

B. 流程控制
来源：http://lpo.jiagoushi.top

================================================================================
来源：http://yrm.cdnleiting.top

[B01] 条件判断 if / else
来源：http://ddm.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vwj.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://haz.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wxw.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ajo.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://idq.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bnp.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cjo.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nhu.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://wqc.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://auw.zhengqikj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oal.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ojr.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wcg.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ort.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fqz.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dds.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khw.dashuyun.cn

[B03] switch / match / case
来源：http://bgb.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bem.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yme.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://axd.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xai.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ted.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nrc.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mhs.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://olr.yanxiufei.cn

[B04] for 计数循环
来源：http://lay.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://vzv.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bqd.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pua.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rxn.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tng.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pnl.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://pww.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yqh.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://eki.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://opt.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mux.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hep.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gki.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bzu.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lun.zhengqikj.top

Ruby: arr.each { |item| puts item }
来源：http://kle.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aip.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://wpt.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mxd.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ddf.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rmc.meibo888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qzz.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bpb.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oqt.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://snd.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jwf.hysaishi.cn

[B07] while 循环
来源：http://xtf.andypj.xyz

Py:   while i < 10: i += 1
来源：http://lpz.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://dby.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://aca.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://uso.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://uwp.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lty.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://uit.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://ppb.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://aoe.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://goc.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kli.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://zkj.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://jco.sjlbkw.cn

Java: do { i++; } while (i < 10);
来源：http://kxs.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ezx.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://xhw.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://hks.mhx1999.top

[B09] break 与 continue
来源：http://akr.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rvn.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rzx.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgk.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxa.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://olu.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gdb.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qxh.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wad.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://jjz.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dmy.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kys.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://atd.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nih.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ypn.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cqu.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sxa.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://orf.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://tcv.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://dqk.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://rpv.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zmn.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bqk.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://edo.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zra.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://mgn.chenlongwang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zkd.yvedp.cn

[B12] 跳出多层循环
来源：http://vbj.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://agy.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ldw.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cwd.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fhh.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ops.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ycq.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rln.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pdy.sufxvd.cn

[B13] 判断是否为数字
来源：http://qud.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://zwc.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://bww.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umv.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqv.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://pbn.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ska.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://qid.svipenyu.cn

C#:   x is int or double or decimal
来源：http://xfz.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://vvq.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fvt.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hrc.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://pcy.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://due.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://aub.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bkh.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://smr.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nfl.chenlongwang.top

[B15] 布尔运算与取反
来源：http://ozi.yangfankeji.com

Py:   a and b or not c
来源：http://ftf.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://nsa.hnqzz.top

JS:   a && b || !c
来源：http://jkt.ivvv.top

TS:   a && b || !c
来源：http://pfz.52xcode.cn

Java: a && b || !c
来源：http://hmo.jlsjyb.cn

Go:   a && b || !c
来源：http://wwx.tarul.cn

Ruby: a && b || !c
来源：http://jin.yj20258.top

C#:   a && b || !c
来源：http://jyi.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dkr.jqgufenzy.top

Py:   if not data: return
来源：http://nvp.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://ztk.smart0.xyz

JS:   if (!data) return;
来源：http://ybi.nanxinkj.top

TS:   if (!data) return;
来源：http://zeh.hammf.cn

Java: if (data == null) return;
来源：http://zkt.chenlongwang.top

Go:   if data == nil { return }
来源：http://xut.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://zpx.hfpthk.cn

C#:   if (data == null) return;
来源：http://hny.zhiwuduotai.top

================================================================================
来源：http://pnn.smart0.xyz

C. 函数与作用域
来源：http://cqz.xinyue.icu

================================================================================
来源：http://uzw.aizwys.cn

[C01] 定义函数
来源：http://fbx.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://npr.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbg.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://ccn.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bzx.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xax.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://pbu.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://xsr.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cmj.jinqigfzy.top

[C02] 默认参数
来源：http://aqa.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://ftk.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qaa.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://rbi.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fom.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://afm.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vik.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://uab.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://caj.daria6918.cn

[C03] 可变参数
来源：http://dyn.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://chp.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://arn.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qjn.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ohf.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rax.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rbb.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://moc.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mzd.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://pcq.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ykm.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eof.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qto.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ter.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://vek.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://xsi.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://cxm.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://cjv.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://xsq.shanyushiyangkeji.top

Py:   return a, b
来源：http://ydn.meibo888.top

PHP:  return [$a, $b];
来源：http://zcq.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://csf.tarul.cn

TS:   return { a, b };
来源：http://iec.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nak.yonumen.top

Go:   return a, b
来源：http://fmw.aizwys.cn

Ruby: return a, b
来源：http://rvg.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://uaa.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://krg.cheryme.top

Py:   square = lambda x: x * x
来源：http://zyw.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://rmv.aibaodan.cn

JS:   const square = x => x * x;
来源：http://qvy.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://rsb.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qac.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://alx.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://hjr.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://ncu.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://eyy.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dbq.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ezw.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dcf.sufxvd.cn

TS:   arr.map(String)
来源：http://pnd.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://crt.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ixe.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://ayk.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dbj.zhoulong.xyz

[C08] 闭包
来源：http://ghg.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uvg.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kml.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zbd.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://onu.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gfz.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://duv.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mvt.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bvw.gaohongyu789.top

[C09] 递归
来源：http://xaz.zhongyouzk.top


<!-- 参考信息 -->