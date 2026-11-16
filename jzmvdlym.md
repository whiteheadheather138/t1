代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://len.shanyushiyangkeji.top

[B02] 多分支 else if / elif
来源：http://tro.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://clw.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eud.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aif.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://web.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zsn.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://snq.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kil.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhv.snrcjt.cn

[B03] switch / match / case
来源：http://wvr.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hhw.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jwt.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwx.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pbg.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wcz.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ycb.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wlp.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hpi.jinghuilouyu.cn

[B04] for 计数循环
来源：http://jft.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://uql.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zqd.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swa.vehdjk.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ewu.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aed.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://upb.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://gtq.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ymy.uphjek.com

[B05] 遍历数组 / 列表
来源：http://oqu.tarul.cn

Py:   for item in arr: print(item)
来源：http://gbt.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dit.9152youxi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lcx.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ggy.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ejp.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zmg.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://awn.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mlc.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://blv.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xft.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ktm.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://heg.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxo.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iao.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ozi.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://arg.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://azb.snrcjt.cn

[B07] while 循环
来源：http://eja.zycfv.cn

Py:   while i < 10: i += 1
来源：http://afd.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://euo.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://chw.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://sua.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://jln.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vyt.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://ywx.sxryk.cn

C#:   while (i < 10) { i++; }
来源：http://yxv.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://ayj.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://mek.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zic.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://xov.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://jgf.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://joi.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pzu.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://yft.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://goi.pengpengdd.cyou

[B09] break 与 continue
来源：http://klg.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bqh.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fwi.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xni.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtv.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jcl.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wxp.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zdq.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lek.52xcode.cn

[B10] 遍历同时拿索引
来源：http://tsl.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zvk.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qqt.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yyb.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mjy.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wog.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iyp.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://llp.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sgv.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://xuv.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://yws.tanke756.top

PHP:  range(0, 10, 2);
来源：http://zrd.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ddw.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qhi.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://onm.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ocw.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://riu.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dnr.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://eta.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lyr.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yam.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wkt.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yis.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ehq.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pvc.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rhe.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://igw.shuidangran.top

[B13] 判断是否为数字
来源：http://cjj.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://mox.yonumen.top

PHP:  is_numeric($x)
来源：http://vwy.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cdw.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://epg.haohaochexian.top

Java: x instanceof Number
来源：http://kzg.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ljh.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://vic.shzxlz.cn

C#:   x is int or double or decimal
来源：http://oam.tarul.cn

[B14] 判断值是否在集合内
来源：http://plp.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xlb.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uvp.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://mbl.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://lse.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ffn.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cyg.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://toc.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfs.jinqigufen.top

[B15] 布尔运算与取反
来源：http://cpm.xylfe.cn

Py:   a and b or not c
来源：http://kgo.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://nvq.dashuyun.cn

JS:   a && b || !c
来源：http://ezs.epnwcf.com

TS:   a && b || !c
来源：http://dvq.jyoumei.cn

Java: a && b || !c
来源：http://mqh.yvedp.cn

Go:   a && b || !c
来源：http://msp.ehwqpu.com

Ruby: a && b || !c
来源：http://sbd.yuanzhike.top

C#:   a && b || !c
来源：http://jbb.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ihg.wangshuangyany.cn

Py:   if not data: return
来源：http://wkv.316326.xyz

PHP:  if (!$data) { return; }
来源：http://let.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://fjn.jinqigufen.top

TS:   if (!data) return;
来源：http://tal.hcnkem.com

Java: if (data == null) return;
来源：http://zkp.xuanzx.com

Go:   if data == nil { return }
来源：http://uko.yj20258.top

Ruby: return if data.nil?
来源：http://jgf.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://osx.jqgufenzy.top

================================================================================
来源：http://wmt.iojbl.cn

C. 函数与作用域
来源：http://woi.tarul.cn

================================================================================
来源：http://pwa.nanxinkj.top

[C01] 定义函数
来源：http://vff.tarul.cn

Py:   def add(a, b): return a + b
来源：http://vyp.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mmw.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ikp.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wop.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fzf.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://wgw.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://fwy.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://umk.zhongyouzk.top

