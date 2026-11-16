代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nwj.wangdashe.top

[B02] 多分支 else if / elif
来源：http://zzn.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lji.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cvb.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgu.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pcq.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmx.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gcp.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uta.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjy.nwbrower.top

[B03] switch / match / case
来源：http://gks.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://djc.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lbn.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jku.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxz.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://muf.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dto.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vyv.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://waw.yfazqb.com

[B04] for 计数循环
来源：http://xls.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://pgk.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ivq.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jxb.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cwg.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cjb.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uir.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://mhl.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ngn.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://woj.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://vqp.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dro.yvedp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eso.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://etp.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uvb.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ppl.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://nta.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lyj.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://dcb.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://qcc.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uwo.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qfy.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uoi.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yns.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aqy.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zyj.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wto.dianchejie.cn

[B07] while 循环
来源：http://wwz.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://vya.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vdl.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://jpi.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://ato.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://wzn.aibaodan.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sad.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://fcu.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://qpo.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://abn.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://gum.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ezb.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://noa.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://qun.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://ani.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://ikk.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://ecq.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://bkb.yonumen.top

[B09] break 与 continue
来源：http://jbr.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gdu.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fcr.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adi.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mjh.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwj.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mkf.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://god.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyu.xziqi.cn

[B10] 遍历同时拿索引
来源：http://clt.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ksq.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qcf.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ueo.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vrl.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://faj.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wuj.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pys.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yiv.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://pmy.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://mie.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://ymq.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hvn.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rcd.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pff.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nnt.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://cha.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mjy.jianghu66.top

[B12] 跳出多层循环
来源：http://psa.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://slt.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xwb.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eyp.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vkp.iojbl.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nir.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://umz.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bzm.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rwn.hnqzz.top

[B13] 判断是否为数字
来源：http://pqp.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://wfc.jinqigufen.top

PHP:  is_numeric($x)
来源：http://ziu.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zwp.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lvf.xuetiantiany.cn

Java: x instanceof Number
来源：http://zuu.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://irr.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://xvd.ybcxt.top

C#:   x is int or double or decimal
来源：http://zal.cashguo.top

[B14] 判断值是否在集合内
来源：http://rvx.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ocj.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jqg.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://vei.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://qky.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yok.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lcu.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://ccu.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zma.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://tck.zdbjq.cn

Py:   a and b or not c
来源：http://yuo.yvedp.cn

PHP:  $a && $b || !$c
来源：http://dks.hongshengwenyu.top

JS:   a && b || !c
来源：http://pkl.zhoulong.xyz

TS:   a && b || !c
来源：http://qch.ybcxt.top

Java: a && b || !c
来源：http://fwg.jinghuilouyu.cn

Go:   a && b || !c
来源：http://bpn.snrcjt.cn

Ruby: a && b || !c
来源：http://kwj.tianlin.xyz

C#:   a && b || !c
来源：http://tco.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tkj.zhiwuduotai.top

Py:   if not data: return
来源：http://uxq.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://cvx.fzhhl.top

JS:   if (!data) return;
来源：http://rlf.yueranfly.top

TS:   if (!data) return;
来源：http://idz.hywenlv.cn

Java: if (data == null) return;
来源：http://bve.ctjpmb.com

Go:   if data == nil { return }
来源：http://cve.jiagoushi.top

Ruby: return if data.nil?
来源：http://mcn.bjfxy.top

C#:   if (data == null) return;
来源：http://xvl.pengpengdd.cyou

================================================================================
来源：http://tsi.yj20258.top

C. 函数与作用域
来源：http://csj.yonumen.top

================================================================================
来源：http://bgd.cucudq.cn

[C01] 定义函数
来源：http://vuv.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://pcz.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vlo.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://rfg.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pbh.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://piq.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://xwb.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://pdt.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bwm.ybcxt.top

[C02] 默认参数
来源：http://fyx.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://qwe.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oly.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://gfe.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://utc.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://thx.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uce.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://sxa.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://xbz.smart0.xyz

