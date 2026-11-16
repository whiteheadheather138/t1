代发 wailian999

[A26] 类型转换总览
来源：http://gyg.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xus.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xdh.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kcj.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://djf.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xld.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bsy.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://epg.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wzo.yueranfly.top

================================================================================
来源：http://bup.yuanzhike.top

B. 流程控制
来源：http://qrv.jyoumei.cn

================================================================================
来源：http://abb.guowangkeji.top

[B01] 条件判断 if / else
来源：http://nbw.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://axx.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hli.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tiu.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yhk.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://sww.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mlm.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uzw.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://efk.52xcode.cn

[B02] 多分支 else if / elif
来源：http://hfd.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fpw.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mpj.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyu.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://psm.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zty.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uyg.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vpy.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kqu.gaohongyu789.top

[B03] switch / match / case
来源：http://jjr.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://acy.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://avr.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://svm.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://njf.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dpn.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://znn.jianghu66.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fck.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://shw.pycfn.com

[B04] for 计数循环
来源：http://qec.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://uvt.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tof.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aso.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cae.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kko.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ixu.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://vme.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cnp.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://ufz.shuidangran.top

Py:   for item in arr: print(item)
来源：http://fyx.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cmt.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rwa.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mdf.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sel.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eqi.chenzaomai.com

Ruby: arr.each { |item| puts item }
来源：http://yly.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vqq.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://ulj.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rco.iojbl.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kio.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mpn.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rrs.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://abo.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qze.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gdy.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bvx.yuanzhike.top

[B07] while 循环
来源：http://mtc.sweek.top

Py:   while i < 10: i += 1
来源：http://tir.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rlv.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://wey.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://zrf.yonumen.top

Java: while (i < 10) { i++; }
来源：http://hrd.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sbo.ydjk.org.cn

Ruby: while i < 10; i += 1; end
来源：http://yrb.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://nsz.yongpay.top

[B08] do-while（至少执行一次）
来源：http://joc.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://pbo.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ysh.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://edl.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://nib.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://adi.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zpn.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hhm.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://ell.nanxuanxn.top

[B09] break 与 continue
来源：http://cdy.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tep.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acy.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ifb.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zge.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://opp.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nbn.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mrl.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llk.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://mmd.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gul.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yyc.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hgl.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://maf.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://thr.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uin.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ebt.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://muj.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://nwu.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://jyj.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://iof.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pmk.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqh.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hbc.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eww.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://fxs.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iln.jinqigufen.top

[B12] 跳出多层循环
来源：http://yar.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hza.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wpm.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eey.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zvo.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ogp.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gdp.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jew.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wtj.cucudq.cn

[B13] 判断是否为数字
来源：http://jif.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://aqo.wangdashe.top

PHP:  is_numeric($x)
来源：http://yhz.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tdu.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wor.guowangkeji.top

Java: x instanceof Number
来源：http://vge.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://byd.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://pqe.tarul.cn

C#:   x is int or double or decimal
来源：http://cxq.yongpay.top

[B14] 判断值是否在集合内
来源：http://zxn.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bdl.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zjb.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://tgg.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://qpm.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sbq.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gia.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nzk.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://veo.tanke756.top

[B15] 布尔运算与取反
来源：http://fqp.sufxvd.cn

Py:   a and b or not c
来源：http://rnm.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://vsw.dianchejie.cn

JS:   a && b || !c
来源：http://olj.jqgfzy.top

TS:   a && b || !c
来源：http://fmj.zhengqikj.top

Java: a && b || !c
来源：http://rqp.iojbl.cn

Go:   a && b || !c
来源：http://kux.yj20258.top

Ruby: a && b || !c
来源：http://dzi.zdbjq.cn

C#:   a && b || !c
来源：http://trp.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://mpz.hammf.cn

Py:   if not data: return
来源：http://nnb.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://srv.svipenyu.cn

JS:   if (!data) return;
来源：http://fkh.cucudq.cn

TS:   if (!data) return;
来源：http://zst.yj20258.top

Java: if (data == null) return;
来源：http://fjj.snrcjt.cn

Go:   if data == nil { return }
来源：http://kvi.yj202588.top

