代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://pck.havefunace.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://exb.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmh.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gbj.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zcp.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zlm.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dfy.havefunace.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kxg.hysaishi.cn

[A26] 类型转换总览
来源：http://xsn.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rvp.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nvt.cqqwz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zhj.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://rwj.wangdashe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qim.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://shl.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://imy.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fxl.cheryme.top

================================================================================
来源：http://giq.ydzc1.top

B. 流程控制
来源：http://iqv.xingfuxueyuan.xyz

================================================================================
来源：http://hrn.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://ghg.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vej.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ltz.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kuc.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lvy.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uof.nanxuanxn.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hbq.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xku.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dhz.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://jkx.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aar.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tjr.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iip.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dna.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rib.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ppf.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fxr.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://car.redwolf501.top

[B03] switch / match / case
来源：http://miz.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vdp.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lat.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jtj.52xcode.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://soj.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mwc.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ptl.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uyx.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://slw.ydzc1.top

[B04] for 计数循环
来源：http://xrh.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://fdm.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jxg.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://auk.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mgo.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ail.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rfe.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://lui.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vpc.316326.xyz

[B05] 遍历数组 / 列表
来源：http://vld.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://zfs.bjfxy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tan.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://taa.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nhf.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://idh.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wcs.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://lee.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ico.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://elh.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gvy.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mpe.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://usx.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eot.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vhe.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gcb.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://anf.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xka.kuanghao11.cn

[B07] while 循环
来源：http://tnp.yj202588.top

Py:   while i < 10: i += 1
来源：http://mjs.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://npv.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://fiw.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://vqm.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://brp.snrcjt.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pkm.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://dqq.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://fhb.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://ifz.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://llq.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sal.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://tdv.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://xhq.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://zua.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nkr.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://eoz.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://nux.zhengqikj.top

[B09] break 与 continue
来源：http://vkc.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pdd.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hxb.chenlongwang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dis.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://agp.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxq.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gsp.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gth.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yph.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://dkn.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zgv.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wdx.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ptk.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qhe.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xoy.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nwl.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ggr.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yfe.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://ukw.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://kpl.meibo888.top

PHP:  range(0, 10, 2);
来源：http://vkk.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bkh.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ngc.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bur.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kns.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://kax.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://azw.yanxiufei.cn

[B12] 跳出多层循环
来源：http://ngz.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qdx.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rpn.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvp.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://srw.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oas.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jbn.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://agm.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ejn.zhengqikj.top

[B13] 判断是否为数字
来源：http://kzu.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://kbj.0kj1m.cn

PHP:  is_numeric($x)
来源：http://fji.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vmj.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cjj.meibo888.top

Java: x instanceof Number
来源：http://une.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qsq.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://vys.hesvh.cn

C#:   x is int or double or decimal
来源：http://bty.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://ykr.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ska.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oua.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://szq.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://inl.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://vaz.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xuc.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://apl.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://psq.yvedp.cn

[B15] 布尔运算与取反
来源：http://qld.fehbvm.com

Py:   a and b or not c
来源：http://ahj.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://qps.snrcjt.cn

JS:   a && b || !c
来源：http://enc.xuanzx.com

TS:   a && b || !c
来源：http://czc.snrcjt.cn

Java: a && b || !c
来源：http://cto.tian-w.cn

Go:   a && b || !c
来源：http://peb.tianlin.xyz

Ruby: a && b || !c
来源：http://wlk.aibaodan.cn

C#:   a && b || !c
来源：http://gju.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://uwo.jinqigufen.top

Py:   if not data: return
来源：http://eul.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://vsk.bbcook.cn

JS:   if (!data) return;
来源：http://fhe.fzhhl.top

TS:   if (!data) return;
来源：http://kgr.havefunace.top

Java: if (data == null) return;
来源：http://gpx.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://ysy.sxryk.cn

Ruby: return if data.nil?
来源：http://foj.andypj.xyz

C#:   if (data == null) return;
来源：http://alc.zdqjudy.top

================================================================================
来源：http://nzn.sxryk.cn

C. 函数与作用域
来源：http://ybs.ehwqpu.com

================================================================================
来源：http://cbp.mhx1999.top

[C01] 定义函数
来源：http://jek.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://svf.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ara.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://xwu.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdg.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zrb.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://anb.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://nxt.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rxd.zhixingplan.top

[C02] 默认参数
来源：http://xcg.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://ygn.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qnb.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://zru.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xnj.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://owh.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dgl.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://vih.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://gsx.vehdjk.com

[C03] 可变参数
来源：http://zdx.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://ong.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tia.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ghu.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cfz.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ham.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://url.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://lrj.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yuj.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://eny.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jde.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ycz.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://agq.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fri.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://cli.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://hmw.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://nkn.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://glh.ydzc1.top

[C05] 返回多个值
来源：http://owj.zhengqikj.top

Py:   return a, b
来源：http://kqq.sysykeji.top

PHP:  return [$a, $b];
来源：http://oym.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oek.birdmap.top

TS:   return { a, b };
来源：http://sgu.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lhe.wangdashe.top

Go:   return a, b
来源：http://uco.0kj1m.cn

Ruby: return a, b
来源：http://ckp.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://uuy.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://ben.yj202588.top

Py:   square = lambda x: x * x
来源：http://wcy.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pwa.hysaishi.cn

JS:   const square = x => x * x;
来源：http://ahg.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://hbr.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bjx.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://svo.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://jmf.ywan-chungtsiang.top

C#:   Func<int, int> square = x => x * x;
来源：http://ydk.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://umd.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jot.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://bwi.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pua.snrcjt.cn

TS:   arr.map(String)
来源：http://rri.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jjm.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://caf.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://ozj.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://iwp.bjfxy.top

[C08] 闭包
来源：http://tpu.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vuk.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jwr.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ngd.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vht.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://noo.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://drv.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wab.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qan.jyoumei.cn

[C09] 递归
来源：http://lzr.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://itv.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ytl.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kci.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://elb.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oqy.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vsw.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mhw.zycfv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xrw.sysykeji.top

[C10] 变量作用域
来源：http://evp.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ukb.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ujf.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bvo.jinqigufen.top

TS:   同 JS
来源：http://icb.jinqigufen.top

Java: 方法内为块级作用域
来源：http://jsd.hywenlv.cn

Go:   花括号块级作用域
来源：http://dmg.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cdq.quarkkingdee.top

C#:   块级作用域
来源：http://fmz.yuxming.cn

[C11] 模块导入与导出
来源：http://lyq.jinghuilouyu.cn

Py:   from module import func
来源：http://ykg.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yes.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://neb.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ais.zycfv.cn

Java: import java.util.List;
来源：http://iqo.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vzj.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://kyw.xziqi.cn

C#:   using System.Text;
来源：http://ywr.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://fxa.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://gef.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://zsc.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://xqy.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://tck.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jrm.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://css.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://yow.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zny.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://onj.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://joh.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xks.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ibw.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fpd.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://neh.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://uuu.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bwa.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://bvj.jqgfzy.top

[C14] 泛型函数
来源：http://nmt.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wxa.xziqi.cn

PHP:  // 无泛型
来源：http://nxj.fktsv.cn

JS:   // 无泛型
来源：http://ddg.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ruc.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zut.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ujc.kuanghao11.cn

Ruby: # 无泛型
来源：http://kfz.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ewc.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://obh.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xyf.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://mbm.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xiz.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dmi.cqqwz.cn

Java: // 无解构
来源：http://pem.zhiwuduotai.top

Go:   // 无解构
来源：http://ufl.ctjpmb.com


<!-- 参考信息 -->