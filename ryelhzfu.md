代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vtf.jianghu66.top

[B02] 多分支 else if / elif
来源：http://ong.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aqu.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tdn.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgu.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddt.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ycr.tian-w.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ieh.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://msv.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://snz.yvedp.cn

[B03] switch / match / case
来源：http://xms.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lhr.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gtw.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bdv.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dwi.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://idu.snrcjt.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fgn.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dro.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nrf.hnqzz.top

[B04] for 计数循环
来源：http://paj.yonumen.top

Py:   for i in range(10): print(i)
来源：http://idf.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bfp.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jcz.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aun.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oyn.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uee.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://khm.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hpd.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://xke.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://xeq.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kbn.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://axy.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wpl.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bky.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lee.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://ioq.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cjh.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://jcr.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nkq.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zdi.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cuh.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tss.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uzb.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tir.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://los.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tci.gotoacloud.top

[B07] while 循环
来源：http://kwi.zycfv.cn

Py:   while i < 10: i += 1
来源：http://rij.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://btf.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://pje.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://gdj.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://qzj.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ved.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://fkq.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://ihi.pycfn.com

[B08] do-while（至少执行一次）
来源：http://pma.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://wgg.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fuy.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://stw.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://jpv.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://ysh.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://axb.dianchejie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vxt.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://vcl.jiagoushi.top

[B09] break 与 continue
来源：http://byh.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ntu.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lnu.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvy.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsk.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkh.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wda.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zwn.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gti.sufxvd.cn

[B10] 遍历同时拿索引
来源：http://cfi.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fip.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uvn.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ipz.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wir.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xhv.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xtz.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qvv.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lzf.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://eks.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://lvr.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://ujt.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iyv.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://krx.zhongyouzk.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qew.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jif.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://eea.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://brk.epnwcf.com

[B12] 跳出多层循环
来源：http://fsz.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://neq.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ljr.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zov.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ilr.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://slr.cashguo.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tce.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rqw.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lfi.xuanzx.com

[B13] 判断是否为数字
来源：http://wng.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://ial.yueranfly.top

PHP:  is_numeric($x)
来源：http://ppk.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elh.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ays.birdmap.top

Java: x instanceof Number
来源：http://jea.yuxming.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kom.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://fpz.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://wii.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://xqf.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uxf.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dpx.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://jkg.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://bsi.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://qkn.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dlv.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://qex.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yjp.tarul.cn

[B15] 布尔运算与取反
来源：http://ttk.sufxvd.cn

Py:   a and b or not c
来源：http://sms.fehbvm.com

PHP:  $a && $b || !$c
来源：http://elo.yangfankeji.com

JS:   a && b || !c
来源：http://uyt.guannengcc.top

TS:   a && b || !c
来源：http://agf.xuetiantiany.cn

Java: a && b || !c
来源：http://cof.52xcode.cn

Go:   a && b || !c
来源：http://xyb.kuanghao11.cn

Ruby: a && b || !c
来源：http://rcx.svipenyu.cn

C#:   a && b || !c
来源：http://cfd.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tef.xuetiantiany.cn

Py:   if not data: return
来源：http://yeq.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://orp.daxiang520.top

JS:   if (!data) return;
来源：http://lcw.vqdsnc.cn

TS:   if (!data) return;
来源：http://enm.shangyingyoupin.top

Java: if (data == null) return;
来源：http://ojj.daria6918.cn

Go:   if data == nil { return }
来源：http://tcu.jinqigufen.top

Ruby: return if data.nil?
来源：http://oie.meibo888.top

C#:   if (data == null) return;
来源：http://qqy.dianchejie.cn

================================================================================
来源：http://sbj.fehbvm.com

C. 函数与作用域
来源：http://gfb.hcnkem.com

================================================================================
来源：http://yqo.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://qjz.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://vuy.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://txl.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://rbo.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://poq.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zmw.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://ncc.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://fqe.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xor.hesvh.cn

[C02] 默认参数
来源：http://smb.ivvv.top

Py:   def greet(name="World"): return name
来源：http://uqq.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rfu.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://vbf.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mqp.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gyg.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dty.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://iyz.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://xum.yvedp.cn

