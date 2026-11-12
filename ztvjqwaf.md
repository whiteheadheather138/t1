代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bio.daxiang520.top

[B02] 多分支 else if / elif
来源：http://rfe.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bwq.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wgv.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgp.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtz.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhp.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cpp.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fez.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oow.pengpengdd.cyou

[B03] switch / match / case
来源：http://ugb.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fuq.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nqr.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ksg.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgp.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xkd.hnqzz.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://agr.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zmt.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wli.yfazqb.com

[B04] for 计数循环
来源：http://dfo.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://yvk.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hld.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ixw.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bqv.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tjy.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hue.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://ytr.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hku.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://tuv.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://tgx.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ejv.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uuo.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kzm.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ovj.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dct.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://nji.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nne.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://vuk.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qdn.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://smn.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gjd.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ehr.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqq.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yhl.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ksj.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://clk.fzhhl.top

[B07] while 循环
来源：http://qzl.fehbvm.com

Py:   while i < 10: i += 1
来源：http://lcs.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bgg.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://zgd.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://sue.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://nqu.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aiq.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://xka.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://eys.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://evg.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ejm.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cma.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://vxr.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://mqk.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://xrf.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aju.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://wyu.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://xqg.snrcjt.cn

[B09] break 与 continue
来源：http://wvu.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dpf.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yot.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsy.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tqt.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nec.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kfh.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nnc.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cli.cucudq.cn

[B10] 遍历同时拿索引
来源：http://kig.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://izg.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zvi.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sti.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ily.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nwe.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ikz.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kgp.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ofe.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://lvi.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://qsc.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://yii.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://evv.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://odu.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fma.yueranfly.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fxg.pycfn.com

Ruby: (0...10).step(2).to_a
来源：http://tvv.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://goo.tarul.cn

[B12] 跳出多层循环
来源：http://zeu.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jle.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cpa.xingfuxueyuan.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jho.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mrp.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lml.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yql.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wzo.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hii.snrcjt.cn

[B13] 判断是否为数字
来源：http://wza.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://tvz.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://idu.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wuv.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://abg.nanxuanxn.top

Java: x instanceof Number
来源：http://pap.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hop.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://krx.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://bgi.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://zkr.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dbd.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hho.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://cax.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://xbv.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bye.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgw.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://wcq.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pud.yongpay.top

[B15] 布尔运算与取反
来源：http://hre.yuxming.cn

Py:   a and b or not c
来源：http://wgu.guannengcc.top

PHP:  $a && $b || !$c
来源：http://tme.hammf.cn

JS:   a && b || !c
来源：http://fxe.yangfankeji.com

TS:   a && b || !c
来源：http://gcq.zhoulong.xyz

Java: a && b || !c
来源：http://gjb.pycfn.com

Go:   a && b || !c
来源：http://wxh.jinqigufen.top

Ruby: a && b || !c
来源：http://tzn.dashuyun.cn

C#:   a && b || !c
来源：http://fqu.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://eyz.jinqigufen.top

Py:   if not data: return
来源：http://hqs.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://mgp.shzxlz.cn

JS:   if (!data) return;
来源：http://jix.yuanzhike.top

TS:   if (!data) return;
来源：http://qvd.hammf.cn

Java: if (data == null) return;
来源：http://tml.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://tdp.bjfxy.top

Ruby: return if data.nil?
来源：http://zku.zhengqikj.top

C#:   if (data == null) return;
来源：http://knq.ywan-chungtsiang.top

================================================================================
来源：http://seu.redwolf501.top

C. 函数与作用域
来源：http://kwn.hesvh.cn

================================================================================
来源：http://vtr.chenjidiqi.icu

[C01] 定义函数
来源：http://hlo.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://wuh.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yua.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://vtq.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://utv.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ehr.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lkl.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://nhd.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qwg.xuetiantiany.cn

[C02] 默认参数
来源：http://qfx.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://mru.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://elr.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://oks.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nna.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gcv.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mxw.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://oec.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://xjp.jinghuilouyu.cn

