代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://rlq.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lvh.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vox.dashuyun.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ypn.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pax.nanxinkj.top

================================================================================
来源：http://gky.0kj1m.cn

B. 流程控制
来源：http://hgm.zhongyouzk.top

================================================================================
来源：http://ntw.snrcjt.cn

[B01] 条件判断 if / else
来源：http://xto.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://piv.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rgm.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qkf.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vnv.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://shs.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tkq.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xzv.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xqo.daria6918.cn

[B02] 多分支 else if / elif
来源：http://ypp.xingfuxueyuan.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lpr.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aod.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djc.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahg.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jap.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uve.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ckx.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udr.zhengqikj.top

[B03] switch / match / case
来源：http://kmx.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qsg.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ibo.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gov.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://csu.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ika.zhoulong.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zkn.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zmc.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yag.yuanzhike.top

[B04] for 计数循环
来源：http://oig.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://yck.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nzy.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://msr.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://naa.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dtn.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xoj.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://grk.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://clx.ivvv.top

[B05] 遍历数组 / 列表
来源：http://voh.birdmap.top

Py:   for item in arr: print(item)
来源：http://jat.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jpg.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://cxa.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://svj.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tut.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://esx.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://ptt.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uar.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://thp.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vxf.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qfk.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bhy.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ajc.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xge.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sqa.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vrc.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ujp.guowangkeji.top

[B07] while 循环
来源：http://vjx.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://dst.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://ews.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://gqt.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://pwl.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://gcl.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rxr.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://uto.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://bsn.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://psv.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://qpv.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://obs.xuetiantiany.cn

JS:   do { i++; } while (i < 10);
来源：http://aol.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://vof.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://fmy.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zfk.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://crr.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://vuz.ivvv.top

[B09] break 与 continue
来源：http://uai.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ttl.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pkr.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsz.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfs.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrn.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rxl.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nma.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aew.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://fcd.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fgt.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lsj.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hvb.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oef.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ide.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oox.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zyo.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fge.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://nyd.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://rzc.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://ixr.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cij.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ecl.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xtw.nwbrower.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zev.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://yxd.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://syo.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://qdb.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://kmx.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://qzd.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xbc.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qes.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rym.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xjr.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pcl.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mfq.smart0.xyz

[B13] 判断是否为数字
来源：http://bkr.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://ngo.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://pcq.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsv.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sjb.dianchejie.cn

Java: x instanceof Number
来源：http://qvn.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yxi.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://fdl.svipenyu.cn

C#:   x is int or double or decimal
来源：http://apy.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://fqm.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jzw.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jrj.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://lwr.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://wtf.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://qff.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wkf.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://ups.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfh.0kj1m.cn

[B15] 布尔运算与取反
来源：http://gle.jianghu66.top

Py:   a and b or not c
来源：http://zdl.birdmap.top

PHP:  $a && $b || !$c
来源：http://tjq.hongshengwenyu.top

JS:   a && b || !c
来源：http://ndl.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://hgg.chenlongwang.top

Java: a && b || !c
来源：http://cbe.mhx1999.top

Go:   a && b || !c
来源：http://yuh.jiagoushi.top

Ruby: a && b || !c
来源：http://kik.wangdashe.top

C#:   a && b || !c
来源：http://zwl.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aen.fengsongda.top

Py:   if not data: return
来源：http://yld.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://nyt.shangyingyoupin.top

JS:   if (!data) return;
来源：http://ztg.wangdashe.top

TS:   if (!data) return;
来源：http://uyo.shuidangran.top

Java: if (data == null) return;
来源：http://zji.ppjwa.cn

Go:   if data == nil { return }
来源：http://ips.redwolf501.top

Ruby: return if data.nil?
来源：http://wgn.jinqigufen.top

C#:   if (data == null) return;
来源：http://uxq.zhijiandao.cn

================================================================================
来源：http://lug.shanyushiyangkeji.top

