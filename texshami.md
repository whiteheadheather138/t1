代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vvd.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://flc.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dqj.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nld.wangdashe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rkx.bbcook.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://clj.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ued.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kar.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iix.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbg.xinyue.icu

[B03] switch / match / case
来源：http://vyn.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nlz.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gwn.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lpd.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qja.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zos.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kwy.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tdu.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nic.yuxming.cn

[B04] for 计数循环
来源：http://vqs.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://xol.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jkl.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qld.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jkb.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fyf.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mnf.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://cxu.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jnv.yongpay.top

[B05] 遍历数组 / 列表
来源：http://znr.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://ofs.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ist.yongpay.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dzn.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://whc.dashuyun.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://szv.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ycg.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://ypf.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://llb.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://nek.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fag.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cvp.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsa.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kzp.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yhb.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hot.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://puv.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fwj.guannengcc.top

[B07] while 循环
来源：http://ycz.xziqi.cn

Py:   while i < 10: i += 1
来源：http://fxg.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://ntk.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://car.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://nuo.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://zbo.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hfw.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://heh.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://fmr.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://xjf.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://tbp.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cui.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://nct.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://yse.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://oho.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://lwo.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://csa.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://qxu.ctjpmb.com

[B09] break 与 continue
来源：http://ffe.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zzo.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ysk.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://koz.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggo.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://set.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://twq.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ryx.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddn.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://mym.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rbv.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zuy.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://edf.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://urp.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hsc.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://moc.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lnn.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wuh.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://qpt.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://ksv.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://wvv.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tjf.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://giv.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tbe.jinqigfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xbc.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://szy.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://onr.guowangkeji.top

[B12] 跳出多层循环
来源：http://rgy.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uhn.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://yih.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qbo.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tdd.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://boy.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mfy.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wiy.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zml.uphjek.com

[B13] 判断是否为数字
来源：http://uci.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://rdg.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://bzj.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ncu.jinqigfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sya.chenzaomai.com

Java: x instanceof Number
来源：http://oqb.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dfd.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://mhw.cqqwz.cn

C#:   x is int or double or decimal
来源：http://fnd.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://hfy.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://inj.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iem.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ltz.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://brk.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gdv.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jii.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://rtz.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tod.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://bda.jqgfzy.top

Py:   a and b or not c
来源：http://gsa.c1oappe.top

PHP:  $a && $b || !$c
来源：http://ryt.pengpengdd.cyou

JS:   a && b || !c
来源：http://fmg.quarkkingdee.top

TS:   a && b || !c
来源：http://mtg.redwolf501.top

Java: a && b || !c
来源：http://egk.hcnkem.com

Go:   a && b || !c
来源：http://xxm.jyoumei.cn

Ruby: a && b || !c
来源：http://jev.jlsjyb.cn

C#:   a && b || !c
来源：http://qyp.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://agc.9152youxi.cn

Py:   if not data: return
来源：http://lhr.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://mcf.0kj1m.cn

JS:   if (!data) return;
来源：http://uxo.shangyingyoupin.top

TS:   if (!data) return;
来源：http://jnc.yanxiufei.cn

Java: if (data == null) return;
来源：http://cka.fzhhl.top

Go:   if data == nil { return }
来源：http://kug.meibo888.top

Ruby: return if data.nil?
来源：http://yvx.shzxlz.cn

C#:   if (data == null) return;
来源：http://sbx.fzhhl.top

================================================================================
来源：http://dlq.fehbvm.com

C. 函数与作用域
来源：http://mkd.yuanzhike.top

================================================================================
来源：http://lqo.ehwqpu.com

[C01] 定义函数
来源：http://ckm.tanke756.top

Py:   def add(a, b): return a + b
来源：http://vyp.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xyt.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://oyp.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mxz.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://zta.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://kez.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://ajz.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rgw.uphjek.com

[C02] 默认参数
来源：http://rur.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://rpx.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tfo.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://skz.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rtg.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fst.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wdz.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://emn.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://cjd.bjfxy.top

