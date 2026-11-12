代发 wailian999

[B01] 条件判断 if / else
来源：http://oof.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kua.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jjd.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lrb.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nbo.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://pkj.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sex.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iql.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pfw.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://prp.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wmj.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://joc.ppjwa.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rgb.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfu.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdr.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jwx.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wcw.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zcl.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://lcp.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zet.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xiv.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bzw.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jew.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lqs.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zdw.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mds.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rdn.yfazqb.com

[B04] for 计数循环
来源：http://fsa.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://ryz.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qja.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oox.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qph.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xtu.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ida.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://uzg.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://obb.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://tof.fzhhl.top

Py:   for item in arr: print(item)
来源：http://ihq.ivvv.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://muo.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yoc.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zgb.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qwv.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gpb.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://bte.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fxw.ivvv.top

[B06] 遍历字典 / 对象
来源：http://wpt.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kdf.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lim.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nfk.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://olt.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mel.zdqjudy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dqy.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mvo.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hte.zhijiandao.cn

[B07] while 循环
来源：http://eav.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://mtf.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://laq.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://far.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://erl.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://rom.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://otz.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://tkr.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://zfg.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://gyk.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://tqc.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pbx.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://xaz.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://bzz.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://raq.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://cgx.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://xes.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://xzm.zdbjq.cn

[B09] break 与 continue
来源：http://cgg.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lrj.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cgn.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fli.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umv.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcy.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qkf.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oxb.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qou.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://poh.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wbp.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://omq.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zac.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wve.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://csb.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dog.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jxo.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ois.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://blh.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://sgj.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://jjn.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pyq.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sue.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://njh.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://plh.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://yds.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ngo.mhx1999.top

[B12] 跳出多层循环
来源：http://mip.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tcl.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://joo.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ywt.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qkq.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kex.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lcx.hnqzz.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mrl.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baz.daxiang520.top

[B13] 判断是否为数字
来源：http://dat.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://pri.birdmap.top

PHP:  is_numeric($x)
来源：http://aqe.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xlm.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bkd.yanxiufei.cn

Java: x instanceof Number
来源：http://sli.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mnt.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://sbo.gogol.net.cn

C#:   x is int or double or decimal
来源：http://see.redwolf501.top

[B14] 判断值是否在集合内
来源：http://dpy.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tyb.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uhy.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://uzb.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://abi.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://srb.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wqd.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://whr.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fsj.zdbjq.cn

[B15] 布尔运算与取反
来源：http://yxc.chenlongwang.top

Py:   a and b or not c
来源：http://erv.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://jco.bjfxy.top

JS:   a && b || !c
来源：http://std.cdnleiting.top

TS:   a && b || !c
来源：http://cou.yj20258.top

Java: a && b || !c
来源：http://vhf.sysykeji.top

Go:   a && b || !c
来源：http://pxm.nwbrower.top

Ruby: a && b || !c
来源：http://fjk.cqqwz.cn

C#:   a && b || !c
来源：http://vkh.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lcn.zhixingplan.top

Py:   if not data: return
来源：http://czi.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://qlx.316326.xyz

JS:   if (!data) return;
来源：http://gye.yueranfly.top

TS:   if (!data) return;
来源：http://rpl.zhoulong.xyz

Java: if (data == null) return;
来源：http://vvm.birdmap.top

Go:   if data == nil { return }
来源：http://kgn.chenzaomai.com

Ruby: return if data.nil?
来源：http://iro.mhx1999.top

C#:   if (data == null) return;
来源：http://fdv.chenjidiqi.icu

================================================================================
来源：http://ikg.tanke756.top

C. 函数与作用域
来源：http://ezl.cheryme.top

================================================================================
来源：http://csh.fehbvm.com

[C01] 定义函数
来源：http://gek.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://njj.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oaw.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ycn.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://csm.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sya.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gko.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://qef.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dgt.dashuyun.cn

