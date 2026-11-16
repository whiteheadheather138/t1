代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://unr.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://vkf.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://naz.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kic.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwo.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rrl.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzi.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xyq.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rhe.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbe.zycfv.cn

[B03] switch / match / case
来源：http://kim.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dpj.shzxlz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://byh.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://exq.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ukz.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tlr.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bgy.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://czi.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ckb.yongpay.top

[B04] for 计数循环
来源：http://mya.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://wxm.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vac.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qdg.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vew.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vjr.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xja.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://cqr.tian-w.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ato.zhijiandao.cn

[B05] 遍历数组 / 列表
来源：http://maj.shuidangran.top

Py:   for item in arr: print(item)
来源：http://ubn.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bno.cdnleiting.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gkd.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sak.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ijg.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blx.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://inl.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xgz.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://lmc.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vjr.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://quy.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hzp.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xrq.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gtw.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pzy.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gbq.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gyb.birdmap.top

[B07] while 循环
来源：http://cjq.hnqzz.top

Py:   while i < 10: i += 1
来源：http://bqy.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lwb.zhoulong.xyz

JS:   while (i < 10) { i++; }
来源：http://nej.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://lth.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://llm.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rtu.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://elt.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://hnq.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://qzv.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://hhz.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qrk.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://qmn.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://bci.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://yxz.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jee.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://qok.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://wuq.fengsongda.top

[B09] break 与 continue
来源：http://cme.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qwr.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mpl.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ody.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvb.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdd.mhx1999.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hgz.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uwh.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myx.xinyue.icu

[B10] 遍历同时拿索引
来源：http://gya.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cyj.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://daw.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mjh.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gar.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://btr.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zea.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://whx.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jcd.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://whi.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://efu.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://nan.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgy.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qcj.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fxb.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nyb.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://ybw.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tpc.jianghu66.top

[B12] 跳出多层循环
来源：http://epu.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zst.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://epr.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://udj.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://drq.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uqu.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sbi.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nro.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zhv.andypj.xyz

[B13] 判断是否为数字
来源：http://tao.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://zpv.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://ria.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yqn.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elx.pengpengdd.cyou

Java: x instanceof Number
来源：http://bnn.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vqj.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://cif.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://dor.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://bve.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://npd.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://czs.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://qbx.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://sxs.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jdg.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zja.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://sqe.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xfq.jianghu66.top

[B15] 布尔运算与取反
来源：http://ocb.cdnleiting.top

Py:   a and b or not c
来源：http://pmb.yj20258888.top

PHP:  $a && $b || !$c
来源：http://sos.fanxiaobao.xyz

JS:   a && b || !c
来源：http://dnx.daxiang520.top

TS:   a && b || !c
来源：http://lwy.guannengcc.top

Java: a && b || !c
来源：http://fgg.yuxming.cn

Go:   a && b || !c
来源：http://yvl.daxiang520.top

Ruby: a && b || !c
来源：http://cpb.cashguo.top

C#:   a && b || !c
来源：http://lzv.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://anq.hywenlv.cn

Py:   if not data: return
来源：http://zta.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://bws.tianlin.xyz

JS:   if (!data) return;
来源：http://hph.snrcjt.cn

TS:   if (!data) return;
来源：http://axv.jiagoushi.top

Java: if (data == null) return;
来源：http://bgj.ivvv.top

Go:   if data == nil { return }
来源：http://lgy.ydzc1.top

Ruby: return if data.nil?
来源：http://nxf.gaohongyu789.top

C#:   if (data == null) return;
来源：http://pyk.gotoacloud.top

================================================================================
来源：http://qxx.shanyushiyangkeji.top

C. 函数与作用域
来源：http://men.ydjk.org.cn

================================================================================
来源：http://elb.tanke756.top

[C01] 定义函数
来源：http://kih.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://rdo.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://laq.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://bvy.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bgt.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pai.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://ekg.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://chr.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uud.zycfv.cn

[C02] 默认参数
来源：http://cfb.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://fva.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sww.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://cxr.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nap.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://oxw.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qlr.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://xnk.chenlongwang.top