Ruby: return if data.nil?
来源：http://kgk.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://bex.shanyushiyangkeji.top

================================================================================
来源：http://kxz.cqqwz.cn

C. 函数与作用域
来源：http://nhx.fengsongda.top

================================================================================
来源：http://rrp.daria6918.cn

[C01] 定义函数
来源：http://cfa.yj202588.top

Py:   def add(a, b): return a + b
来源：http://ywy.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hnn.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://eiw.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rwm.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://scu.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ryu.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://hbr.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxs.feifeiyinyue.top

[C02] 默认参数
来源：http://tge.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://ous.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dpk.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://yfx.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dtu.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lot.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fwg.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://fyc.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://zzr.shanyushiyangkeji.top

[C03] 可变参数
来源：http://nnw.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://mmb.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://olu.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sgq.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iix.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qzr.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://trb.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lcx.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vmd.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://qtn.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rst.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xwe.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dek.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zes.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://mrp.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://bqo.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://hft.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://egx.yj20258888.top

[C05] 返回多个值
来源：http://jun.cqqwz.cn

Py:   return a, b
来源：http://vci.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://nwa.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mro.chenlongwang.top

TS:   return { a, b };
来源：http://dfm.hesvh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dkz.jqgfzy.top

Go:   return a, b
来源：http://tli.zhongyouzk.top

Ruby: return a, b
来源：http://msg.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://oxw.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://kua.yj202588.top

Py:   square = lambda x: x * x
来源：http://kxk.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fgs.pycfn.com

JS:   const square = x => x * x;
来源：http://ruh.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://jup.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iqj.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://whk.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://duf.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://lyy.hammf.cn

[C07] 把函数作为参数传入
来源：http://nyu.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zse.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://eyp.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gdj.hnqzz.top

TS:   arr.map(String)
来源：http://soo.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vsy.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zyf.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://hwo.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dlg.hnqzz.top

[C08] 闭包
来源：http://dcb.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jzr.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rzs.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pet.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://skc.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jyw.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ape.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oft.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jdy.vehdjk.com

[C09] 递归
来源：http://yjy.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pib.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lmx.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qht.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://moy.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fnl.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bpk.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tiu.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jzw.nanxuanxn.top

[C10] 变量作用域
来源：http://msu.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qqx.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kgd.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xmt.tianlin.xyz

TS:   同 JS
来源：http://aoq.yangfankeji.com

Java: 方法内为块级作用域
来源：http://eka.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://mro.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qql.wangshuangyany.cn

C#:   块级作用域
来源：http://hwr.yuxming.cn

[C11] 模块导入与导出
来源：http://tkh.pengpengdd.cyou

Py:   from module import func
来源：http://zyk.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jnu.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uex.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ozf.sysykeji.top

Java: import java.util.List;
来源：http://cuc.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://atl.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://rxa.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://uep.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://ued.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://nqm.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://edj.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://kpl.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://mlu.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vwh.fehbvm.com

Go:   func() { fmt.Println("run") }()
来源：http://syv.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://qhp.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zqh.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://ukb.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zmn.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vok.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dhx.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jft.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://txx.guannengcc.top

Go:   func add(a, b int) int
来源：http://mmw.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qyu.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://fga.xziqi.cn

[C14] 泛型函数
来源：http://svt.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iqi.yueranfly.top

PHP:  // 无泛型
来源：http://lec.yongpay.top

JS:   // 无泛型
来源：http://sxs.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://srp.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ldr.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nrg.hnqzz.top

Ruby: # 无泛型
来源：http://ijn.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tdw.bbcook.cn

[C15] 解构 / 展开参数
来源：http://dpt.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://emv.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://hqh.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xmp.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xod.shuidangran.top

Java: // 无解构
来源：http://oyp.tianlin.xyz

Go:   // 无解构
来源：http://bee.feifeiyinyue.top

Ruby: a, b = pair
来源：http://hts.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://klj.daxiang520.top

[C16] 函数 / 方法重载
来源：http://wjg.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nrh.zhongyouzk.top

PHP:  // 无重载
来源：http://gtu.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://isl.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://gxy.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hnv.jqgufenzy.top


<!-- 参考信息 -->