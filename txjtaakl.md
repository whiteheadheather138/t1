代发 wailian999

[B01] 条件判断 if / else
来源：http://gpz.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xbk.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://toh.c1oappe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jdp.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iyw.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vfq.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dzo.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://inp.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://non.jianghu66.top

[B02] 多分支 else if / elif
来源：http://vje.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bay.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gvw.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gez.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zro.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jhx.nanxinkj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nrg.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://icl.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzc.yongpay.top

[B03] switch / match / case
来源：http://onv.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dfp.redwolf501.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lvg.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uqh.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lue.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hpi.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://llg.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xhf.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yuw.316326.xyz

[B04] for 计数循环
来源：http://kre.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://wos.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lpl.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kzn.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bsc.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fkp.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxs.cashguo.top

Ruby: 10.times { |i| puts i }
来源：http://jdg.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mub.yj202588.top

[B05] 遍历数组 / 列表
来源：http://lqg.pycfn.com

Py:   for item in arr: print(item)
来源：http://llc.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jmz.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dbx.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uzp.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wij.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cbj.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://boh.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qmo.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://lwy.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ejf.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qbc.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mfl.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ksc.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qlb.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dii.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qzh.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rwx.sjlbkw.cn

[B07] while 循环
来源：http://zfq.havefunace.top

Py:   while i < 10: i += 1
来源：http://xiq.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://yuk.xuetiantiany.cn

JS:   while (i < 10) { i++; }
来源：http://bgv.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://cjk.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://lki.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lkh.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://suk.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://lbi.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://qvg.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://qdt.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vrg.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://luj.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://wpy.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://isk.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://joa.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kid.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://pdm.xuetiantiany.cn

[B09] break 与 continue
来源：http://wiu.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://snh.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ntc.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vbs.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpw.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axb.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xyc.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ykq.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dea.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://kyk.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lyt.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ukz.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lti.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rug.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rap.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gle.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xbl.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sfq.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://lsz.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://bxn.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://gcl.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cka.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hei.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bai.aizwys.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sql.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://aoe.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jqc.fengsongda.top

[B12] 跳出多层循环
来源：http://mjv.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bmk.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://urb.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://laj.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://waz.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fru.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nsu.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cyj.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ihy.jyoumei.cn

[B13] 判断是否为数字
来源：http://jis.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://ltc.jianghu66.top

PHP:  is_numeric($x)
来源：http://rry.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ljt.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yjc.yuxming.cn

Java: x instanceof Number
来源：http://jny.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://muo.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://xzm.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://muc.hesvh.cn

[B14] 判断值是否在集合内
来源：http://hfx.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mfs.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nmk.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://krg.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://dej.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jgo.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bbf.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://xun.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sme.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://fpt.52xcode.cn

Py:   a and b or not c
来源：http://qsp.pycfn.com

PHP:  $a && $b || !$c
来源：http://jkk.daria6918.cn

JS:   a && b || !c
来源：http://iaq.shzxlz.cn

TS:   a && b || !c
来源：http://bej.yanxiufei.cn

Java: a && b || !c
来源：http://siu.hfpthk.cn

Go:   a && b || !c
来源：http://hug.cheryme.top

Ruby: a && b || !c
来源：http://xwg.fktsv.cn

C#:   a && b || !c
来源：http://spk.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://win.cucudq.cn

Py:   if not data: return
来源：http://drj.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://huv.yuanzhike.top

JS:   if (!data) return;
来源：http://tpt.shuidangran.top

TS:   if (!data) return;
来源：http://dpo.aizwys.cn

Java: if (data == null) return;
来源：http://ypp.c1oappe.top

Go:   if data == nil { return }
来源：http://fda.dashuyun.cn

Ruby: return if data.nil?
来源：http://cjf.tarul.cn

C#:   if (data == null) return;
来源：http://set.jlsjyb.cn

================================================================================
来源：http://htp.epnwcf.com

C. 函数与作用域
来源：http://uxt.sxryk.cn

================================================================================
来源：http://thk.xuetiantiany.cn

