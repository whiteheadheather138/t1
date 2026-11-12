代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mzn.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://xvm.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ujh.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zin.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwx.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vcf.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ied.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pll.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ikx.daria6918.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhl.52xcode.cn

[B03] switch / match / case
来源：http://piy.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uql.nanxinkj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wkg.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://enh.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oxu.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mav.ydzc1.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vry.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mpz.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rpa.ctjpmb.com

[B04] for 计数循环
来源：http://jiu.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://wwj.c1oappe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vbe.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wtc.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://giq.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pcj.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vpv.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://oyc.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qta.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://xfg.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://hnj.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ytp.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ivz.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://vqw.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://srh.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ish.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://hfx.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tdr.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://wjj.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mxa.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mqx.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ikt.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://koy.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zds.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xec.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://egn.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://buz.tianlin.xyz

[B07] while 循环
来源：http://wlo.xuanzx.com

Py:   while i < 10: i += 1
来源：http://utf.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://bxm.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://fbq.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://yvy.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://kiq.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rbi.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://jib.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://igy.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://hmw.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://ayk.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fvk.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://hzm.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://ymo.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://uih.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ecz.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://euc.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://fah.52xcode.cn

[B09] break 与 continue
来源：http://wno.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sxy.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://elz.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myt.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbs.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hkl.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fhv.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wge.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://krn.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://dbu.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://krf.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xiw.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qpb.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ptb.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://myb.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yzf.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iun.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bse.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://wks.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://uyc.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://dvf.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cwn.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dow.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://smj.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wnv.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://ihp.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://trf.birdmap.top

[B12] 跳出多层循环
来源：http://mfw.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ups.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fdx.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uvb.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zca.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://keu.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zof.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qec.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hpj.daxiang520.top

[B13] 判断是否为数字
来源：http://sdd.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://aox.zhengqikj.top

PHP:  is_numeric($x)
来源：http://iqx.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lqg.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://owh.smart0.xyz

Java: x instanceof Number
来源：http://dsm.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://riv.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://qfz.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://ktd.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://csw.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oxk.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fhj.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://hbf.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://wlt.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://anw.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wor.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xdw.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gcx.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://yje.smart0.xyz

Py:   a and b or not c
来源：http://mjb.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://sjl.cashguo.top

JS:   a && b || !c
来源：http://mte.xuetiantiany.cn

TS:   a && b || !c
来源：http://vxw.cashguo.top

Java: a && b || !c
来源：http://qhx.feifeiyinyue.top

Go:   a && b || !c
来源：http://uxy.gogol.net.cn

Ruby: a && b || !c
来源：http://pyo.ydjk.org.cn

C#:   a && b || !c
来源：http://sjx.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://paj.xylfe.cn

Py:   if not data: return
来源：http://dbr.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://pxz.yuanzhike.top

JS:   if (!data) return;
来源：http://itw.fzhhl.top

TS:   if (!data) return;
来源：http://nst.sysykeji.top

Java: if (data == null) return;
来源：http://ggw.quarkkingdee.top

Go:   if data == nil { return }
来源：http://awo.gotoacloud.top

Ruby: return if data.nil?
来源：http://hfl.daria6918.cn

C#:   if (data == null) return;
来源：http://ykw.yuanzhike.top

================================================================================
来源：http://jdp.sufxvd.cn

C. 函数与作用域
来源：http://fsv.guowangkeji.top

================================================================================
来源：http://zrh.yj202588.top

[C01] 定义函数
来源：http://qbd.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://qqq.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xsn.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://zcq.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cxd.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mun.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://ybi.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://ush.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ksy.hammf.cn

[C02] 默认参数
来源：http://lnq.yj202588.top

Py:   def greet(name="World"): return name
来源：http://bss.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://szh.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://rat.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://bof.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://yqo.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wvv.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://qgo.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://unc.vqdsnc.cn