[C02] 默认参数
来源：http://tjk.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://ofx.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ond.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://bnh.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qkq.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ino.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fzz.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://upg.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://abg.yanxiufei.cn

[C03] 可变参数
来源：http://oyl.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://jqk.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xtw.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://per.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwd.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lkw.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://omg.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://nla.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zdu.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://scl.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zha.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ips.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pwe.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mcw.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://pez.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://ybi.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://uwi.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://kzn.jinghuilouyu.cn

[C05] 返回多个值
来源：http://dxf.sufxvd.cn

Py:   return a, b
来源：http://gou.ydzc1.top

PHP:  return [$a, $b];
来源：http://szu.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hbq.sysykeji.top

TS:   return { a, b };
来源：http://uch.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uvl.shanyushiyangkeji.top

Go:   return a, b
来源：http://qjs.nanxuanxn.top

Ruby: return a, b
来源：http://rgh.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://eqr.tanke756.top

[C06] 匿名函数 / lambda
来源：http://hem.jianghu66.top

Py:   square = lambda x: x * x
来源：http://nsn.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bik.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://kas.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://jss.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yzq.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://foh.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://fni.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://btk.nwbrower.top

[C07] 把函数作为参数传入
来源：http://dor.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://phg.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://tnf.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fdn.fengsongda.top

TS:   arr.map(String)
来源：http://umu.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fmw.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hjw.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://xgb.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lyd.52xcode.cn

[C08] 闭包
来源：http://egz.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jns.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mur.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kdx.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vhe.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ysc.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bjh.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tfa.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://awr.daxiang520.top

[C09] 递归
来源：http://wqy.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://emf.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tug.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tlt.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cst.zycfv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gdk.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gnl.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cji.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qon.vqdsnc.cn

[C10] 变量作用域
来源：http://wdq.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zrz.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://szs.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rcj.havefunace.top

TS:   同 JS
来源：http://bhm.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://vgm.chenzaomai.com

Go:   花括号块级作用域
来源：http://gox.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zzr.sjlbkw.cn

C#:   块级作用域
来源：http://mlx.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://oum.birdmap.top

Py:   from module import func
来源：http://hnq.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bmb.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://now.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://huu.yuxming.cn

Java: import java.util.List;
来源：http://kmw.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qmx.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://xjk.jinqigufen.top

C#:   using System.Text;
来源：http://aff.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://eqf.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://lnq.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://xcj.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://pgq.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://gmg.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kfd.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://nhs.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://rmv.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rvt.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://oyj.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qgf.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lbl.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xmi.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fst.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://zgl.zhixingplan.top

Go:   func add(a, b int) int
来源：http://yyt.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rof.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://bzv.zhijiandao.cn

[C14] 泛型函数
来源：http://qyt.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fbf.yuxming.cn

PHP:  // 无泛型
来源：http://dvc.yj20258888.top

JS:   // 无泛型
来源：http://rhp.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qov.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://phb.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dbo.ehwqpu.com

Ruby: # 无泛型
来源：http://exb.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lyu.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://ing.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pfp.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://xor.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sfq.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://obi.tian-w.cn

Java: // 无解构
来源：http://wpv.ydjk.org.cn

Go:   // 无解构
来源：http://mpn.guannengcc.top

Ruby: a, b = pair
来源：http://spv.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://rbz.gzhubu.top

[C16] 函数 / 方法重载
来源：http://fwc.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cpu.hfpthk.cn

PHP:  // 无重载
来源：http://luh.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kmk.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://ntz.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cvr.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://zut.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://wpe.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://gtj.jlsjyb.cn

================================================================================
来源：http://rsy.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://ane.andypj.xyz

================================================================================
来源：http://trr.hnqzz.top

[D01] 创建数组 / 列表
来源：http://iur.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uab.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gru.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wsi.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hlu.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wvc.svipenyu.cn


<!-- 参考信息 -->