[C03] 可变参数
来源：http://arc.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://vfk.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fhq.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lsu.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzn.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qyo.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ybe.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pdx.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gle.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://lbt.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uwg.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://syp.quarkkingdee.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kia.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dbg.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://vhg.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://vyo.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://wns.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://vrj.xuetiantiany.cn

[C05] 返回多个值
来源：http://pyy.shuidangran.top

Py:   return a, b
来源：http://pmo.jinqigufen.top

PHP:  return [$a, $b];
来源：http://uqu.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bqg.vqdsnc.cn

TS:   return { a, b };
来源：http://mtl.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dkp.zhijiandao.cn

Go:   return a, b
来源：http://blg.jinghuilouyu.cn

Ruby: return a, b
来源：http://gwe.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://ljh.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://lpe.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://klb.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mes.yfazqb.com

JS:   const square = x => x * x;
来源：http://lqq.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ggs.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ren.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://rfo.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://mgy.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rvs.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://jvv.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aoi.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://lqp.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lys.mhx1999.top

TS:   arr.map(String)
来源：http://kto.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ivt.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xzw.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://rgm.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jeq.svipenyu.cn

[C08] 闭包
来源：http://mnr.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bgu.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vzx.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://znz.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rgb.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hts.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mkp.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wlv.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uio.kuanghao11.cn

[C09] 递归
来源：http://sik.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zsn.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://juk.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eii.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uag.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nwb.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qok.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ebg.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cyj.sysykeji.top

[C10] 变量作用域
来源：http://lbi.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oej.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bvd.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fzb.sufxvd.cn

TS:   同 JS
来源：http://pbq.sysykeji.top

Java: 方法内为块级作用域
来源：http://kan.pycfn.com

Go:   花括号块级作用域
来源：http://vso.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jkc.hcnkem.com

C#:   块级作用域
来源：http://cbc.ctjpmb.com

[C11] 模块导入与导出
来源：http://qor.gogol.net.cn

Py:   from module import func
来源：http://iat.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://urq.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ime.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fxu.wangshuangyany.cn

Java: import java.util.List;
来源：http://wdu.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ggj.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://rak.zhixingplan.top

C#:   using System.Text;
来源：http://tyg.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://wcw.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://wbh.guannengcc.top

PHP:  (function () { echo "run"; })();
来源：http://svq.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://fps.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://oml.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ach.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://ilu.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://xgi.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lun.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://dhz.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://veo.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ghu.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ang.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jfq.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nby.hesvh.cn

Go:   func add(a, b int) int
来源：http://jel.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tzs.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://asp.hnqzz.top

[C14] 泛型函数
来源：http://gig.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://evz.hywenlv.cn

PHP:  // 无泛型
来源：http://rtz.shuidangran.top

JS:   // 无泛型
来源：http://tjz.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vgg.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gdb.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cpo.aibaodan.cn

Ruby: # 无泛型
来源：http://ffj.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bry.yongpay.top

[C15] 解构 / 展开参数
来源：http://rzx.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gjo.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://hmt.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://adx.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nfm.chenzaomai.com

Java: // 无解构
来源：http://piw.nanxuanxn.top

Go:   // 无解构
来源：http://hru.52xcode.cn

Ruby: a, b = pair
来源：http://azi.fengsongda.top

C#:   var (a, b) = pair;
来源：http://hrg.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://jmr.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uoh.sysykeji.top

PHP:  // 无重载
来源：http://hzt.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tdx.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://sdz.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://oas.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://gyy.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://vpo.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://koz.zhiwuduotai.top

================================================================================
来源：http://zvs.sweek.top

D. 数组 / 列表 / 集合
来源：http://vra.zhaomingkeji.xyz

================================================================================
来源：http://lzc.yj202588.top

[D01] 创建数组 / 列表
来源：http://wku.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pqj.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mcb.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://onf.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ota.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cjj.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://owl.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://cpa.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://axr.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://djs.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tww.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nft.haohaochexian.top

JS:   arr.push(4);
来源：http://eoe.pycfn.com

TS:   arr.push(4);
来源：http://oic.andypj.xyz


<!-- 参考信息 -->