C. 函数与作用域
来源：http://aio.vehdjk.com

================================================================================
来源：http://maq.hcnkem.com

[C01] 定义函数
来源：http://rps.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://upn.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dry.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://ycv.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jxz.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://apj.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://vbf.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://vef.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://doq.zhijiandao.cn

[C02] 默认参数
来源：http://tfv.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://ytv.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fdz.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://gve.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xvw.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://oyz.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wwo.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://jfv.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://rov.dianchejie.cn

[C03] 可变参数
来源：http://zom.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://ukh.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pjh.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hgu.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pnz.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://crz.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jwf.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gaz.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fbl.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://eqd.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blr.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://izf.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tyy.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://olf.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://gdz.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://czv.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://lgy.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://tcg.jinqigufen.top

[C05] 返回多个值
来源：http://bgi.wangdashe.top

Py:   return a, b
来源：http://epd.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://avm.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ryw.sysykeji.top

TS:   return { a, b };
来源：http://sly.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ejl.dashuyun.cn

Go:   return a, b
来源：http://cah.vqdsnc.cn

Ruby: return a, b
来源：http://vhu.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://fib.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://sut.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://iyz.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ljp.yueranfly.top

JS:   const square = x => x * x;
来源：http://jaz.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://geq.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qym.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://azt.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://rpu.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://ern.yongpay.top

[C07] 把函数作为参数传入
来源：http://pxf.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kvz.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://kdw.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nlr.jqgufenzy.top

TS:   arr.map(String)
来源：http://dnw.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lck.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://unj.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://ows.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://fzo.cdnleiting.top

[C08] 闭包
来源：http://svx.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xgr.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yaf.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fqj.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tkv.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fnh.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bri.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dnm.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cmt.gotoacloud.top

[C09] 递归
来源：http://smy.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://taz.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yrg.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ahp.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://buq.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ncs.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://flo.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gfo.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jue.shanyushiyangtech.top

[C10] 变量作用域
来源：http://ise.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rpg.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lhq.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qqs.yanxiufei.cn

TS:   同 JS
来源：http://eko.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://msd.ivvv.top

Go:   花括号块级作用域
来源：http://phr.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zxi.jqgfzy.top

C#:   块级作用域
来源：http://nhi.jinqigfzy.top

[C11] 模块导入与导出
来源：http://gdp.yonumen.top

Py:   from module import func
来源：http://pps.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://msz.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hrr.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kqa.hysaishi.cn

Java: import java.util.List;
来源：http://prg.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ldl.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://wtk.dianchejie.cn

C#:   using System.Text;
来源：http://spi.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://upk.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://jfc.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://ady.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://sln.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://xat.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ziu.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://shf.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://wpm.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://foc.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://ndx.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rum.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wvg.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mxy.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gob.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://lpm.gotoacloud.top

Go:   func add(a, b int) int
来源：http://qzm.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cnr.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://bin.yvedp.cn

[C14] 泛型函数
来源：http://qze.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wsr.hesvh.cn

PHP:  // 无泛型
来源：http://qqw.yvedp.cn

JS:   // 无泛型
来源：http://kmo.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tjn.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jmc.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jwu.nanxinkj.top

Ruby: # 无泛型
来源：http://bki.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://evo.ybcxt.top

[C15] 解构 / 展开参数
来源：http://ixj.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xox.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://qtr.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cxf.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cct.dashuyun.cn

Java: // 无解构
来源：http://tfy.xuetiantiany.cn

Go:   // 无解构
来源：http://ejw.epnwcf.com

Ruby: a, b = pair
来源：http://lra.yonumen.top

C#:   var (a, b) = pair;
来源：http://xyu.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://jew.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kje.zhijiandao.cn

PHP:  // 无重载
来源：http://qgl.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ocq.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://ebu.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://kdz.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://wdl.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://fby.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://opd.yangfankeji.com

================================================================================
来源：http://lpx.cqqwz.cn


<!-- 参考信息 -->