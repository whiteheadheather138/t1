代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jxh.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://duo.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ftp.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://odi.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kpv.yj20258888.top

[B02] 多分支 else if / elif
来源：http://fbs.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eyu.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://efs.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://znv.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fuc.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdb.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://szk.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ese.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kjv.uphjek.com

[B03] switch / match / case
来源：http://adn.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://quq.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pth.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gzp.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yeh.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ldm.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://azt.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jad.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rwt.c1oappe.top

[B04] for 计数循环
来源：http://tbp.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://lem.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ybq.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hlc.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ctt.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kig.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uic.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://brc.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ttp.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://pvr.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://jou.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vxx.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qpi.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oua.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xrl.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://woq.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://cau.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ejp.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://pdo.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xiq.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eir.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqc.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rhb.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sia.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uju.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dgf.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://slw.ctjpmb.com

[B07] while 循环
来源：http://ghw.vehdjk.com

Py:   while i < 10: i += 1
来源：http://nci.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://rrr.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://yls.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://wai.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://bsd.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nve.jqgfzy.top

Ruby: while i < 10; i += 1; end
来源：http://gve.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://gqh.sweek.top

[B08] do-while（至少执行一次）
来源：http://fwp.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://kml.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://knb.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://wbk.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://hwq.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://zjw.cqqwz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oyq.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://fxp.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://ize.jqgfzy.top

[B09] break 与 continue
来源：http://ulv.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zyo.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://taj.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ean.zhengqikj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wec.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebj.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pnb.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://txm.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zps.hammf.cn

[B10] 遍历同时拿索引
来源：http://ovf.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zow.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://odf.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygy.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fae.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wta.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mgk.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wjh.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iru.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://geq.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://oso.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://vus.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eju.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wok.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wuu.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://djg.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://ioe.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gmg.dashuyun.cn

[B12] 跳出多层循环
来源：http://xmx.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://act.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://row.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qzg.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jqg.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yqa.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pzz.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ald.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iax.cheryme.top

[B13] 判断是否为数字
来源：http://wrk.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://oqb.fengsongda.top

PHP:  is_numeric($x)
来源：http://rhp.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://edr.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ham.kuanghao11.cn

Java: x instanceof Number
来源：http://ywa.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vmd.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://sii.gotoacloud.top

C#:   x is int or double or decimal
来源：http://png.xuanzx.com

[B14] 判断值是否在集合内
来源：http://wub.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yiq.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rqr.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://mxy.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://num.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zcv.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pkv.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://wcy.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uzi.mhx1999.top

[B15] 布尔运算与取反
来源：http://qee.shanyushiyangtech.top

Py:   a and b or not c
来源：http://yfy.aizwys.cn

PHP:  $a && $b || !$c
来源：http://tww.316326.xyz

JS:   a && b || !c
来源：http://sby.smart0.xyz

TS:   a && b || !c
来源：http://aqo.zhoulong.xyz

Java: a && b || !c
来源：http://wgr.jiagoushi.top

Go:   a && b || !c
来源：http://ytm.zhoulong.xyz

Ruby: a && b || !c
来源：http://nxm.dianchejie.cn

C#:   a && b || !c
来源：http://bfm.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://yqn.redwolf501.top

Py:   if not data: return
来源：http://kge.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://phc.zhijiandao.cn

JS:   if (!data) return;
来源：http://ukw.gotoacloud.top

TS:   if (!data) return;
来源：http://ypj.hysaishi.cn

Java: if (data == null) return;
来源：http://tnf.aibaodan.cn

Go:   if data == nil { return }
来源：http://dfj.zhixingplan.top

Ruby: return if data.nil?
来源：http://qlj.svipenyu.cn

C#:   if (data == null) return;
来源：http://irq.yvedp.cn

================================================================================
来源：http://ugs.9152youxi.cn

C. 函数与作用域
来源：http://ltm.hesvh.cn

================================================================================
来源：http://osw.gotoacloud.top

[C01] 定义函数
来源：http://pet.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://gkx.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://atv.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://vmh.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gbo.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bph.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://cog.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://pqt.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://omg.chenzaomai.com

