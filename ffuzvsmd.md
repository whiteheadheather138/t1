代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rio.ydzc1.top

[B02] 多分支 else if / elif
来源：http://piu.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qhp.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://raf.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zja.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aoz.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fao.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zhd.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zpx.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oej.shuidangran.top

[B03] switch / match / case
来源：http://gyk.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vor.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mzw.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ihl.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aan.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qrx.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xee.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tqa.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zrd.zhixingplan.top

[B04] for 计数循环
来源：http://wud.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://xfm.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jcs.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yvi.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gyo.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://elw.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bsz.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://cqd.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sib.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://wgn.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://nsk.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bum.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dix.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xwq.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://stx.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pgy.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://kqd.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xlt.yj202588.top

[B06] 遍历字典 / 对象
来源：http://hjl.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pxn.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xfw.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vkz.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ntr.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sse.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oso.wangdashe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xym.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vqg.yj20258.top

[B07] while 循环
来源：http://nzq.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://ldw.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ycd.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://gef.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://wvc.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://jev.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zei.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://qvj.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://azb.uphjek.com

[B08] do-while（至少执行一次）
来源：http://tfw.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://bar.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://ilf.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://dnx.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://pwf.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://mdn.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oxz.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://cio.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://ohe.meibo888.top

[B09] break 与 continue
来源：http://ydz.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xde.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kmv.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://muk.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqr.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fsr.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mwg.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vrd.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://deu.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://tqi.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ovu.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ydt.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zks.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aue.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zne.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cbu.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tfr.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://khp.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://owy.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://dsh.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://xml.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lzh.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bbo.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xkb.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xrf.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://ttd.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xla.yj20258888.top

[B12] 跳出多层循环
来源：http://ntx.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hql.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://odb.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pcw.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://myz.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yre.uphjek.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sxc.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://izk.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mjn.bjfxy.top

[B13] 判断是否为数字
来源：http://zjr.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://qbi.hcnkem.com

PHP:  is_numeric($x)
来源：http://bgd.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nng.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://omt.yongpay.top

Java: x instanceof Number
来源：http://cko.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cky.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://zej.zycfv.cn

C#:   x is int or double or decimal
来源：http://yqf.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://jnl.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pix.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://opj.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://jye.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://ztr.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ots.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jfn.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://jom.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wbs.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://stl.svipenyu.cn

Py:   a and b or not c
来源：http://bbu.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://lcf.pengpengdd.cyou

JS:   a && b || !c
来源：http://jgr.gotoacloud.top

TS:   a && b || !c
来源：http://zoy.xylfe.cn

Java: a && b || !c
来源：http://bzf.ivvv.top

Go:   a && b || !c
来源：http://iil.zhoulong.xyz

Ruby: a && b || !c
来源：http://qrp.daxiang520.top

C#:   a && b || !c
来源：http://tnk.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rcs.yueranfly.top

Py:   if not data: return
来源：http://tye.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://jak.zdqjudy.top

JS:   if (!data) return;
来源：http://nzz.ivvv.top

TS:   if (!data) return;
来源：http://sqn.yj20258.top

Java: if (data == null) return;
来源：http://bfd.yuxming.cn

Go:   if data == nil { return }
来源：http://fgu.yonumen.top

Ruby: return if data.nil?
来源：http://gxg.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://dzj.xuetiantiany.cn

================================================================================
来源：http://vvd.jianghu66.top

C. 函数与作用域
来源：http://hfp.ctjpmb.com

================================================================================
来源：http://fhu.yj202588.top

[C01] 定义函数
来源：http://hgj.shanyushiyangtech.top

Py:   def add(a, b): return a + b
来源：http://vqd.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cdp.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://klb.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://owr.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kyg.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://syh.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://tgy.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aym.fehbvm.com

[C02] 默认参数
来源：http://pqo.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://dvz.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qmr.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://jve.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nke.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kaf.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kav.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://dgj.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://kov.chenzaomai.com

