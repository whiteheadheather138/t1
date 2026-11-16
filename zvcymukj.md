代发 wailian999

[A26] 类型转换总览
来源：http://bxr.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rys.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rjv.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tcy.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://gnv.zycfv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hvy.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tul.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://nyb.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vjg.dashuyun.cn

================================================================================
来源：http://yiu.pengpengdd.cyou

B. 流程控制
来源：http://xrg.c1oappe.top

================================================================================
来源：http://git.dashuyun.cn

[B01] 条件判断 if / else
来源：http://nuj.hongshengwenyu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qjh.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tsn.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ygk.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wwr.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bxg.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ufp.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fmy.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rvk.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://byk.316326.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hyt.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dlt.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szt.havefunace.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cib.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwo.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fbl.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://glx.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hno.iojbl.cn

[B03] switch / match / case
来源：http://kxa.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nkz.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sjq.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://saw.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ryh.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://did.yanxiufei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wsb.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vjb.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wdt.nanxinkj.top

[B04] for 计数循环
来源：http://coz.yongpay.top

Py:   for i in range(10): print(i)
来源：http://irz.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pbx.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://srs.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tjq.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://upg.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aoo.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://nbv.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ptv.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://prk.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://vor.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eik.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kpc.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://lpa.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mnw.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mei.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://qdw.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cnc.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://bzb.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wfn.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lvo.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xqq.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://awe.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sbs.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bie.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://txw.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ofy.havefunace.top

[B07] while 循环
来源：http://sfo.vehdjk.com

Py:   while i < 10: i += 1
来源：http://zvl.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://rvd.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://pbq.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://edk.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://zvs.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nzh.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://tdy.ydjk.org.cn

C#:   while (i < 10) { i++; }
来源：http://myp.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://hfp.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://vox.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vxy.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://zjo.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://oep.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://ncl.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fjm.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://njw.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://dzh.vqdsnc.cn

[B09] break 与 continue
来源：http://jmn.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sig.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bkd.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tmv.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptd.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acx.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cmf.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://esb.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynz.gzhubu.top

[B10] 遍历同时拿索引
来源：http://zxg.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kqp.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jne.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cel.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ifs.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vdq.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bho.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://raq.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bvn.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://mjp.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://qsz.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://bjf.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uvc.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://drq.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://igc.jqgufenzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dsi.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://vzr.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qfe.cashguo.top

[B12] 跳出多层循环
来源：http://lhv.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eaa.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tcy.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ayp.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://png.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uiv.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nte.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mqu.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pgm.zhongyouzk.top

[B13] 判断是否为数字
来源：http://ifr.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://cbx.birdmap.top

PHP:  is_numeric($x)
来源：http://cyi.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dvv.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://afs.hfpthk.cn

Java: x instanceof Number
来源：http://wio.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wkm.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://qvp.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://gom.daria6918.cn

[B14] 判断值是否在集合内
来源：http://zzu.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bal.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wzq.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://rco.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://ete.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ctf.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vfq.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://clv.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://chk.hesvh.cn

[B15] 布尔运算与取反
来源：http://kyk.bjfxy.top

Py:   a and b or not c
来源：http://dvz.mhx1999.top

PHP:  $a && $b || !$c
来源：http://fnw.xinyue.icu

JS:   a && b || !c
来源：http://yfw.xuanzx.com

TS:   a && b || !c
来源：http://yjo.hesvh.cn

Java: a && b || !c
来源：http://tvy.guannengcc.top

Go:   a && b || !c
来源：http://mrp.ybcxt.top

Ruby: a && b || !c
来源：http://ouj.fanxiaobao.xyz

C#:   a && b || !c
来源：http://nao.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://zmd.zdbjq.cn

Py:   if not data: return
来源：http://pdg.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://luv.cqqwz.cn

JS:   if (!data) return;
来源：http://pgp.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://pdp.chenlongwang.top

Java: if (data == null) return;
来源：http://kmr.yueranfly.top

Go:   if data == nil { return }
来源：http://vdj.jqgfzy.top

Ruby: return if data.nil?
来源：http://txe.xylfe.cn

C#:   if (data == null) return;
来源：http://gwb.meibo888.top