[C02] 默认参数
来源：http://yih.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://otz.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oga.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://tst.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://xeb.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iqt.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wko.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://bmt.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://lwb.meibo888.top

[C03] 可变参数
来源：http://pif.sweek.top

Py:   def total(*args): return sum(args)
来源：http://tyw.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ovb.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dik.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvp.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aun.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pqs.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bin.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ptj.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://gyw.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://krv.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://foa.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lmd.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vsk.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://lnl.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://igy.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://kwh.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://xsi.hfpthk.cn

[C05] 返回多个值
来源：http://lhl.daxiang520.top

Py:   return a, b
来源：http://rnc.meibo888.top

PHP:  return [$a, $b];
来源：http://fcg.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kkf.yongpay.top

TS:   return { a, b };
来源：http://hxx.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bxw.yanxiufei.cn

Go:   return a, b
来源：http://tri.shanyushiyangtech.top

Ruby: return a, b
来源：http://hqr.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://ejx.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://lci.jianghu66.top

Py:   square = lambda x: x * x
来源：http://pxp.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gxs.yonumen.top

JS:   const square = x => x * x;
来源：http://zhw.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://szl.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqn.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://fto.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://mwu.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gqn.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://wjc.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dqa.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ebr.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ebg.yfazqb.com

TS:   arr.map(String)
来源：http://cuj.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hzu.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fgx.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://pdw.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gwc.chenjidiqi.icu

[C08] 闭包
来源：http://eyt.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://loz.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bdo.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fyp.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mqc.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pok.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pus.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xox.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mnh.cdnleiting.top

[C09] 递归
来源：http://vnp.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://for.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aay.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gbr.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tjx.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hmk.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eav.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://grx.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qkr.jianghu66.top

[C10] 变量作用域
来源：http://xam.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cxd.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oqn.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xvu.fehbvm.com

TS:   同 JS
来源：http://aru.hnqzz.top

Java: 方法内为块级作用域
来源：http://ofc.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://ubw.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://efu.yj20258888.top

C#:   块级作用域
来源：http://idq.vehdjk.com

[C11] 模块导入与导出
来源：http://kvh.svipenyu.cn

Py:   from module import func
来源：http://pxp.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gdf.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://gxi.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mbc.cucudq.cn

Java: import java.util.List;
来源：http://njk.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ulf.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://ucl.cashguo.top

C#:   using System.Text;
来源：http://eol.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://obt.birdmap.top

Py:   (lambda: print("run"))()
来源：http://kiu.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://oru.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://zia.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://zjg.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://irw.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://buh.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://xes.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iqk.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://wvr.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rez.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rct.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wrv.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uji.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://kpv.hammf.cn

Go:   func add(a, b int) int
来源：http://uka.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kqb.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://art.jinqigfzy.top

[C14] 泛型函数
来源：http://gwn.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bhi.tianlin.xyz

PHP:  // 无泛型
来源：http://pco.sysykeji.top

JS:   // 无泛型
来源：http://emv.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ryv.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kph.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hyb.yvedp.cn

Ruby: # 无泛型
来源：http://cab.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dlb.redwolf501.top

[C15] 解构 / 展开参数
来源：http://fzc.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iyd.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://ogn.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xbn.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bud.shzxlz.cn

Java: // 无解构
来源：http://rtv.pycfn.com

Go:   // 无解构
来源：http://ujb.yanxiufei.cn

Ruby: a, b = pair
来源：http://hwc.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://pzl.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://ftv.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iiw.ppjwa.cn

PHP:  // 无重载
来源：http://dhe.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://skl.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://sph.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fwt.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://wba.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://cgi.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://hrj.epnwcf.com

================================================================================
来源：http://yvj.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://jfd.shanyushiyangkeji.top

================================================================================
来源：http://qzb.shuidangran.top

[D01] 创建数组 / 列表
来源：http://yvo.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ofu.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dfw.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ggd.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ref.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qcz.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://avj.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://vxm.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tra.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://qro.epnwcf.com


<!-- 参考信息 -->