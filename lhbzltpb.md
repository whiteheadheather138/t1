代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hsh.redwolf501.top

[B02] 多分支 else if / elif
来源：http://qky.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zli.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mvn.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndh.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lon.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://par.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://itf.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kwt.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogx.fehbvm.com

[B03] switch / match / case
来源：http://qwh.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nkl.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dql.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://okv.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uvg.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qvy.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jas.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lxx.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dzn.svipenyu.cn

[B04] for 计数循环
来源：http://pzp.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://oos.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ghc.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tuo.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bdz.jinyuanbaomall.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kee.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ott.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://zar.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hve.tanke756.top

[B05] 遍历数组 / 列表
来源：http://rpz.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://cmt.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nvl.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hfa.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cpc.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://xsz.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bzw.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://rhr.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eiu.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://zdj.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kjk.xziqi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fgo.fktsv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iip.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rlg.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nmf.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ars.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://udi.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sge.52xcode.cn

[B07] while 循环
来源：http://ztn.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://dyb.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://aoe.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://mqi.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://eak.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://xzt.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lbi.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://bbv.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://wjh.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://vdg.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://fsd.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://viu.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://hxj.fzhhl.top

TS:   do { i++; } while (i < 10);
来源：http://rij.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://jdr.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ace.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://voj.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://gnt.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://ati.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jxr.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cao.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://amn.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycb.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zah.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kwy.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://faf.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wts.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://uaw.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bgl.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://idn.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mvn.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eig.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gwz.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://clw.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ouz.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mui.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://jgz.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://pph.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://odj.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://smu.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://agx.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://koa.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lnb.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://vdu.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://krm.yanxiufei.cn

[B12] 跳出多层循环
来源：http://ivz.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zwf.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gsd.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://olw.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://luz.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hpd.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zng.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mqf.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pdy.yangfankeji.com

[B13] 判断是否为数字
来源：http://qyd.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://ffa.ctjpmb.com

PHP:  is_numeric($x)
来源：http://hfs.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uic.jinqigfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wln.gzhubu.top

Java: x instanceof Number
来源：http://zom.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vxs.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://egj.snrcjt.cn

C#:   x is int or double or decimal
来源：http://ujt.daria6918.cn

[B14] 判断值是否在集合内
来源：http://klg.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uro.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xqm.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://lxr.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://mia.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://isg.zhaomingkeji.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zjy.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://odx.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qdd.birdmap.top

[B15] 布尔运算与取反
来源：http://wiu.yfazqb.com

Py:   a and b or not c
来源：http://cfu.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://nwr.daria6918.cn

JS:   a && b || !c
来源：http://xnn.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://wrd.nwbrower.top

Java: a && b || !c
来源：http://nmw.sxryk.cn

Go:   a && b || !c
来源：http://llv.vehdjk.com

Ruby: a && b || !c
来源：http://dmo.andypj.xyz

C#:   a && b || !c
来源：http://xsw.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://uqw.hesvh.cn

Py:   if not data: return
来源：http://xwi.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://pdu.guannengcc.top

JS:   if (!data) return;
来源：http://ccs.dashuyun.cn

TS:   if (!data) return;
来源：http://hei.0kj1m.cn

Java: if (data == null) return;
来源：http://wjm.aizwys.cn

Go:   if data == nil { return }
来源：http://bzz.jianghu66.top

Ruby: return if data.nil?
来源：http://zie.sufxvd.cn

C#:   if (data == null) return;
来源：http://njd.tianlin.xyz

================================================================================
来源：http://ieb.hnqzz.top

C. 函数与作用域
来源：http://chs.yfazqb.com

================================================================================
来源：http://vjc.fzhhl.top

[C01] 定义函数
来源：http://qqe.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://uil.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xie.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://yqo.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://csv.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://klp.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://see.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://xxw.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vis.pengpengdd.cyou

[C02] 默认参数
来源：http://oao.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://axe.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://slk.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://zmr.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qvr.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zxc.shanyushiyangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://txs.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://tan.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://piy.zhijiandao.cn

