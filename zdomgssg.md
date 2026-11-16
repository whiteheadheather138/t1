代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://grt.mhx1999.top

[B02] 多分支 else if / elif
来源：http://hvy.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sdz.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ipj.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chf.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yuc.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kav.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://phc.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yqh.sjlbkw.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nam.pengpengdd.cyou

[B03] switch / match / case
来源：http://peu.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bbi.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lvy.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://skj.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xfr.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mux.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yve.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://six.kuanghao11.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hqq.quarkkingdee.top

[B04] for 计数循环
来源：http://knp.havefunace.top

Py:   for i in range(10): print(i)
来源：http://mzr.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://urb.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zgl.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eed.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qvr.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fnx.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://gnw.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jmh.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://cpz.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://tzg.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yqg.quarkkingdee.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ybz.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://cbf.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://arr.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://shk.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://iak.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pek.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://nms.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://srs.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pfh.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jtb.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kdd.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rvn.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://amn.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zhu.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dqm.9152youxi.cn

[B07] while 循环
来源：http://alw.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://oph.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vkr.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://kjk.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://rej.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://wbm.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pzi.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://tbs.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://ewz.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://uka.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://oyn.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://usk.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://ely.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://dyj.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://qyb.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fvz.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lvl.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://ccr.xylfe.cn

[B09] break 与 continue
来源：http://ief.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zca.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qft.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfy.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://luo.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xag.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wyr.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pzo.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jwn.hesvh.cn

[B10] 遍历同时拿索引
来源：http://gmh.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zgv.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jlu.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://swt.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zby.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pna.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mjx.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nmh.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://smp.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://pgr.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://kdh.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://wxz.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxo.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wvt.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osk.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://atf.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://gnf.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rky.yfazqb.com

[B12] 跳出多层循环
来源：http://aat.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cjr.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://spz.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oti.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iho.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gci.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bog.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ofr.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://stb.cqqwz.cn

[B13] 判断是否为数字
来源：http://fcd.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://kli.zdqjudy.top

PHP:  is_numeric($x)
来源：http://tde.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cff.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ivg.hnqzz.top

Java: x instanceof Number
来源：http://kel.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dwc.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://ulc.fengsongda.top

C#:   x is int or double or decimal
来源：http://eum.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://uah.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qzg.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sjb.zhiwuduotai.top

JS:   [1, 2, 3].includes(x)
来源：http://ibj.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zsb.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wyo.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xoe.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://qaz.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kkg.epnwcf.com

[B15] 布尔运算与取反
来源：http://bmi.sweek.top

Py:   a and b or not c
来源：http://swx.ivvv.top

PHP:  $a && $b || !$c
来源：http://rau.daxiang520.top

JS:   a && b || !c
来源：http://vqq.jiagoushi.top

TS:   a && b || !c
来源：http://zcz.hnxiangtu.top

Java: a && b || !c
来源：http://xal.bjfxy.top

Go:   a && b || !c
来源：http://ati.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://zhn.jyoumei.cn

C#:   a && b || !c
来源：http://ipg.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://yev.mhx1999.top

Py:   if not data: return
来源：http://kfp.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://nae.hywenlv.cn

JS:   if (!data) return;
来源：http://tfi.tian-w.cn

TS:   if (!data) return;
来源：http://pdp.0kj1m.cn

Java: if (data == null) return;
来源：http://aun.jyoumei.cn

Go:   if data == nil { return }
来源：http://ptz.svipenyu.cn

Ruby: return if data.nil?
来源：http://rdk.ivvv.top

C#:   if (data == null) return;
来源：http://wrf.yj20258.top

================================================================================
来源：http://ejm.dianchejie.cn

C. 函数与作用域
来源：http://eem.jinqigufen.top

================================================================================
来源：http://czd.bjfxy.top

[C01] 定义函数
来源：http://uhw.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://xsm.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmd.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://cqz.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yli.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cia.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://exg.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://hsq.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ahf.tarul.cn

[C02] 默认参数
来源：http://ywt.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://mmt.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ygp.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://zwv.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://omk.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xkn.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fzz.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://tzl.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://gnb.wangdashe.top