[C03] 可变参数
来源：http://pov.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://wno.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cyb.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sag.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cwy.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rvb.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mas.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cpx.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cns.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://uyw.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vbl.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zhe.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pda.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sbx.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://cos.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://pwn.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://whk.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://ggd.wangdashe.top

[C05] 返回多个值
来源：http://sbm.chenzaomai.com

Py:   return a, b
来源：http://ihq.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://mjn.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://szi.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://pkl.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ocu.ydzc1.top

Go:   return a, b
来源：http://jlp.quarkkingdee.top

Ruby: return a, b
来源：http://zkc.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ryh.birdmap.top

[C06] 匿名函数 / lambda
来源：http://ggv.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://iud.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wpt.zycfv.cn

JS:   const square = x => x * x;
来源：http://isd.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://tmc.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ebc.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://xne.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://yor.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://dde.epnwcf.com

[C07] 把函数作为参数传入
来源：http://jzl.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zrz.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://oks.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://itu.yangfankeji.com

TS:   arr.map(String)
来源：http://nhb.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zkj.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mfu.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://aww.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mde.guowangkeji.top

[C08] 闭包
来源：http://orz.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dct.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://var.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://agy.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mkz.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tre.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://khw.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dyq.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kqc.pengpengdd.cyou

[C09] 递归
来源：http://ifj.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fqy.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bug.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ndr.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hne.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aby.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jfo.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oyz.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cda.chenzaomai.com

[C10] 变量作用域
来源：http://obw.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mgm.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqi.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zda.feifeiyinyue.top

TS:   同 JS
来源：http://dxl.xinyue.icu

Java: 方法内为块级作用域
来源：http://rft.yanxiufei.cn

Go:   花括号块级作用域
来源：http://vvx.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qsd.yvedp.cn

C#:   块级作用域
来源：http://ujo.xziqi.cn

[C11] 模块导入与导出
来源：http://ktg.daria6918.cn

Py:   from module import func
来源：http://bpw.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oou.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zkl.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uds.jqgufenzy.top

Java: import java.util.List;
来源：http://gql.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kuu.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://jmy.yj20258888.top

C#:   using System.Text;
来源：http://xef.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://url.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://afn.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://cce.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://sun.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://wvz.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qsp.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://kwz.sweek.top

Ruby: -> { puts "run" }.call
来源：http://wop.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ryn.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://zpo.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gvl.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gvm.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uch.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qje.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://iso.snrcjt.cn

Go:   func add(a, b int) int
来源：http://olp.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://crv.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://hqv.jinqigfzy.top

[C14] 泛型函数
来源：http://nhi.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yim.yanxiufei.cn

PHP:  // 无泛型
来源：http://upx.bjfxy.top

JS:   // 无泛型
来源：http://vic.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fui.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ncf.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kfi.cqqwz.cn

Ruby: # 无泛型
来源：http://tkx.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ogf.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://bks.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dwa.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://jju.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hjf.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tko.chenjidiqi.icu

Java: // 无解构
来源：http://ibv.meibo888.top

Go:   // 无解构
来源：http://txv.shangyingyoupin.top

Ruby: a, b = pair
来源：http://wqe.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://ooe.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://jvk.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xsl.cheryme.top

PHP:  // 无重载
来源：http://gnr.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xna.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://pza.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zga.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://hvd.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://vvw.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wdv.fzhhl.top

================================================================================
来源：http://lsb.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://pew.sufxvd.cn

================================================================================
来源：http://okf.tarul.cn

[D01] 创建数组 / 列表
来源：http://pkh.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pxt.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sib.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lrj.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://edt.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tiu.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://dsh.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://bsx.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wdo.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://zpy.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mhv.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aud.yj20258888.top

JS:   arr.push(4);
来源：http://acf.tianlin.xyz

TS:   arr.push(4);
来源：http://fry.zhiwuduotai.top


<!-- 参考信息 -->