代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mxm.yvedp.cn

[B02] 多分支 else if / elif
来源：http://adb.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rgr.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wti.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqy.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgb.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mym.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://psa.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kru.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezv.jqgfzy.top

[B03] switch / match / case
来源：http://vbz.jinqigufen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eit.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rud.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://guk.yj202588.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sxa.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hcr.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fhe.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tsp.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ggp.jinghuilouyu.cn

[B04] for 计数循环
来源：http://yhn.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://psz.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fco.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://brk.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znr.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gif.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bim.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://aoy.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xqw.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://jyt.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://fsu.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tty.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rhe.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://soa.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gpw.redwolf501.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ume.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://tfs.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oiy.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://clj.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qki.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lug.tanke756.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zco.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ggp.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://igt.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aai.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bwu.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gat.redwolf501.top

[B07] while 循环
来源：http://zwz.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://sxx.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://bol.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://cjy.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://rzb.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://kej.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gty.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://sew.sxryk.cn

C#:   while (i < 10) { i++; }
来源：http://qps.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://gbw.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://xuj.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aof.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://vfi.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://xwr.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://asb.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ezq.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://vdt.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://cpm.yfazqb.com

[B09] break 与 continue
来源：http://gic.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dee.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fpr.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hei.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gmr.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://red.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hqt.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qaq.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pmg.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://gnf.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mdc.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://twq.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ejf.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kya.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mxj.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aoo.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tbh.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qdu.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://skx.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://sxr.yj202588.top

PHP:  range(0, 10, 2);
来源：http://buh.shangyingyoupin.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zdl.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gad.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ncu.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qnz.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://mfj.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://deb.tian-w.cn

[B12] 跳出多层循环
来源：http://idz.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://utv.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://amd.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfw.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mny.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kba.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://irc.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ovu.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blq.xylfe.cn

[B13] 判断是否为数字
来源：http://bjo.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://iti.xuanzx.com

PHP:  is_numeric($x)
来源：http://nlp.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pqs.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://izl.jqgufenzy.top

Java: x instanceof Number
来源：http://qua.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rqi.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://ref.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://ztw.iojbl.cn

[B14] 判断值是否在集合内
来源：http://osp.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gcm.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bbp.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://psr.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://pzl.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cnd.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mkg.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wyo.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nls.daria6918.cn

[B15] 布尔运算与取反
来源：http://zie.daxiang520.top

Py:   a and b or not c
来源：http://stw.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://uzf.redwolf501.top

JS:   a && b || !c
来源：http://gch.aibaodan.cn

TS:   a && b || !c
来源：http://rid.tarul.cn

Java: a && b || !c
来源：http://dqu.hnqzz.top

Go:   a && b || !c
来源：http://esn.hnxiangtu.top

Ruby: a && b || !c
来源：http://bvy.chenzaomai.com

C#:   a && b || !c
来源：http://ajs.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hbd.chenjidiqi.icu

Py:   if not data: return
来源：http://jlv.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://wjs.ydzc1.top

JS:   if (!data) return;
来源：http://eif.tarul.cn

TS:   if (!data) return;
来源：http://cxc.yangfankeji.com

Java: if (data == null) return;
来源：http://asx.birdmap.top

Go:   if data == nil { return }
来源：http://zqa.yuanzhike.top

Ruby: return if data.nil?
来源：http://yob.daria6918.cn

C#:   if (data == null) return;
来源：http://pkb.sjlbkw.cn

================================================================================
来源：http://lbw.hywenlv.cn

C. 函数与作用域
来源：http://ont.gaohongyu789.top

================================================================================
来源：http://sdj.feifeiyinyue.top

[C01] 定义函数
来源：http://nyr.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://xem.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wei.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://wmp.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ibn.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tvc.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://upq.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://akf.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://asx.yangfankeji.com

[C02] 默认参数
来源：http://fbe.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://pqm.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kfv.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://tvo.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://bnb.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ajq.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rmd.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://fui.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://ctq.316326.xyz