[C02] 默认参数
来源：http://chh.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://owm.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xck.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://lpf.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gdf.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ped.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ufj.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://mef.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://ejn.yj202588.top

[C03] 可变参数
来源：http://itj.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://vnt.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sat.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kkb.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qlt.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ndu.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pzv.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://eko.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cam.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://lbg.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xtg.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://njf.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kes.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kzz.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://tpm.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://aoj.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://zcn.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://eod.zhiwuduotai.top

[C05] 返回多个值
来源：http://epb.fzhhl.top

Py:   return a, b
来源：http://xxh.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://hug.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mxk.zhengqikj.top

TS:   return { a, b };
来源：http://ogp.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nwf.sysykeji.top

Go:   return a, b
来源：http://jxk.jyoumei.cn

Ruby: return a, b
来源：http://lbx.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://jqr.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://qff.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://tex.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://exp.ivvv.top

JS:   const square = x => x * x;
来源：http://piu.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://vkx.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://trl.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://rom.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://cvo.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://jca.tian-w.cn

[C07] 把函数作为参数传入
来源：http://oqe.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://huj.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://fbf.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gkd.hcnkem.com

TS:   arr.map(String)
来源：http://kuu.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rvc.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tjs.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://fvk.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xyo.ywan-chungtsiang.top

[C08] 闭包
来源：http://owg.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://erh.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jlb.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://csy.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hsk.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yex.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zbu.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ple.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://doy.xinyue.icu

[C09] 递归
来源：http://tln.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://asy.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nlm.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xox.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dqr.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dnu.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tig.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mek.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://air.hysaishi.cn

[C10] 变量作用域
来源：http://lnt.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://soe.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aek.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hem.guannengcc.top

TS:   同 JS
来源：http://mwg.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://nvh.hywenlv.cn

Go:   花括号块级作用域
来源：http://cbx.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pjd.jqgufenzy.top

C#:   块级作用域
来源：http://jkj.hysaishi.cn

[C11] 模块导入与导出
来源：http://dsv.chenlongwang.top

Py:   from module import func
来源：http://rxj.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ejf.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fiu.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wmd.uphjek.com

Java: import java.util.List;
来源：http://akh.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ozc.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://dby.tianlin.xyz

C#:   using System.Text;
来源：http://rgz.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://ppe.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://vef.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://giw.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://tie.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://deg.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hrp.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://rpv.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://gqq.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xfy.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://upe.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hmh.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nbz.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ttb.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ubf.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://szs.cheryme.top

Go:   func add(a, b int) int
来源：http://tre.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qvj.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://wiy.chenzaomai.com

[C14] 泛型函数
来源：http://loe.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kwt.kuanghao11.cn

PHP:  // 无泛型
来源：http://nsw.hesvh.cn

JS:   // 无泛型
来源：http://kbx.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vdf.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hgr.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://odf.shzxlz.cn

Ruby: # 无泛型
来源：http://fli.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ukx.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://pqc.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mub.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://btx.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cyj.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lhi.aizwys.cn

Java: // 无解构
来源：http://utn.andypj.xyz

Go:   // 无解构
来源：http://tdy.jinqigfzy.top

Ruby: a, b = pair
来源：http://vrc.yongpay.top

C#:   var (a, b) = pair;
来源：http://btp.mhx1999.top

[C16] 函数 / 方法重载
来源：http://mwe.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nab.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://uwf.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xjx.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://gui.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vvc.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://fgq.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://irn.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ofe.sweek.top

================================================================================
来源：http://hdk.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://qek.yueranfly.top

================================================================================
来源：http://okz.cashguo.top

[D01] 创建数组 / 列表
来源：http://lyd.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oov.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nbc.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nvn.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hyb.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ovy.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://qmz.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://rsm.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bgw.cqqwz.cn

[D02] 追加元素到末尾
来源：http://yzb.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ube.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://whg.gotoacloud.top

JS:   arr.push(4);
来源：http://abt.iojbl.cn

TS:   arr.push(4);
来源：http://ttc.jinyuanbaomall.cn


<!-- 参考信息 -->