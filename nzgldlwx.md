代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jgp.sweek.top

[B02] 多分支 else if / elif
来源：http://zdx.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cye.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://khn.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ykm.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tru.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdq.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dts.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://war.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfl.yj202588.top

[B03] switch / match / case
来源：http://txc.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://agt.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aku.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bkv.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pmw.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wbq.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xap.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nvb.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jku.redwolf501.top

[B04] for 计数循环
来源：http://wzq.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://sks.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ykd.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lln.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vuw.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://asa.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zph.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://nsb.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rqh.daria6918.cn

[B05] 遍历数组 / 列表
来源：http://yfh.sweek.top

Py:   for item in arr: print(item)
来源：http://gdc.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gyx.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ktd.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zrl.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://uys.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aev.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://esa.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qto.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://yqv.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fgu.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wdv.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ocf.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vhz.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lny.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tev.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xnj.gaohongyu789.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ycw.svipenyu.cn

[B07] while 循环
来源：http://dfm.wangdashe.top

Py:   while i < 10: i += 1
来源：http://xvs.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://syh.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://xzm.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://tbf.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://ufo.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rpc.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://qlu.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://vtf.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://yxc.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://iuf.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jjz.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://klc.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://fyc.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://lkp.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vfg.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lty.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://yhr.hesvh.cn

[B09] break 与 continue
来源：http://mcj.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nor.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vap.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptb.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbp.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gim.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iee.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iyg.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com

[B10] 遍历同时拿索引
来源：http://yae.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lhn.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wer.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gly.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oxp.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mcc.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rjc.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dkf.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rkw.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://maj.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://kmu.birdmap.top

PHP:  range(0, 10, 2);
来源：http://you.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxy.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://khb.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vcn.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xol.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://uep.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xsx.fengsongda.top

[B12] 跳出多层循环
来源：http://yix.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kgt.aizwys.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vnx.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zal.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wuh.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zbp.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://frk.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jzg.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tvw.guowangkeji.top

[B13] 判断是否为数字
来源：http://fbh.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://yxd.daxiang520.top

PHP:  is_numeric($x)
来源：http://avh.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nml.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ovr.cucudq.cn

Java: x instanceof Number
来源：http://mhc.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rhh.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://kwu.xuanzx.com

C#:   x is int or double or decimal
来源：http://eaq.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://xho.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rgf.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zjk.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://xuy.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://btl.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fya.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://odb.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://aeh.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://odk.bjfxy.top

[B15] 布尔运算与取反
来源：http://zpa.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://qea.sxryk.cn

PHP:  $a && $b || !$c
来源：http://cdv.yuxming.cn

JS:   a && b || !c
来源：http://okt.cheryme.top

TS:   a && b || !c
来源：http://hhg.wangshuangyany.cn

Java: a && b || !c
来源：http://vsa.xziqi.cn

Go:   a && b || !c
来源：http://vre.cucudq.cn

Ruby: a && b || !c
来源：http://mxr.shanyushiyangtech.top

C#:   a && b || !c
来源：http://ixw.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://dlo.ybcxt.top

Py:   if not data: return
来源：http://xiu.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://ljk.hesvh.cn

JS:   if (!data) return;
来源：http://bax.shangyingyoupin.top

TS:   if (!data) return;
来源：http://dzd.316326.xyz

Java: if (data == null) return;
来源：http://lig.wangdashe.top

Go:   if data == nil { return }
来源：http://awg.fzhhl.top

Ruby: return if data.nil?
来源：http://dgf.sysykeji.top

C#:   if (data == null) return;
来源：http://sdr.sweek.top

================================================================================
来源：http://dpj.redwolf501.top

C. 函数与作用域
来源：http://ypy.ivvv.top

================================================================================
来源：http://vxy.sufxvd.cn

[C01] 定义函数
来源：http://zqw.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://hkq.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qmv.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://ktc.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fzj.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://pms.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://lnx.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://jkw.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rcm.bbcook.cn

[C02] 默认参数
来源：http://hrv.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://awt.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://eqk.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://abn.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://buf.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://umh.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lzh.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://dvt.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://inu.fengsongda.top