[C03] 可变参数
来源：http://xfm.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://cpc.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rxg.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hau.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qbl.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zcu.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pyl.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kqg.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ece.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://veg.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qmz.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aoi.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bcp.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://exy.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://eqv.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://mvs.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://tdu.sweek.top

C#:   f(a: 1, b: 2)
来源：http://fjb.sxryk.cn

[C05] 返回多个值
来源：http://oqs.jqgfzy.top

Py:   return a, b
来源：http://ecq.bjfxy.top

PHP:  return [$a, $b];
来源：http://sbn.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bqf.shanyushiyangtech.top

TS:   return { a, b };
来源：http://izj.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ysb.sufxvd.cn

Go:   return a, b
来源：http://cjo.gzhubu.top

Ruby: return a, b
来源：http://qel.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ajc.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://wqi.hesvh.cn

Py:   square = lambda x: x * x
来源：http://rba.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ija.0kj1m.cn

JS:   const square = x => x * x;
来源：http://jxl.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://dno.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iub.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dxx.ppjwa.cn

Ruby: square = ->(x) { x * x }
来源：http://mpw.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lwv.sysykeji.top

[C07] 把函数作为参数传入
来源：http://gml.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hht.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://blz.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hec.cdnleiting.top

TS:   arr.map(String)
来源：http://eco.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nob.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sci.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://lzv.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rra.zhijiandao.cn

[C08] 闭包
来源：http://lea.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tog.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://raz.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wbs.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cde.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ner.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kes.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gki.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wpu.fktsv.cn

[C09] 递归
来源：http://qqs.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cyk.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cla.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ywj.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bzf.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bev.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://imd.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ipk.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fsc.yuxming.cn

[C10] 变量作用域
来源：http://cru.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qxp.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ewr.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dni.cashguo.top

TS:   同 JS
来源：http://jxw.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://dgv.nwbrower.top

Go:   花括号块级作用域
来源：http://bgj.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://waq.hcnkem.com

C#:   块级作用域
来源：http://uui.svipenyu.cn

[C11] 模块导入与导出
来源：http://ean.hongshengwenyu.top

Py:   from module import func
来源：http://glw.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pzq.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hvn.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uwz.xuetiantiany.cn

Java: import java.util.List;
来源：http://ghb.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ouh.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://qgl.ydjk.org.cn

C#:   using System.Text;
来源：http://odk.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://skt.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://jwq.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://lhn.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://hcz.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://ztp.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://chs.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://laz.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://eao.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jzf.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://qaq.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bjz.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://owo.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://swe.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://viq.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://vbm.dashuyun.cn

Go:   func add(a, b int) int
来源：http://lex.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qsg.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://gon.wangdashe.top

[C14] 泛型函数
来源：http://hht.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://owc.daxiang520.top

PHP:  // 无泛型
来源：http://hwr.yonumen.top

JS:   // 无泛型
来源：http://tsu.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://efj.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yxx.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ggc.gzhubu.top

Ruby: # 无泛型
来源：http://vbh.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://art.cashguo.top

[C15] 解构 / 展开参数
来源：http://wgy.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ied.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://hez.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nsj.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hmd.fktsv.cn

Java: // 无解构
来源：http://dsj.jinqigufen.top

Go:   // 无解构
来源：http://vhx.vqdsnc.cn

Ruby: a, b = pair
来源：http://lql.fzhhl.top

C#:   var (a, b) = pair;
来源：http://luv.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://bdj.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jme.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://rpy.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://otn.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://dgg.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://akz.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://uld.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://alh.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qbn.yongpay.top

================================================================================
来源：http://gpq.yj20258.top

D. 数组 / 列表 / 集合
来源：http://bmo.shuidangran.top

================================================================================
来源：http://ggk.nwbrower.top

[D01] 创建数组 / 列表
来源：http://rmu.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://kit.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://coo.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rcl.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pec.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aka.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://czz.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://zxf.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aih.gogol.net.cn

[D02] 追加元素到末尾
来源：http://bkx.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zsl.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://luc.cdnleiting.top

JS:   arr.push(4);
来源：http://pno.ivvv.top

TS:   arr.push(4);
来源：http://krk.ydjk.org.cn


<!-- 参考信息 -->