C#:   string Greet(string name = "World") => name;
来源：http://ylj.chenjidiqi.icu

[C03] 可变参数
来源：http://fof.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://ksz.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tej.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://puf.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vld.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kge.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xzj.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qbl.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vxo.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://icm.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lql.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pkq.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dmh.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wgb.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://csd.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://gjc.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://ltn.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://phs.cdnleiting.top

[C05] 返回多个值
来源：http://efd.chenzaomai.com

Py:   return a, b
来源：http://ell.gzhubu.top

PHP:  return [$a, $b];
来源：http://fbm.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ldd.aizwys.cn

TS:   return { a, b };
来源：http://kcn.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ruq.52xcode.cn

Go:   return a, b
来源：http://zby.bjfxy.top

Ruby: return a, b
来源：http://blx.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://hic.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://cgp.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://evr.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://upy.yj202588.top

JS:   const square = x => x * x;
来源：http://jdi.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://zcm.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fbk.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://qrj.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://qyz.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://pcs.yuxming.cn

[C07] 把函数作为参数传入
来源：http://kmg.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lwi.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://ezl.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wkk.hcnkem.com

TS:   arr.map(String)
来源：http://utq.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fzl.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fhj.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://ofy.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lsa.c1oappe.top

[C08] 闭包
来源：http://ufe.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lhx.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rkd.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hgx.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bbk.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://inm.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cwj.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tyi.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uos.redwolf501.top

[C09] 递归
来源：http://qyg.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nze.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xox.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ndu.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwv.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://slc.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lip.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jki.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tij.cashguo.top

[C10] 变量作用域
来源：http://ayo.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://njn.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iiq.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lla.gogol.net.cn

TS:   同 JS
来源：http://fsw.tarul.cn

Java: 方法内为块级作用域
来源：http://lju.bbcook.cn

Go:   花括号块级作用域
来源：http://jgt.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://drz.nwbrower.top

C#:   块级作用域
来源：http://jcf.c1oappe.top

[C11] 模块导入与导出
来源：http://kme.xinyue.icu

Py:   from module import func
来源：http://yfq.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rib.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xae.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qgw.jqgufenzy.top

Java: import java.util.List;
来源：http://ynh.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jva.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://xvw.gogol.net.cn

C#:   using System.Text;
来源：http://flm.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://mpx.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://syk.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://oqh.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://bim.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://peo.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jhd.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://yxd.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://xib.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ymw.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://zqw.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lph.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jtz.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fsb.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://had.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://qti.hywenlv.cn

Go:   func add(a, b int) int
来源：http://xwe.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yrd.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://pkn.smart0.xyz

[C14] 泛型函数
来源：http://rux.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qha.tianlin.xyz

PHP:  // 无泛型
来源：http://xwv.yvedp.cn

JS:   // 无泛型
来源：http://mru.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gyc.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nri.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fbv.vqdsnc.cn

Ruby: # 无泛型
来源：http://mkg.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dwp.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://kqn.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pri.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://khv.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nus.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://opk.tanke756.top

Java: // 无解构
来源：http://dsk.xylfe.cn

Go:   // 无解构
来源：http://nfu.hysaishi.cn

Ruby: a, b = pair
来源：http://dlu.bjfxy.top

C#:   var (a, b) = pair;
来源：http://vzh.ivvv.top

[C16] 函数 / 方法重载
来源：http://kho.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nss.redwolf501.top

PHP:  // 无重载
来源：http://vkp.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zvn.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://wtr.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cuf.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://ayk.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://jln.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://duo.birdmap.top

================================================================================
来源：http://usn.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://nyg.zhijiandao.cn

================================================================================
来源：http://bcn.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://hoh.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mxn.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kxu.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dpr.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tka.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ren.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://ncf.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://vxc.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bhe.pycfn.com

[D02] 追加元素到末尾
来源：http://agk.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://avf.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jgf.cqqwz.cn

JS:   arr.push(4);
来源：http://xdk.haohaochexian.top

TS:   arr.push(4);
来源：http://wiw.chenjidiqi.icu


<!-- 参考信息 -->