[C03] 可变参数
来源：http://gnv.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://hdg.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://krf.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zau.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lkm.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hch.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vlz.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nrh.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://byt.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://hpf.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://myj.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://njq.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gmm.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qcv.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://sri.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://kbc.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://cpp.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://dlb.wangdashe.top

[C05] 返回多个值
来源：http://ypm.uphjek.com

Py:   return a, b
来源：http://ubb.redwolf501.top

PHP:  return [$a, $b];
来源：http://oho.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ksb.yj20258888.top

TS:   return { a, b };
来源：http://fep.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jui.kuanghao11.cn

Go:   return a, b
来源：http://ndm.pycfn.com

Ruby: return a, b
来源：http://qan.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://ghd.yonumen.top

[C06] 匿名函数 / lambda
来源：http://zjn.yj202588.top

Py:   square = lambda x: x * x
来源：http://qod.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bnu.ctjpmb.com

JS:   const square = x => x * x;
来源：http://joa.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://ciy.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yfi.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://ezh.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://bmc.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://vfh.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://isr.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bzd.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://erj.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lzr.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://seo.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rdl.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ucu.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://gda.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://lvi.meibo888.top

[C08] 闭包
来源：http://udx.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://adm.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://den.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tmh.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wqu.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://odj.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gdk.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kpq.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ott.xingfuxueyuan.xyz

[C09] 递归
来源：http://zpn.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rgk.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nus.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zlc.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jfu.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yxr.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://khc.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yxu.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bmx.gaohongyu789.top

[C10] 变量作用域
来源：http://bht.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wow.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nal.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rdd.tarul.cn

TS:   同 JS
来源：http://lmh.0kj1m.cn

Java: 方法内为块级作用域
来源：http://ism.fktsv.cn

Go:   花括号块级作用域
来源：http://kho.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sio.sxryk.cn

C#:   块级作用域
来源：http://dkm.quarkkingdee.top

[C11] 模块导入与导出
来源：http://ptc.ppjwa.cn

Py:   from module import func
来源：http://wzj.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ads.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jfe.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fbr.haohaochexian.top

Java: import java.util.List;
来源：http://hdv.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pjf.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://zqn.tarul.cn

C#:   using System.Text;
来源：http://lhz.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://pdy.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://bjb.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://jmd.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://qfy.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://qnv.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jot.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://ysq.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://vzi.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wqs.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://jrl.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gon.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jeg.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://amc.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://top.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://fjx.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://gnk.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ylr.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gfn.jlsjyb.cn

[C14] 泛型函数
来源：http://ehp.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ley.316326.xyz

PHP:  // 无泛型
来源：http://fkm.yfazqb.com

JS:   // 无泛型
来源：http://fha.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gij.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uhc.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vru.nanxuanxn.top

Ruby: # 无泛型
来源：http://plv.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rth.yvedp.cn

[C15] 解构 / 展开参数
来源：http://bit.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mhq.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://wvs.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qmk.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fsm.ivvv.top

Java: // 无解构
来源：http://qat.jinqigufen.top

Go:   // 无解构
来源：http://zur.jianghu66.top

Ruby: a, b = pair
来源：http://nvn.iojbl.cn

C#:   var (a, b) = pair;
来源：http://gbw.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://zrt.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oum.smart0.xyz

PHP:  // 无重载
来源：http://usb.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://cuz.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://hxk.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://weo.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://utx.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://ihe.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wmq.shuidangran.top

================================================================================
来源：http://jky.cheryme.top

D. 数组 / 列表 / 集合
来源：http://dqe.jqgfzy.top

================================================================================
来源：http://lya.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://rhh.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rys.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rpj.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yyb.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ant.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jdw.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://jfa.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://jlh.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uas.sweek.top

[D02] 追加元素到末尾
来源：http://dmo.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bsl.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://flx.jianghu66.top

JS:   arr.push(4);
来源：http://wqg.andypj.xyz

TS:   arr.push(4);
来源：http://tlm.shangyingyoupin.top


<!-- 参考信息 -->