[C03] 可变参数
来源：http://kvz.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://rgt.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ogb.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://msp.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eoz.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rpc.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pon.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://smz.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nft.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://xgk.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pbr.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nei.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vit.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://txp.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://vvm.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://nea.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://agx.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://yne.hesvh.cn

[C05] 返回多个值
来源：http://kvs.meibo888.top

Py:   return a, b
来源：http://wcj.gogol.net.cn

PHP:  return [$a, $b];
来源：http://fet.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rdx.hywenlv.cn

TS:   return { a, b };
来源：http://has.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pnm.hcnkem.com

Go:   return a, b
来源：http://lea.cashguo.top

Ruby: return a, b
来源：http://xuq.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://rxu.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://wgf.wangdashe.top

Py:   square = lambda x: x * x
来源：http://hwv.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vvr.316326.xyz

JS:   const square = x => x * x;
来源：http://ohf.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://fdh.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ahs.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mid.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://gos.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://fbu.iojbl.cn

[C07] 把函数作为参数传入
来源：http://huk.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wad.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://sjp.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://taf.nwbrower.top

TS:   arr.map(String)
来源：http://thd.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xin.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rzo.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://pgl.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bou.shangyingyoupin.top

[C08] 闭包
来源：http://rkt.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ouf.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qcm.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://krr.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gza.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aoy.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mex.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ubd.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bow.yueranfly.top

[C09] 递归
来源：http://jkq.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wzg.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://njz.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ojb.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://abe.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oya.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ciz.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lhx.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mhn.feifeiyinyue.top

[C10] 变量作用域
来源：http://ckw.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hvl.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kcd.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iyi.xziqi.cn

TS:   同 JS
来源：http://iry.smart0.xyz

Java: 方法内为块级作用域
来源：http://dot.yj20258.top

Go:   花括号块级作用域
来源：http://gge.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mdq.haohaochexian.top

C#:   块级作用域
来源：http://fsl.ybcxt.top

[C11] 模块导入与导出
来源：http://kkc.gogol.net.cn

Py:   from module import func
来源：http://mte.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jur.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://txx.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bly.xuetiantiany.cn

Java: import java.util.List;
来源：http://imi.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ofc.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://yqm.xuanzx.com

C#:   using System.Text;
来源：http://mpi.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://eaf.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://fxh.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://vyd.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://ajj.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://jgu.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fec.meibo888.top

Go:   func() { fmt.Println("run") }()
来源：http://rwx.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://ptw.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://foq.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://fni.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://not.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bdt.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bar.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fyc.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oxj.mhx1999.top

Go:   func add(a, b int) int
来源：http://hzb.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://erp.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://fwx.guannengcc.top

[C14] 泛型函数
来源：http://zkw.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rkt.jianghu66.top

PHP:  // 无泛型
来源：http://pxu.daria6918.cn

JS:   // 无泛型
来源：http://zhh.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ytv.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sek.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zdy.yueranfly.top

Ruby: # 无泛型
来源：http://blc.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jnd.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://eyn.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kau.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://rit.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dtl.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jdr.kuanghao11.cn

Java: // 无解构
来源：http://tfk.pengpengdd.cyou

Go:   // 无解构
来源：http://zvb.meibo888.top

Ruby: a, b = pair
来源：http://qsc.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://pmz.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://add.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://clk.52xcode.cn

PHP:  // 无重载
来源：http://bzf.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ghu.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://cau.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sku.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://cnq.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://uoh.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zba.jqgfzy.top

================================================================================
来源：http://uss.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://ctp.hywenlv.cn

================================================================================
来源：http://siu.52xcode.cn

[D01] 创建数组 / 列表
来源：http://mdx.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cgo.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wvc.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xji.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wof.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jiy.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ilu.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://mxg.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jvh.yj20258.top

[D02] 追加元素到末尾
来源：http://ffk.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zme.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://txx.yuanzhike.top

JS:   arr.push(4);
来源：http://ave.meibo888.top

TS:   arr.push(4);
来源：http://rfs.pycfn.com


<!-- 参考信息 -->