[C03] 可变参数
来源：http://gmn.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://xvr.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cpb.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cty.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwj.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ykv.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ajj.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://duw.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://srl.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://kvs.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uha.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sqg.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gdt.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bmi.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://mmj.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://jky.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://dax.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://dug.hcnkem.com

[C05] 返回多个值
来源：http://cpq.ehwqpu.com

Py:   return a, b
来源：http://vek.bjfxy.top

PHP:  return [$a, $b];
来源：http://nun.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://nts.feifeiyinyue.top

TS:   return { a, b };
来源：http://vgr.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vqk.jinghuilouyu.cn

Go:   return a, b
来源：http://psk.wangdashe.top

Ruby: return a, b
来源：http://lct.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://kit.yj20258.top

[C06] 匿名函数 / lambda
来源：http://jqw.yongpay.top

Py:   square = lambda x: x * x
来源：http://yiz.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uuw.52xcode.cn

JS:   const square = x => x * x;
来源：http://sev.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://nko.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://shv.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ryv.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://qcf.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dqd.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://dch.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://agr.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://anl.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yfq.hammf.cn

TS:   arr.map(String)
来源：http://pih.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xob.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mfp.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://jqz.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://crh.zhengqikj.top

[C08] 闭包
来源：http://mlf.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qfi.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://axg.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://huo.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dfl.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gbp.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sai.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wdw.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dqi.fktsv.cn

[C09] 递归
来源：http://vbn.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dvy.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zkt.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ujb.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oim.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tfo.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://war.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hcw.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oot.daria6918.cn

[C10] 变量作用域
来源：http://gdz.xuanzx.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bho.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lpv.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jgk.havefunace.top

TS:   同 JS
来源：http://wmb.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://fpl.jianghu66.top

Go:   花括号块级作用域
来源：http://bcu.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zyw.dashuyun.cn

C#:   块级作用域
来源：http://pjc.meibo888.top

[C11] 模块导入与导出
来源：http://buo.tarul.cn

Py:   from module import func
来源：http://rfx.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xvp.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jxu.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cva.yongpay.top

Java: import java.util.List;
来源：http://uuq.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gkv.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://lta.uphjek.com

C#:   using System.Text;
来源：http://wvp.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://jfd.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://pnp.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://bct.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://ruh.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://etj.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kvb.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://liq.sweek.top

Ruby: -> { puts "run" }.call
来源：http://sit.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qyz.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://csu.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://whe.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edj.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ien.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vuj.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oxb.zdqjudy.top

Go:   func add(a, b int) int
来源：http://gky.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eff.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://bsx.cdnleiting.top

[C14] 泛型函数
来源：http://lxg.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tkm.guowangkeji.top

PHP:  // 无泛型
来源：http://pvi.yfazqb.com

JS:   // 无泛型
来源：http://bvx.jinghuilouyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lbs.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wyo.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vqi.havefunace.top

Ruby: # 无泛型
来源：http://opr.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xqq.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://hne.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hnc.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://tma.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pzc.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pjy.vqdsnc.cn

Java: // 无解构
来源：http://vir.cucudq.cn

Go:   // 无解构
来源：http://wiy.zdbjq.cn

Ruby: a, b = pair
来源：http://bkc.wangdashe.top

C#:   var (a, b) = pair;
来源：http://xbr.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://kxz.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ngu.nanxuanxn.top

PHP:  // 无重载
来源：http://daq.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hcf.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://bpg.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gdu.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://jxg.zdbjq.cn

Ruby: # 无重载：靠动态参数
来源：http://dsc.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://zel.daxiang520.top

================================================================================
来源：http://obv.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://rcf.ctjpmb.com

================================================================================
来源：http://fub.yuxming.cn

[D01] 创建数组 / 列表
来源：http://mfl.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ntz.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kuc.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qhv.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://zma.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://brj.zhoulong.xyz

Go:   arr := []int{1, 2, 3}
来源：http://fii.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://qts.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rkf.xuanzx.com

[D02] 追加元素到末尾
来源：http://mwy.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fyd.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cis.uphjek.com

JS:   arr.push(4);
来源：http://rke.sxryk.cn

TS:   arr.push(4);
来源：http://yun.zhengqikj.top


<!-- 参考信息 -->