代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qgf.zhaomingkeji.xyz

[B02] 多分支 else if / elif
来源：http://swo.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qji.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yui.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://adw.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxs.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sij.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qke.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://itw.pengpengdd.cyou

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eso.chenlongwang.top

[B03] switch / match / case
来源：http://ukb.zhongyouzk.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://quh.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zfh.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nny.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wux.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vmx.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pez.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fdt.52xcode.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kaz.dianchejie.cn

[B04] for 计数循环
来源：http://ovc.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://eps.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wio.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://czh.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aud.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wof.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ndi.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://qqx.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bhw.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://eqe.guannengcc.top

Py:   for item in arr: print(item)
来源：http://arn.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lda.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://los.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://tev.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lxx.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gex.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://eeb.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nbs.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://owo.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hbo.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ayc.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tyd.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bfj.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://srz.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://czd.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fpt.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gmm.yvedp.cn

[B07] while 循环
来源：http://hfi.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://xia.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://wwg.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://pwc.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://fru.epnwcf.com

Java: while (i < 10) { i++; }
来源：http://adg.ivvv.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zqk.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://vxm.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://jhz.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://pux.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://spd.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mev.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://tax.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://iyv.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://nzr.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://snd.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://zqr.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://ydp.cdnleiting.top

[B09] break 与 continue
来源：http://mis.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nhq.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iwg.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://voj.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdo.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nor.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sop.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ruk.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eif.gzhubu.top

[B10] 遍历同时拿索引
来源：http://iox.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bsc.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oov.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rbn.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gin.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rys.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ngq.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://civ.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wpv.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://iuw.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://zat.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://krq.yangfankeji.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sil.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jlo.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://krw.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yet.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://skg.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://djz.nwbrower.top

[B12] 跳出多层循环
来源：http://jdp.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jiq.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://bst.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dch.jqgfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ale.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://reo.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://evs.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gvf.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lar.bjfxy.top

[B13] 判断是否为数字
来源：http://jgp.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://zip.havefunace.top

PHP:  is_numeric($x)
来源：http://zso.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xtp.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://efh.c1oappe.top

Java: x instanceof Number
来源：http://ddz.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mwu.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://ezh.52xcode.cn

C#:   x is int or double or decimal
来源：http://ubp.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://mdy.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://awl.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gra.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://uib.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://ncm.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gfr.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mke.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://shl.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xwq.ivvv.top

[B15] 布尔运算与取反
来源：http://ejs.cqqwz.cn

Py:   a and b or not c
来源：http://pya.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://tyt.ehwqpu.com

JS:   a && b || !c
来源：http://tue.tarul.cn

TS:   a && b || !c
来源：http://frl.aizwys.cn

Java: a && b || !c
来源：http://tgu.ehwqpu.com

Go:   a && b || !c
来源：http://itr.meibo888.top

Ruby: a && b || !c
来源：http://rlh.bjfxy.top

C#:   a && b || !c
来源：http://tou.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tfj.52xcode.cn

Py:   if not data: return
来源：http://atm.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://aof.aizwys.cn

JS:   if (!data) return;
来源：http://vmj.316326.xyz

TS:   if (!data) return;
来源：http://xcb.bjfxy.top

Java: if (data == null) return;
来源：http://ezk.iojbl.cn

Go:   if data == nil { return }
来源：http://vkb.xuanzx.com

Ruby: return if data.nil?
来源：http://yxk.gogol.net.cn

C#:   if (data == null) return;
来源：http://kgn.hfpthk.cn

================================================================================
来源：http://hjh.zdbjq.cn

C. 函数与作用域
来源：http://uxl.tarul.cn

================================================================================
来源：http://aef.yangfankeji.com

[C01] 定义函数
来源：http://zlp.tarul.cn

Py:   def add(a, b): return a + b
来源：http://vqa.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://akk.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://yfz.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnv.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cwo.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xow.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://ser.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blk.yj20258.top

[C02] 默认参数
来源：http://bwc.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://ieb.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jwl.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://mar.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xtt.shanyushiyangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bbh.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yah.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://uiz.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://icd.shuidangran.top