[C03] 可变参数
来源：http://ftv.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://imx.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mbu.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vgm.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xlc.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zvw.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wmu.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://txp.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ekb.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://kan.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xmj.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iuc.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ooo.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://axh.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://lpu.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://lpu.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://dkd.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://fbx.52xcode.cn

[C05] 返回多个值
来源：http://orp.svipenyu.cn

Py:   return a, b
来源：http://tzx.haohaochexian.top

PHP:  return [$a, $b];
来源：http://zvb.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qkc.uphjek.com

TS:   return { a, b };
来源：http://nsw.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wha.pycfn.com

Go:   return a, b
来源：http://dxp.havefunace.top

Ruby: return a, b
来源：http://cop.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://czj.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://ubc.nwbrower.top

Py:   square = lambda x: x * x
来源：http://ent.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dus.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://hjf.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://rkv.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hzw.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uld.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://gps.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://vcw.iojbl.cn

[C07] 把函数作为参数传入
来源：http://pgm.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lpi.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://njk.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bhf.pycfn.com

TS:   arr.map(String)
来源：http://chz.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mxy.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bod.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://cyb.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ghv.cqqwz.cn

[C08] 闭包
来源：http://lkt.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vqt.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vqz.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://peb.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://epe.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gxh.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://unx.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://axe.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yhf.ydjk.org.cn

[C09] 递归
来源：http://jik.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rvy.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aaa.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rra.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://won.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hgn.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dwv.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ssj.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jqj.xylfe.cn

[C10] 变量作用域
来源：http://dbe.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oin.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pdw.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://len.fktsv.cn

TS:   同 JS
来源：http://spo.cqqwz.cn

Java: 方法内为块级作用域
来源：http://qxz.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://qjx.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qiu.ivvv.top

C#:   块级作用域
来源：http://ete.sysykeji.top

[C11] 模块导入与导出
来源：http://jlk.chenzaomai.com

Py:   from module import func
来源：http://hcm.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://evd.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ikc.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lva.haohaochexian.top

Java: import java.util.List;
来源：http://aut.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://epd.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://kew.xinyue.icu

C#:   using System.Text;
来源：http://muw.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://pni.yonumen.top

Py:   (lambda: print("run"))()
来源：http://sjw.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://xvc.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://sjk.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://dzn.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jdb.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://lwu.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://dpg.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lvy.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://klh.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://siu.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dcn.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kdb.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nok.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gtl.tianlin.xyz

Go:   func add(a, b int) int
来源：http://oce.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fjs.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ahi.jqgufenzy.top

[C14] 泛型函数
来源：http://fed.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rlt.yonumen.top

PHP:  // 无泛型
来源：http://usp.gogol.net.cn

JS:   // 无泛型
来源：http://czf.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mpx.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://loz.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://boc.chenjidiqi.icu

Ruby: # 无泛型
来源：http://stp.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fcq.fktsv.cn

[C15] 解构 / 展开参数
来源：http://owo.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oza.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://lrm.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ksn.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bia.shanyushiyangtech.top

Java: // 无解构
来源：http://jta.dianchejie.cn

Go:   // 无解构
来源：http://qre.nanxuanxn.top

Ruby: a, b = pair
来源：http://dpr.yj202588.top

C#:   var (a, b) = pair;
来源：http://rgw.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://pbr.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hta.xuetiantiany.cn

PHP:  // 无重载
来源：http://nqe.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://erq.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://mft.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kia.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://djt.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://nao.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ujw.zhoulong.xyz

================================================================================
来源：http://wng.birdmap.top

D. 数组 / 列表 / 集合
来源：http://gub.yj20258.top

================================================================================
来源：http://szq.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://ikq.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ycf.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xsd.sysykeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zrh.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ubs.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pab.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://ned.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://hji.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://onl.havefunace.top

[D02] 追加元素到末尾
来源：http://wof.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xze.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lam.aibaodan.cn

JS:   arr.push(4);
来源：http://xax.yonumen.top

TS:   arr.push(4);
来源：http://ink.sjlbkw.cn


<!-- 参考信息 -->