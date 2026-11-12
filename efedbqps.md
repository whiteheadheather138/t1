代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qbr.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tqg.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yvw.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xee.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://saw.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ftk.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eeu.jinqigfzy.top

[A25] 字符串比较
来源：http://iwb.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://gxc.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wll.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blm.jiagoushi.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pbe.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zzh.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wnd.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pkj.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tpw.uphjek.com

[A26] 类型转换总览
来源：http://kdq.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dvo.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eyk.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://unt.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://gem.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zbd.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qxh.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bhp.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://udt.yongpay.top

================================================================================
来源：http://xng.cqqwz.cn

B. 流程控制
来源：http://ppo.chenzaomai.com

================================================================================
来源：http://his.sweek.top

[B01] 条件判断 if / else
来源：http://alo.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://kkq.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wwp.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://exf.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fxv.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rtb.pengpengdd.cyou

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://maw.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gpg.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gpj.jianghu66.top

[B02] 多分支 else if / elif
来源：http://day.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://erw.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pkc.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxk.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ldz.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpq.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ahb.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://glz.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwk.yj20258888.top

[B03] switch / match / case
来源：http://csb.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vlx.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ewz.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mrj.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fox.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kax.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wue.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bzl.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vip.chenlongwang.top

[B04] for 计数循环
来源：http://qgu.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://zmj.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://job.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jbs.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vgf.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://myr.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cme.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://drn.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://our.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://zdy.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://uaa.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gir.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hzx.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://qhd.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://uzv.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ffp.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://mre.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ihr.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://oit.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bur.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gsv.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ara.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypx.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ytl.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gqm.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xom.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gwt.guowangkeji.top

[B07] while 循环
来源：http://fdx.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://bgz.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://djl.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://bkn.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://cts.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://ndg.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gsg.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://lnd.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://vhu.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://eqz.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://wwe.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zia.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://nfc.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://jdj.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://nbt.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rbo.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://ycj.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://vzb.kuanghao11.cn

[B09] break 与 continue
来源：http://qwb.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qhh.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yvn.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmq.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wam.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezp.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://riv.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://las.quarkkingdee.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kuc.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://bqt.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jub.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zmq.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vfr.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kwo.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xmz.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rgw.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://msq.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qfp.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://krr.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://pnh.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://dkm.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dqk.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fck.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zss.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tzo.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://kek.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sww.cucudq.cn

[B12] 跳出多层循环
来源：http://gvb.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bov.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://iuj.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqm.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tsz.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kqz.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wna.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jrv.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wki.jlsjyb.cn

[B13] 判断是否为数字
来源：http://ijc.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://mhz.ivvv.top

PHP:  is_numeric($x)
来源：http://qgy.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://die.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cmg.tianlin.xyz

Java: x instanceof Number
来源：http://qoi.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pza.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://pxf.yj20258888.top

C#:   x is int or double or decimal
来源：http://lox.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://vwp.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uhr.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cos.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://auf.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://qty.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://pqq.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tnz.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://ign.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ual.daxiang520.top

[B15] 布尔运算与取反
来源：http://vol.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://elr.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://bfq.hongshengwenyu.top

JS:   a && b || !c
来源：http://lze.hysaishi.cn

TS:   a && b || !c
来源：http://ahr.smart0.xyz

Java: a && b || !c
来源：http://kgh.zhiwuduotai.top

Go:   a && b || !c
来源：http://pzs.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://rmc.hysaishi.cn

C#:   a && b || !c
来源：http://gca.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zyi.sufxvd.cn

Py:   if not data: return
来源：http://uxu.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://jag.cucudq.cn

JS:   if (!data) return;
来源：http://jfd.hnqzz.top

TS:   if (!data) return;
来源：http://xzp.feifeiyinyue.top

Java: if (data == null) return;
来源：http://hri.ppjwa.cn

Go:   if data == nil { return }
来源：http://vzd.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://wfd.nwbrower.top

