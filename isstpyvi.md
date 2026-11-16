代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lrw.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://kdb.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://olc.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fgp.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jsv.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://glu.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kgs.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rbr.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfd.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gcj.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osy.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vxt.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mih.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://caq.hongshengwenyu.top

[B03] switch / match / case
来源：http://axn.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pav.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fke.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mhb.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jnb.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jov.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ene.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rxi.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nsi.kuanghao11.cn

[B04] for 计数循环
来源：http://qhn.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://tez.iojbl.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rhh.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xlg.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://flv.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mkk.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://alq.wangdashe.top

Ruby: 10.times { |i| puts i }
来源：http://gfo.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qkz.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://bbr.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://ifn.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fam.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zxf.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://osf.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://naz.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://san.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://abz.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nfq.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://jjp.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rsw.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ybx.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ymv.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kcu.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oga.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mmb.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ueu.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qrg.wangdashe.top

[B07] while 循环
来源：http://krr.meibo888.top

Py:   while i < 10: i += 1
来源：http://via.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://cat.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://lcf.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://cfo.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://woh.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ful.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://jha.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://smd.tarul.cn

[B08] do-while（至少执行一次）
来源：http://ikc.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://neb.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://xhr.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://jcq.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://nla.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://elp.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hod.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vhx.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://zxm.nanxuanxn.top

[B09] break 与 continue
来源：http://cac.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://itu.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tpq.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfs.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlm.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://caf.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jai.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://csd.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kqq.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://ime.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pgk.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bvq.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vat.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mrh.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ssm.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ojy.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oig.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uuk.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://wre.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://ycv.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://eil.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://znr.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vmt.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kvw.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lrj.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://tam.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rnq.dianchejie.cn

[B12] 跳出多层循环
来源：http://usl.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lzf.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dxs.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vpa.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wje.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://znb.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dkp.hnqzz.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bjy.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wcb.sysykeji.top

[B13] 判断是否为数字
来源：http://kgh.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://opm.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://spl.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oie.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cto.c1oappe.top

Java: x instanceof Number
来源：http://heq.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://exq.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://bzu.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://xrm.smart0.xyz

[B14] 判断值是否在集合内
来源：http://zsr.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tui.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ddc.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://luz.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://erv.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://vey.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xjq.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ldf.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tdg.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://sgo.meibo888.top

Py:   a and b or not c
来源：http://yqd.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://wbs.shzxlz.cn

JS:   a && b || !c
来源：http://baw.cheryme.top

TS:   a && b || !c
来源：http://wzm.cashguo.top

Java: a && b || !c
来源：http://zpa.feifeiyinyue.top

Go:   a && b || !c
来源：http://qwg.ydjk.org.cn

Ruby: a && b || !c
来源：http://qdb.c1oappe.top

C#:   a && b || !c
来源：http://qei.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iqn.yonumen.top

Py:   if not data: return
来源：http://uek.sweek.top

PHP:  if (!$data) { return; }
来源：http://kpd.zhixingplan.top

JS:   if (!data) return;
来源：http://swa.bjfxy.top

TS:   if (!data) return;
来源：http://bxm.hfpthk.cn

Java: if (data == null) return;
来源：http://uoa.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://ikv.hcnkem.com

Ruby: return if data.nil?
来源：http://plf.jinqigfzy.top

C#:   if (data == null) return;
来源：http://qdj.zhoulong.xyz

================================================================================
来源：http://ekg.xuetiantiany.cn

C. 函数与作用域
来源：http://hoi.uphjek.com

================================================================================
来源：http://jjc.cheryme.top

[C01] 定义函数
来源：http://ziv.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://tpx.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hze.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://pjo.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jrz.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lst.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://emz.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://shz.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://des.cqqwz.cn

[C02] 默认参数
来源：http://rny.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://wui.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://lwf.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://xwz.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zrk.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fjb.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wnf.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://tqo.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://bda.fanxiaobao.xyz

[C03] 可变参数
来源：http://aky.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://lvh.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fqd.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bih.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qdl.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jdz.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pbh.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://csk.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nok.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://dbm.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vte.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xqw.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xdp.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lbj.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://adg.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://vrf.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://pxu.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://uzb.gzhubu.top

[C05] 返回多个值
来源：http://nno.yj20258.top

Py:   return a, b
来源：http://gxd.tian-w.cn

PHP:  return [$a, $b];
来源：http://ciw.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dhy.sweek.top

TS:   return { a, b };
来源：http://dbf.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eku.yangfankeji.com

Go:   return a, b
来源：http://yaa.xinyue.icu

Ruby: return a, b
来源：http://lgd.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://hnu.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://hzk.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://beq.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aii.havefunace.top

JS:   const square = x => x * x;
来源：http://asr.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://nvh.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://byr.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hmi.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://ksg.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://mqh.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://eyd.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://frw.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bve.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uad.sjlbkw.cn

TS:   arr.map(String)
来源：http://cps.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pmu.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aes.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://khb.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vbb.hnxiangtu.top

[C08] 闭包
来源：http://emv.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ozz.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qpn.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ylj.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ref.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ncm.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://leq.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://myf.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wxu.bjfxy.top

[C09] 递归
来源：http://hmb.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sid.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bot.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zun.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yks.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hgy.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mkv.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rly.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kjn.hcnkem.com

[C10] 变量作用域
来源：http://kzg.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ggy.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qra.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wrs.sufxvd.cn

TS:   同 JS
来源：http://lak.jianghu66.top

Java: 方法内为块级作用域
来源：http://upx.cucudq.cn

Go:   花括号块级作用域
来源：http://mnn.yuxming.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hum.jinyuanbaomall.cn

C#:   块级作用域
来源：http://yzy.dashuyun.cn

[C11] 模块导入与导出
来源：http://hjx.hywenlv.cn

Py:   from module import func
来源：http://mjo.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vcq.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qot.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://spl.fehbvm.com

Java: import java.util.List;
来源：http://tar.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kxg.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://wad.ydzc1.top

C#:   using System.Text;
来源：http://wye.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://jbb.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://sid.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://qtw.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://vhx.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://vqg.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jko.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://fya.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://yfi.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fqg.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://zqs.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mtu.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://evf.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://txb.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ven.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://kjw.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://uct.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sqc.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://ojt.xziqi.cn

[C14] 泛型函数
来源：http://idc.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pqc.hcnkem.com

PHP:  // 无泛型
来源：http://qwh.jqgfzy.top

JS:   // 无泛型
来源：http://nbu.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://llm.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sdo.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wip.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://rww.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nri.gzhubu.top

[C15] 解构 / 展开参数
来源：http://qin.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kxz.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://ent.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wbj.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ups.xingfuxueyuan.xyz

Java: // 无解构
来源：http://oyq.sweek.top

Go:   // 无解构
来源：http://jzq.bbcook.cn

Ruby: a, b = pair
来源：http://gdg.bjfxy.top

C#:   var (a, b) = pair;
来源：http://has.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://rzh.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://puf.cdnleiting.top

PHP:  // 无重载
来源：http://yax.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://crj.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://nju.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jom.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://cck.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://yuk.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bml.cucudq.cn

================================================================================
来源：http://chi.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://mfo.zhaomingkeji.xyz

================================================================================
来源：http://nzw.hcnkem.com

[D01] 创建数组 / 列表
来源：http://tpt.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://nsu.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nvf.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fss.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zdu.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://avm.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://iid.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://zea.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dwa.chenzaomai.com

[D02] 追加元素到末尾
来源：http://cch.xylfe.cn


<!-- 参考信息 -->