[C01] 定义函数
来源：http://vtt.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://fxu.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://egz.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://gls.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lhr.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://stw.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://alr.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://sso.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nyv.jqgfzy.top

[C02] 默认参数
来源：http://whh.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://cid.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jrf.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://jco.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://nly.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://rec.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rul.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://atn.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://tts.jlsjyb.cn

[C03] 可变参数
来源：http://xky.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://zsp.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dhh.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zaf.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bmk.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://okp.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jxy.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://isk.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pxp.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://oqr.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hcy.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bow.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cag.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nnn.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://xoj.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://coy.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://wxg.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://naf.shuidangran.top

[C05] 返回多个值
来源：http://drm.guowangkeji.top

Py:   return a, b
来源：http://xvf.snrcjt.cn

PHP:  return [$a, $b];
来源：http://joc.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://uik.havefunace.top

TS:   return { a, b };
来源：http://fhs.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hlv.epnwcf.com

Go:   return a, b
来源：http://isb.sufxvd.cn

Ruby: return a, b
来源：http://ril.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://jpu.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://ypc.jqgufenzy.top

Py:   square = lambda x: x * x
来源：http://cvt.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ofy.jianghu66.top

JS:   const square = x => x * x;
来源：http://kvu.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://gmt.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://brp.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://qjd.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://itr.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://ukd.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://twd.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lfx.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://yeq.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://axz.birdmap.top

TS:   arr.map(String)
来源：http://ese.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ajq.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tvf.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://cyu.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gtx.cdnleiting.top

[C08] 闭包
来源：http://ztg.fehbvm.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gir.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qez.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nse.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://asc.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lny.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://apr.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kso.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ilp.ehwqpu.com

[C09] 递归
来源：http://srl.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aci.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xah.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bkq.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dze.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://shl.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://htd.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pld.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kzf.yj20258.top

[C10] 变量作用域
来源：http://pix.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ivr.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kok.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rec.ppjwa.cn

TS:   同 JS
来源：http://pdv.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://bpx.yj202588.top

Go:   花括号块级作用域
来源：http://dlq.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ndp.gotoacloud.top

C#:   块级作用域
来源：http://kjm.cucudq.cn

[C11] 模块导入与导出
来源：http://hbj.birdmap.top

Py:   from module import func
来源：http://wqj.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jyv.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wsh.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yyp.fengsongda.top

Java: import java.util.List;
来源：http://bke.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hzf.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://dqe.vehdjk.com

C#:   using System.Text;
来源：http://jrz.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://qsl.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://yfa.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://jes.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://usc.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://ezr.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://utp.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://kxr.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://tnc.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dmn.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://apu.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wtg.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ebb.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pwz.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cho.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://ldb.zycfv.cn

Go:   func add(a, b int) int
来源：http://ixe.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gga.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://tqz.yj20258.top

[C14] 泛型函数
来源：http://xdc.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://emr.cheryme.top

PHP:  // 无泛型
来源：http://rrk.sysykeji.top

JS:   // 无泛型
来源：http://wnz.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qsx.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dwr.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qfo.snrcjt.cn

Ruby: # 无泛型
来源：http://cun.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xde.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://iwk.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mlp.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://sxt.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://usd.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://byg.cqqwz.cn

Java: // 无解构
来源：http://ogf.tianlin.xyz

Go:   // 无解构
来源：http://vcj.ydzc1.top

Ruby: a, b = pair
来源：http://zwm.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://jke.yj20258.top

[C16] 函数 / 方法重载
来源：http://vzq.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oaa.nanxinkj.top

PHP:  // 无重载
来源：http://yvp.jinqigufen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bcm.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://tmp.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://emq.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://qpx.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://vxq.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gzb.haohaochexian.top

================================================================================
来源：http://ogq.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://gfb.jinghuilouyu.cn

================================================================================
来源：http://ssn.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://hwt.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rsf.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://slv.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jgc.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rxo.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nir.gzhubu.top


<!-- 参考信息 -->