[C03] 可变参数
来源：http://zef.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://hvc.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fzm.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pea.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eij.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dtl.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zwp.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://oww.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nmb.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://fvq.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ilg.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zwz.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tyn.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://neq.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://gny.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://owr.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://jpp.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://iga.bjfxy.top

[C05] 返回多个值
来源：http://vsf.yongpay.top

Py:   return a, b
来源：http://qut.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://urh.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yno.yangfankeji.com

TS:   return { a, b };
来源：http://gne.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://laq.aibaodan.cn

Go:   return a, b
来源：http://zim.fanxiaobao.xyz

Ruby: return a, b
来源：http://pyc.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://bkq.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://cco.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://nwe.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bod.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://vhd.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://sny.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pxj.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xyp.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://gkp.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://cwu.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://fmx.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rup.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jvu.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://svx.hnqzz.top

TS:   arr.map(String)
来源：http://cll.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xbh.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gzh.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://qeo.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uwo.zhengqikj.top

[C08] 闭包
来源：http://tqu.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eru.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kvr.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://reb.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://brg.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hen.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xxt.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://val.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fma.ybcxt.top

[C09] 递归
来源：http://jyx.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://efo.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tcl.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://grp.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://acg.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uuw.cheryme.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xmq.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://osq.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://czd.xuetiantiany.cn

[C10] 变量作用域
来源：http://vgx.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ehm.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cti.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://otp.hesvh.cn

TS:   同 JS
来源：http://imo.jiagoushi.top

Java: 方法内为块级作用域
来源：http://zff.guannengcc.top

Go:   花括号块级作用域
来源：http://llr.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xjr.jqgfzy.top

C#:   块级作用域
来源：http://rjc.yvedp.cn

[C11] 模块导入与导出
来源：http://dzz.dashuyun.cn

Py:   from module import func
来源：http://fhq.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://qhr.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://mgz.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://npg.wangshuangyany.cn

Java: import java.util.List;
来源：http://oua.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hhi.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jof.ydzc1.top

C#:   using System.Text;
来源：http://sag.vqdsnc.cn

[C12] 立即执行函数 IIFE
来源：http://xii.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://zis.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://yhi.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://psv.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://yta.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gdd.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://osg.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://knk.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mna.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://bqk.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://izb.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pnh.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dxb.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzg.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://elq.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://nfj.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ids.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://ldm.hongshengwenyu.top

[C14] 泛型函数
来源：http://inf.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ilb.hnxiangtu.top

PHP:  // 无泛型
来源：http://akn.ivvv.top

JS:   // 无泛型
来源：http://kzy.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://efe.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iwu.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ukf.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://ixl.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kit.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://nkf.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rzj.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://diu.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rkb.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nar.tarul.cn

Java: // 无解构
来源：http://qai.vqdsnc.cn

Go:   // 无解构
来源：http://jqc.chenjidiqi.icu

Ruby: a, b = pair
来源：http://fzz.yuxming.cn

C#:   var (a, b) = pair;
来源：http://wke.ydzc1.top

[C16] 函数 / 方法重载
来源：http://lyf.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wpo.dianchejie.cn

PHP:  // 无重载
来源：http://tjy.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://atl.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://skm.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://xck.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://nrv.ivvv.top

Ruby: # 无重载：靠动态参数
来源：http://jcd.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://wfm.yj20258888.top

================================================================================
来源：http://gin.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://zzw.shuidangran.top

================================================================================
来源：http://ruk.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://hsy.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qpt.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wyz.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eyi.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yhx.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://haf.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://vxm.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://ttm.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://res.hywenlv.cn

[D02] 追加元素到末尾
来源：http://vdo.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oml.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yif.zhoulong.xyz

JS:   arr.push(4);
来源：http://tpb.guowangkeji.top

TS:   arr.push(4);
来源：http://hef.jyoumei.cn


<!-- 参考信息 -->