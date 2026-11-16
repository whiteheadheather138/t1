代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://peq.jianghu66.top

[B02] 多分支 else if / elif
来源：http://nte.ppjwa.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cye.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qai.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmk.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gag.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oer.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gmo.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lxp.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxo.sysykeji.top

[B03] switch / match / case
来源：http://ilv.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yss.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sox.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wkr.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rqg.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jzt.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cwu.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hav.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://trm.shanyushiyangtech.top

[B04] for 计数循环
来源：http://puq.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://dpi.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nfs.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mva.c1oappe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wnp.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ujq.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mlf.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://veq.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wip.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://ggf.yj20258888.top

Py:   for item in arr: print(item)
来源：http://fyq.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jlo.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cyy.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://zbx.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tge.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dzu.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://lbm.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rty.tanke756.top

[B06] 遍历字典 / 对象
来源：http://npl.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://lfn.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ntr.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pdr.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xme.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jhi.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jio.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wrh.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fos.jinghuilouyu.cn

[B07] while 循环
来源：http://qkz.ydzc1.top

Py:   while i < 10: i += 1
来源：http://ptw.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tir.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://ozi.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://pys.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://mcu.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qxs.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://fyv.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://ccy.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://gbh.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://jnl.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://spz.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://ape.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://gwb.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://kxf.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uhv.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://ppi.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://ugm.cheryme.top

[B09] break 与 continue
来源：http://ngb.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ipz.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://evv.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpa.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkl.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bmo.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://grp.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hxb.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxo.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://fdw.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://itm.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vmw.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ice.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fuf.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xts.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cqm.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ctu.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ers.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://alh.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://jhy.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://swn.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yri.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqt.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ekf.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ate.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://bby.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nsw.meibo888.top

[B12] 跳出多层循环
来源：http://wif.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://joj.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://kae.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qks.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbq.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xxk.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iit.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tta.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rdn.svipenyu.cn

[B13] 判断是否为数字
来源：http://yog.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://zae.jqgfzy.top

PHP:  is_numeric($x)
来源：http://loo.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ipn.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rrt.zhengqikj.top

Java: x instanceof Number
来源：http://oqv.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kqx.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://tln.ybcxt.top

C#:   x is int or double or decimal
来源：http://byf.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://rlg.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ucf.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fes.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://jso.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://lkz.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oys.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gan.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ftz.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jrm.cdnleiting.top

[B15] 布尔运算与取反
来源：http://wle.gzhubu.top

Py:   a and b or not c
来源：http://qkj.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://vxt.yj20258888.top

JS:   a && b || !c
来源：http://ssq.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://mcw.guowangkeji.top

Java: a && b || !c
来源：http://iln.ydzc1.top

Go:   a && b || !c
来源：http://cej.smart0.xyz

Ruby: a && b || !c
来源：http://qpd.yuxming.cn

C#:   a && b || !c
来源：http://zgx.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://chj.svipenyu.cn

Py:   if not data: return
来源：http://mzg.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://fmb.bjfxy.top

JS:   if (!data) return;
来源：http://xre.yanxiufei.cn

TS:   if (!data) return;
来源：http://jfl.xziqi.cn

Java: if (data == null) return;
来源：http://mjy.havefunace.top

Go:   if data == nil { return }
来源：http://zon.daria6918.cn

Ruby: return if data.nil?
来源：http://fwm.sufxvd.cn

C#:   if (data == null) return;
来源：http://nqh.gogol.net.cn

================================================================================
来源：http://ude.hnxiangtu.top

C. 函数与作用域
来源：http://vvv.hywenlv.cn

================================================================================
来源：http://jce.svipenyu.cn

[C01] 定义函数
来源：http://hya.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://yer.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dnl.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://urd.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://llw.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://omg.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://uff.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://ldr.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ymi.yfazqb.com

