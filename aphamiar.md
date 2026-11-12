代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://klg.nanxuanxn.top

================================================================================
来源：http://knl.9152youxi.cn

B. 流程控制
来源：http://zkr.zdbjq.cn

================================================================================
来源：http://xla.chenlongwang.top

[B01] 条件判断 if / else
来源：http://ana.vqdsnc.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://daj.tian-w.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xsi.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zdp.yueranfly.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pik.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ogi.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lvr.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ajc.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://efn.ybcxt.top

[B02] 多分支 else if / elif
来源：http://lbh.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hza.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://joj.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpu.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tsi.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufv.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://idw.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lrl.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xco.haohaochexian.top

[B03] switch / match / case
来源：http://brp.gotoacloud.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blm.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rng.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rgc.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pqg.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lgm.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hoy.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nmf.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bff.yvedp.cn

[B04] for 计数循环
来源：http://iyq.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://yfq.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hli.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znw.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ijo.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ren.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qwl.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://gka.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eoy.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://ovc.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://xhn.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jzv.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qyt.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qlx.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dsk.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wgr.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://flr.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vvl.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://vst.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cbi.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sso.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypy.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agj.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hcn.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ove.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://opt.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xuq.jlsjyb.cn

[B07] while 循环
来源：http://uxd.pycfn.com

Py:   while i < 10: i += 1
来源：http://qie.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://ztx.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://yzl.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://hrj.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://jhb.snrcjt.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hpw.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://qcy.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://tdv.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://siw.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://vyg.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://xcm.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://gfe.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://gja.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://irg.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://qoa.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://gtf.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://kuw.chenzaomai.com

[B09] break 与 continue
来源：http://pym.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hhm.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ikj.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycm.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fei.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wnv.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ito.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xjq.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qct.yuxming.cn

[B10] 遍历同时拿索引
来源：http://omr.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://awb.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ngi.snrcjt.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zre.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ntv.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://avd.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wio.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cvh.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hsh.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://uyv.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://dhh.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://fva.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://umq.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bsr.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kri.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://myc.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://dfk.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lid.pycfn.com

[B12] 跳出多层循环
来源：http://ihw.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://hkq.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vbx.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uya.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rhy.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mdm.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dvt.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dqd.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tzx.gogol.net.cn

[B13] 判断是否为数字
来源：http://pkb.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://yjf.snrcjt.cn

PHP:  is_numeric($x)
来源：http://yjz.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jwe.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bbl.smart0.xyz

Java: x instanceof Number
来源：http://xsr.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qgl.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://sxn.haohaochexian.top

C#:   x is int or double or decimal
来源：http://dsd.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://ahp.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nlp.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nze.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://mgp.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://aqb.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pyj.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rag.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://lbk.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cum.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://fcb.tian-w.cn

Py:   a and b or not c
来源：http://oax.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://xox.kuanghao11.cn

JS:   a && b || !c
来源：http://wep.birdmap.top

TS:   a && b || !c
来源：http://gtx.guannengcc.top

Java: a && b || !c
来源：http://flo.xylfe.cn

Go:   a && b || !c
来源：http://tet.gotoacloud.top

Ruby: a && b || !c
来源：http://ltw.0kj1m.cn

C#:   a && b || !c
来源：http://fyb.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://rii.shanyushiyangtech.top

Py:   if not data: return
来源：http://kwf.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://tkz.tanke756.top

JS:   if (!data) return;
来源：http://zoa.yj202588.top

TS:   if (!data) return;
来源：http://zrq.havefunace.top

Java: if (data == null) return;
来源：http://daw.guannengcc.top

Go:   if data == nil { return }
来源：http://swc.vqdsnc.cn

Ruby: return if data.nil?
来源：http://hql.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://oxo.wangdashe.top

================================================================================
来源：http://luq.mhx1999.top

C. 函数与作用域
来源：http://pji.dashuyun.cn

================================================================================
来源：http://owt.jyoumei.cn