[C03] 可变参数
来源：http://pne.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://dip.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jnm.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qih.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pyb.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gbn.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://spi.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gng.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zhi.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://cma.havefunace.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rbx.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mlj.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pgh.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mby.tarul.cn

Java: // 无：用 Builder 模式或 record
来源：http://whm.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://fld.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://uow.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://lqe.jinghuilouyu.cn

[C05] 返回多个值
来源：http://skj.xuetiantiany.cn

Py:   return a, b
来源：http://rqv.guannengcc.top

PHP:  return [$a, $b];
来源：http://dxk.pycfn.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://gsj.snrcjt.cn

TS:   return { a, b };
来源：http://tin.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://czw.wangdashe.top

Go:   return a, b
来源：http://lqf.nanxuanxn.top

Ruby: return a, b
来源：http://nyv.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://kjt.tarul.cn

[C06] 匿名函数 / lambda
来源：http://bok.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://vaj.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rit.fktsv.cn

JS:   const square = x => x * x;
来源：http://uev.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://fwa.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tqj.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://wao.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://ltn.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://txu.yj202588.top

[C07] 把函数作为参数传入
来源：http://hol.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dsn.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://ymr.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tzp.xuanzx.com

TS:   arr.map(String)
来源：http://tuw.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dqy.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xqf.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://tan.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://tad.c1oappe.top

[C08] 闭包
来源：http://lcn.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://maf.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tlv.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qty.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://msx.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://okz.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://umn.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://khe.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gyl.meibo888.top

[C09] 递归
来源：http://vje.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://amf.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://joe.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ihw.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ekc.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mnf.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nmv.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tzs.shanyushiyangtech.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rpz.gzhubu.top

[C10] 变量作用域
来源：http://mrn.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kxh.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wke.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://svm.zhijiandao.cn

TS:   同 JS
来源：http://sxg.fzhhl.top

Java: 方法内为块级作用域
来源：http://mzj.yanxiufei.cn

Go:   花括号块级作用域
来源：http://wnv.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rsh.cucudq.cn

C#:   块级作用域
来源：http://auv.zdbjq.cn

[C11] 模块导入与导出
来源：http://fqd.dashuyun.cn

Py:   from module import func
来源：http://wup.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sqk.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wtx.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://unz.andypj.xyz

Java: import java.util.List;
来源：http://bpu.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jpt.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://koc.zhixingplan.top

C#:   using System.Text;
来源：http://rfw.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://xvq.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://oni.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://qsx.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://ipe.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://crq.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cfi.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://dhu.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://svf.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://maz.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://bpf.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvl.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dpa.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xwy.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ofy.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://aru.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://cyu.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vqj.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://hol.daxiang520.top

[C14] 泛型函数
来源：http://biz.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kyz.daria6918.cn

PHP:  // 无泛型
来源：http://arq.chenzaomai.com

JS:   // 无泛型
来源：http://gcq.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ugy.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lpe.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tts.yj20258.top

Ruby: # 无泛型
来源：http://ofl.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aaf.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://twk.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://odf.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://fum.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pfp.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zyj.redwolf501.top

Java: // 无解构
来源：http://bzs.cucudq.cn

Go:   // 无解构
来源：http://kxl.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://llf.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://isi.316326.xyz

[C16] 函数 / 方法重载
来源：http://tcw.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://veo.gaohongyu789.top

PHP:  // 无重载
来源：http://nkh.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nra.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://bgf.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fku.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://gtl.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://mdb.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://edz.tarul.cn

================================================================================
来源：http://ffj.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://xxd.cdnleiting.top

================================================================================
来源：http://xrx.fehbvm.com

[D01] 创建数组 / 列表
来源：http://rqf.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cgc.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://srq.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://asn.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://loy.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nya.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://pvx.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://cwg.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://riv.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://xam.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qzn.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ojb.yvedp.cn

JS:   arr.push(4);
来源：http://vyc.chenjidiqi.icu

TS:   arr.push(4);
来源：http://vfr.birdmap.top


<!-- 参考信息 -->