[C02] 默认参数
来源：http://rmc.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://voa.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vfs.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://zio.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qsn.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nnd.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://srz.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://dzl.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://pzo.haohaochexian.top

[C03] 可变参数
来源：http://wel.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://lgg.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xak.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fvm.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnj.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hif.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bvw.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qir.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pqu.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://vkr.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kxv.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nmf.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yac.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rjz.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://rbj.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://faw.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://mjy.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://qlo.mhx1999.top

[C05] 返回多个值
来源：http://mca.guowangkeji.top

Py:   return a, b
来源：http://uep.ybcxt.top

PHP:  return [$a, $b];
来源：http://jps.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qkw.yj20258888.top

TS:   return { a, b };
来源：http://vyr.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kwu.fktsv.cn

Go:   return a, b
来源：http://duq.9152youxi.cn

Ruby: return a, b
来源：http://zvy.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://qfd.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://pou.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://bib.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mpe.daria6918.cn

JS:   const square = x => x * x;
来源：http://kig.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://vlk.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xhg.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://cuk.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://ulo.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://hqa.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://byz.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kyb.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://sey.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pbg.cucudq.cn

TS:   arr.map(String)
来源：http://ubz.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ikr.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://syg.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://jpg.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://jkw.yfazqb.com

[C08] 闭包
来源：http://muf.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hkl.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pas.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cpj.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kbc.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gim.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zqd.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ynb.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kli.xingfuxueyuan.xyz

[C09] 递归
来源：http://qku.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xkx.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gbv.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://imt.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wls.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://izd.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ufz.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://abh.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://czh.hysaishi.cn

[C10] 变量作用域
来源：http://lln.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zsq.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vjp.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qoc.aibaodan.cn

TS:   同 JS
来源：http://kit.yonumen.top

Java: 方法内为块级作用域
来源：http://vll.zhengqikj.top

Go:   花括号块级作用域
来源：http://lgh.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fyk.guowangkeji.top

C#:   块级作用域
来源：http://wvb.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://utq.zycfv.cn

Py:   from module import func
来源：http://cgd.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://trq.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wjc.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zhn.xuanzx.com

Java: import java.util.List;
来源：http://sra.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://csj.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://pab.nanxinkj.top

C#:   using System.Text;
来源：http://mxf.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://bki.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://zyu.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://nid.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://ywq.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://egm.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://spu.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://pol.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://qsn.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mct.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://dtt.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ckh.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://piq.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ptf.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vaa.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rdk.uphjek.com

Go:   func add(a, b int) int
来源：http://wea.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ewm.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tjf.yuanzhike.top

[C14] 泛型函数
来源：http://pev.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xtn.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://oad.ivvv.top

JS:   // 无泛型
来源：http://lfs.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mao.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qlo.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nnl.birdmap.top

Ruby: # 无泛型
来源：http://tau.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://skh.yfazqb.com

[C15] 解构 / 展开参数
来源：http://gcb.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dya.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://ynl.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yyy.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bll.guannengcc.top

Java: // 无解构
来源：http://xks.zdqjudy.top

Go:   // 无解构
来源：http://nye.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://bkp.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://omf.hcnkem.com

[C16] 函数 / 方法重载
来源：http://rgn.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kdt.xuanzx.com

PHP:  // 无重载
来源：http://izp.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://klt.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://wzh.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ptx.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://qbb.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://udq.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://bti.pycfn.com

================================================================================
来源：http://crf.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://ind.svipenyu.cn

================================================================================
来源：http://tqm.daxiang520.top

[D01] 创建数组 / 列表
来源：http://hph.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kiw.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dal.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mrn.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://aag.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gnf.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://snr.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://luu.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ppg.sufxvd.cn

[D02] 追加元素到末尾
来源：http://coe.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blk.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pmz.zdbjq.cn

JS:   arr.push(4);
来源：http://gow.jiagoushi.top

TS:   arr.push(4);
来源：http://dol.ydzc1.top


<!-- 参考信息 -->