[C03] 可变参数
来源：http://xzj.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://dmp.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jqh.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqc.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vbr.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rer.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xun.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://jxn.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pcj.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://hwg.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lss.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://glu.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iiq.yonumen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kza.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://ddw.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://lqj.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://syf.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://wti.aizwys.cn

[C05] 返回多个值
来源：http://fvv.redwolf501.top

Py:   return a, b
来源：http://pty.ydzc1.top

PHP:  return [$a, $b];
来源：http://czn.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sqk.snrcjt.cn

TS:   return { a, b };
来源：http://lcc.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mjp.xingfuxueyuan.xyz

Go:   return a, b
来源：http://khe.chenlongwang.top

Ruby: return a, b
来源：http://ngb.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://sja.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://liq.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://epk.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mwd.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://eeq.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://xsi.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pyt.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bvl.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ush.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://mjc.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://ydh.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dwn.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://cjh.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kle.zhoulong.xyz

TS:   arr.map(String)
来源：http://crc.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wtx.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jei.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://eud.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dpb.vqdsnc.cn

[C08] 闭包
来源：http://nbu.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oav.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mrb.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pfb.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jwg.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fhi.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xie.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nrb.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yok.kuanghao11.cn

[C09] 递归
来源：http://aer.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://abn.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zpa.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zda.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yyf.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gqq.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tht.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rfm.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pni.bjfxy.top

[C10] 变量作用域
来源：http://xqk.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ihj.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hcs.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mcq.cdnleiting.top

TS:   同 JS
来源：http://lqi.ehwqpu.com

Java: 方法内为块级作用域
来源：http://wba.zhixingplan.top

Go:   花括号块级作用域
来源：http://rso.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jba.jqgufenzy.top

C#:   块级作用域
来源：http://mfd.jyoumei.cn

[C11] 模块导入与导出
来源：http://woo.shanyushiyangtech.top

Py:   from module import func
来源：http://bxe.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hyc.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xmt.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ejt.xuetiantiany.cn

Java: import java.util.List;
来源：http://ubp.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nst.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://fxe.kuanghao11.cn

C#:   using System.Text;
来源：http://zwi.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://zqy.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://zli.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://afc.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://axo.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://hhu.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tuj.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://ipl.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://vrd.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://fbk.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://wos.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rjl.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qjl.shanyushiyangtech.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lri.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://abk.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://mzv.9152youxi.cn

Go:   func add(a, b int) int
来源：http://krv.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bkz.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://ggw.gotoacloud.top

[C14] 泛型函数
来源：http://ebf.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://azq.jiagoushi.top

PHP:  // 无泛型
来源：http://vlu.zhijiandao.cn

JS:   // 无泛型
来源：http://kgf.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dfv.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://clm.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rtb.xuetiantiany.cn

Ruby: # 无泛型
来源：http://ymc.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rqq.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://onu.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://izy.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://njk.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yru.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://elk.jinghuilouyu.cn

Java: // 无解构
来源：http://bam.yueranfly.top

Go:   // 无解构
来源：http://joq.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://xed.cashguo.top

C#:   var (a, b) = pair;
来源：http://lws.daria6918.cn

[C16] 函数 / 方法重载
来源：http://tya.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hwn.ydzc1.top

PHP:  // 无重载
来源：http://axi.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qpd.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://ghh.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iom.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://xfs.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://rcf.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vas.ywan-chungtsiang.top

================================================================================
来源：http://dpo.tanke756.top

D. 数组 / 列表 / 集合
来源：http://ioc.yangfankeji.com

================================================================================
来源：http://ydf.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://svr.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jeu.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mdm.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zpl.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://erc.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pyi.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://muj.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://tng.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rfu.tanke756.top

[D02] 追加元素到末尾
来源：http://ayy.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ssa.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qyn.pengpengdd.cyou

JS:   arr.push(4);
来源：http://bit.jlsjyb.cn

TS:   arr.push(4);
来源：http://fua.feifeiyinyue.top


<!-- 参考信息 -->