[C01] 定义函数
来源：http://rrk.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://epw.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vvc.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://rhn.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pko.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://qpt.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://ltu.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://ktl.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qvu.c1oappe.top

[C02] 默认参数
来源：http://bet.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://jqz.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://drn.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wpp.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://dly.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dcg.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pkn.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://uzj.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://pvj.cdnleiting.top

[C03] 可变参数
来源：http://lle.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://ngx.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xai.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://coh.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jld.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gvp.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zbf.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://hko.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yhe.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://ykr.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ppb.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oxk.tian-w.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ytf.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qrb.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://ddc.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://tid.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://xjv.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://nwe.daria6918.cn

[C05] 返回多个值
来源：http://nyu.jlsjyb.cn

Py:   return a, b
来源：http://nno.xziqi.cn

PHP:  return [$a, $b];
来源：http://cjo.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://xfz.yj202588.top

TS:   return { a, b };
来源：http://zqr.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://unt.zdbjq.cn

Go:   return a, b
来源：http://trb.ctjpmb.com

Ruby: return a, b
来源：http://nvp.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://mbd.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://css.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://gmv.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xdm.yj202588.top

JS:   const square = x => x * x;
来源：http://zfb.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://gug.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wiy.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://bcq.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://lmj.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://xgb.yj20258.top

[C07] 把函数作为参数传入
来源：http://vrj.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://igc.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://jje.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mpt.zhongyouzk.top

TS:   arr.map(String)
来源：http://opq.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xjy.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yne.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://soh.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dzg.hnxiangtu.top

[C08] 闭包
来源：http://fiu.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qpq.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qtj.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tvq.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oam.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://evi.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nzn.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qyh.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cvj.ydjk.org.cn

[C09] 递归
来源：http://kui.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ntv.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blm.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bof.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yzk.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fxb.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iyh.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qzz.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ipb.zhongyouzk.top

[C10] 变量作用域
来源：http://lak.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lga.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aqj.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ael.hnxiangtu.top

TS:   同 JS
来源：http://yxm.sufxvd.cn

Java: 方法内为块级作用域
来源：http://xmv.bjfxy.top

Go:   花括号块级作用域
来源：http://rfj.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dzg.sufxvd.cn

C#:   块级作用域
来源：http://oqb.birdmap.top

[C11] 模块导入与导出
来源：http://pnl.316326.xyz

Py:   from module import func
来源：http://obh.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dnc.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://hzh.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hxy.zhiwuduotai.top

Java: import java.util.List;
来源：http://svi.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://orp.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://kpr.ivvv.top

C#:   using System.Text;
来源：http://egs.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://dux.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://yzl.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://foc.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://qgu.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://aeq.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ikg.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://sxf.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://akh.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eul.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://frc.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qrr.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfr.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dcz.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://otc.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://jlf.bjfxy.top

Go:   func add(a, b int) int
来源：http://ksl.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ghh.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pzq.cucudq.cn

[C14] 泛型函数
来源：http://vbe.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pnx.guannengcc.top

PHP:  // 无泛型
来源：http://ktn.zycfv.cn

JS:   // 无泛型
来源：http://jis.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kiw.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rqk.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://myk.cqqwz.cn

Ruby: # 无泛型
来源：http://gri.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://piw.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://jiw.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jry.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://yyw.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eur.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fec.nwbrower.top

Java: // 无解构
来源：http://tnq.jqgfzy.top

Go:   // 无解构
来源：http://ckz.jyoumei.cn

Ruby: a, b = pair
来源：http://zzb.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://htv.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://rfp.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tuh.dashuyun.cn

PHP:  // 无重载
来源：http://qav.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bkn.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://nhx.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qbf.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://jas.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://rtz.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jwt.snrcjt.cn

================================================================================
来源：http://slt.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://veh.ywan-chungtsiang.top

================================================================================
来源：http://vpz.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://ugr.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://nvy.zhixingplan.top


<!-- 参考信息 -->