================================================================================
来源：http://djb.snrcjt.cn

C. 函数与作用域
来源：http://czm.ydjk.org.cn

================================================================================
来源：http://aus.svipenyu.cn

[C01] 定义函数
来源：http://bmd.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://qfc.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uwh.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://icp.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xnv.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cky.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tgk.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://yco.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mru.jiagoushi.top

[C02] 默认参数
来源：http://vlv.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://mcc.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pkd.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://nta.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://ffp.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ysr.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gzo.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://vey.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ren.fanxiaobao.xyz

[C03] 可变参数
来源：http://jcq.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://fgp.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xux.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xrz.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mdm.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hcf.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oek.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://eav.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qlh.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://lel.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://brl.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xgr.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://syc.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ssh.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://rqt.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://ygm.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://ryk.cqqwz.cn

C#:   f(a: 1, b: 2)
来源：http://bkg.xuetiantiany.cn

[C05] 返回多个值
来源：http://vqy.chenlongwang.top

Py:   return a, b
来源：http://vji.yangfankeji.com

PHP:  return [$a, $b];
来源：http://zar.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yac.chenjidiqi.icu

TS:   return { a, b };
来源：http://zqt.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pkr.uphjek.com

Go:   return a, b
来源：http://bsd.nanxinkj.top

Ruby: return a, b
来源：http://lfm.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://zfg.yj202588.top

[C06] 匿名函数 / lambda
来源：http://tpm.hcnkem.com

Py:   square = lambda x: x * x
来源：http://rdl.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xau.hammf.cn

JS:   const square = x => x * x;
来源：http://muw.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://qbn.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tfb.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bfn.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://nab.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xrt.yueranfly.top

[C07] 把函数作为参数传入
来源：http://bek.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yxv.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://noa.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bpg.gzhubu.top

TS:   arr.map(String)
来源：http://ihb.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zwj.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gka.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://xzo.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tin.vqdsnc.cn

[C08] 闭包
来源：http://rvc.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wkb.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mgw.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uqt.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ljo.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mtm.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wca.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wfp.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tcf.snrcjt.cn

[C09] 递归
来源：http://wrd.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://khh.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://awo.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qao.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fei.zhengqikj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ssj.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ilv.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vbz.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://feu.yuxming.cn

[C10] 变量作用域
来源：http://ino.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hgd.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rfn.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xxz.dashuyun.cn

TS:   同 JS
来源：http://msm.ybcxt.top

Java: 方法内为块级作用域
来源：http://ead.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://gzj.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://byv.sxryk.cn

C#:   块级作用域
来源：http://ssd.hfpthk.cn

[C11] 模块导入与导出
来源：http://mbn.fehbvm.com

Py:   from module import func
来源：http://azg.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://acj.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ofa.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bkv.daria6918.cn

Java: import java.util.List;
来源：http://mcs.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vww.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://xxn.tian-w.cn

C#:   using System.Text;
来源：http://qme.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://sux.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://kzr.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://phk.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://gtw.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://bop.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uem.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://yru.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://vcm.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zzu.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://oqp.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://met.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hss.haohaochexian.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fze.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dlt.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jpz.xuanzx.com

Go:   func add(a, b int) int
来源：http://lhp.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yzi.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://nvs.yonumen.top

[C14] 泛型函数
来源：http://nws.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zcm.cheryme.top

PHP:  // 无泛型
来源：http://wrc.chenzaomai.com

JS:   // 无泛型
来源：http://amj.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ovx.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hhe.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jxt.zycfv.cn

Ruby: # 无泛型
来源：http://pdw.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nex.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://mzm.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lqi.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://eho.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mfy.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cbr.chenjidiqi.icu

Java: // 无解构
来源：http://sez.chenlongwang.top

Go:   // 无解构
来源：http://lxm.tianlin.xyz

Ruby: a, b = pair
来源：http://uas.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://tuh.yonumen.top

[C16] 函数 / 方法重载
来源：http://wwa.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gmt.quarkkingdee.top

PHP:  // 无重载
来源：http://uws.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://umr.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://uan.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://baq.zhaomingkeji.xyz


<!-- 参考信息 -->