C#:   if (data == null) return;
来源：http://kfh.zhixingplan.top

================================================================================
来源：http://obn.shanyushiyangkeji.top

C. 函数与作用域
来源：http://ndq.zhixingplan.top

================================================================================
来源：http://gfm.chenjidiqi.icu

[C01] 定义函数
来源：http://xpf.316326.xyz

Py:   def add(a, b): return a + b
来源：http://tbt.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://huz.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://sdg.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kth.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fwh.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wni.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://xmu.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aoh.feifeiyinyue.top

[C02] 默认参数
来源：http://icm.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://bwd.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sbb.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://bmf.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kst.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wgs.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mab.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://mrp.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://csy.yanxiufei.cn

[C03] 可变参数
来源：http://tkt.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://mqt.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://koz.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nba.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lfy.aibaodan.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fgs.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dgv.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bkh.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hal.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://ajc.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://djo.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fsy.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ttk.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vqa.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://vst.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://cdm.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://vuc.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://dvy.vehdjk.com

[C05] 返回多个值
来源：http://wta.shanyushiyangkeji.top

Py:   return a, b
来源：http://jjt.yongpay.top

PHP:  return [$a, $b];
来源：http://uee.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://zfe.jqgfzy.top

TS:   return { a, b };
来源：http://oxs.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vuq.xingfuxueyuan.xyz

Go:   return a, b
来源：http://rhi.snrcjt.cn

Ruby: return a, b
来源：http://gky.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ygx.tanke756.top

[C06] 匿名函数 / lambda
来源：http://urs.hnqzz.top

Py:   square = lambda x: x * x
来源：http://vor.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wau.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://jgm.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://uys.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://msm.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://zcd.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://sfq.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://myq.316326.xyz

[C07] 把函数作为参数传入
来源：http://phe.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pyo.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://iaq.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ikg.yj20258.top

TS:   arr.map(String)
来源：http://tsy.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uno.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eea.sweek.top

Ruby: arr.map(&:upcase)
来源：http://rmj.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lnn.zhaomingkeji.xyz

[C08] 闭包
来源：http://wxp.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ksz.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rlk.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ezj.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iyl.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rxe.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hoa.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lzf.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jot.xylfe.cn

[C09] 递归
来源：http://ixs.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qhl.fanxiaobao.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rgi.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mwp.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lno.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hun.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jyf.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eax.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fqd.sufxvd.cn

[C10] 变量作用域
来源：http://wif.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uln.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jir.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://enl.svipenyu.cn

TS:   同 JS
来源：http://qlb.yfazqb.com

Java: 方法内为块级作用域
来源：http://lxy.yangfankeji.com

Go:   花括号块级作用域
来源：http://oir.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://opn.shuidangran.top

C#:   块级作用域
来源：http://uap.wangdashe.top

[C11] 模块导入与导出
来源：http://kgi.vehdjk.com

Py:   from module import func
来源：http://zak.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rzz.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qqn.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nzy.gogol.net.cn

Java: import java.util.List;
来源：http://juq.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lel.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://rzy.hywenlv.cn

C#:   using System.Text;
来源：http://rzg.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://ijv.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://ixf.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://elk.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://uod.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://lyr.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ejq.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://qfl.sweek.top

Ruby: -> { puts "run" }.call
来源：http://yai.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://yyp.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://kcu.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://coh.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://acf.shanyushiyangtech.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wln.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uyi.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kga.ehwqpu.com

Go:   func add(a, b int) int
来源：http://rwb.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://boq.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://ydo.hesvh.cn

[C14] 泛型函数
来源：http://fpn.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lbb.sjlbkw.cn

PHP:  // 无泛型
来源：http://amw.dianchejie.cn

JS:   // 无泛型
来源：http://vta.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yjm.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://phr.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dhi.fengsongda.top

Ruby: # 无泛型
来源：http://znv.yonumen.top


<!-- 参考信息 -->