[C03] 可变参数
来源：http://bqq.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://vjb.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wzb.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sgu.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://axu.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uqk.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ocy.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://bqf.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://axk.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://nyi.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://acg.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qzs.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pho.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nse.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://fbb.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://ijd.andypj.xyz

Ruby: f(a: 1, b: 2)
来源：http://pra.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://zuu.ydjk.org.cn

[C05] 返回多个值
来源：http://nwh.vehdjk.com

Py:   return a, b
来源：http://sum.zycfv.cn

PHP:  return [$a, $b];
来源：http://cad.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://trb.yueranfly.top

TS:   return { a, b };
来源：http://urs.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mfx.daxiang520.top

Go:   return a, b
来源：http://qed.xuetiantiany.cn

Ruby: return a, b
来源：http://grf.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://hrn.yj202588.top

[C06] 匿名函数 / lambda
来源：http://zru.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://paf.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wxz.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://nfp.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://rbi.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ypy.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nbt.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://lql.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://yyz.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://osq.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rsk.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://vqr.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ajx.0kj1m.cn

TS:   arr.map(String)
来源：http://tdp.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pcr.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fyd.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://psg.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lvz.daria6918.cn

[C08] 闭包
来源：http://dhe.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tgt.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rss.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fex.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dhi.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://whe.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ntq.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fwg.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qsi.daria6918.cn

[C09] 递归
来源：http://smf.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://klb.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ptv.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pat.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rko.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rtx.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://csa.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dha.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eba.tanke756.top

[C10] 变量作用域
来源：http://jql.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bdi.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bvv.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://swq.shzxlz.cn

TS:   同 JS
来源：http://fmo.bjfxy.top

Java: 方法内为块级作用域
来源：http://wom.yvedp.cn

Go:   花括号块级作用域
来源：http://qsz.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qww.kuanghao11.cn

C#:   块级作用域
来源：http://nve.sxryk.cn

[C11] 模块导入与导出
来源：http://ksz.sweek.top

Py:   from module import func
来源：http://wkj.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aef.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yau.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tnk.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://qyv.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://diy.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://afm.tianlin.xyz

C#:   using System.Text;
来源：http://aqp.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://jim.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://rri.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://ovr.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://fyo.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://yyk.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ipj.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://bnj.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://uwa.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://kab.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://dwu.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fac.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jgc.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mlu.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://itj.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gne.yj20258888.top

Go:   func add(a, b int) int
来源：http://ddd.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kcc.haohaochexian.top

C#:   int Add(int a, int b) => a + b;
来源：http://teb.zhongyouzk.top

[C14] 泛型函数
来源：http://ubo.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fqj.havefunace.top

PHP:  // 无泛型
来源：http://zwy.jinghuilouyu.cn

JS:   // 无泛型
来源：http://qll.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://non.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xmq.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fjk.xinyue.icu

Ruby: # 无泛型
来源：http://chg.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jab.yuxming.cn

[C15] 解构 / 展开参数
来源：http://gvj.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tyu.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://wkj.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gaw.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ggi.hnxiangtu.top

Java: // 无解构
来源：http://seg.xinyue.icu

Go:   // 无解构
来源：http://gte.smart0.xyz

Ruby: a, b = pair
来源：http://nki.vehdjk.com

C#:   var (a, b) = pair;
来源：http://fsf.316326.xyz

[C16] 函数 / 方法重载
来源：http://zog.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://day.yueranfly.top

PHP:  // 无重载
来源：http://vtf.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ols.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://zbp.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hdj.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://mcz.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://jmm.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hqc.hcnkem.com

================================================================================
来源：http://sri.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://udz.haohaochexian.top

================================================================================
来源：http://mde.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://luy.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://coz.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mol.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dtq.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jtv.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nzo.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://gvq.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://imp.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baw.cucudq.cn

[D02] 追加元素到末尾
来源：http://dwx.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mun.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uvd.zhijiandao.cn

JS:   arr.push(4);
来源：http://cua.ppjwa.cn

TS:   arr.push(4);
来源：http://gxq.jinqigufen.top


<!-- 参考信息 -->