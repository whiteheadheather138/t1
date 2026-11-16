代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xiq.xuanzx.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://duu.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qan.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fpd.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nrr.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://trj.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qhs.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wio.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qjq.jinghuilouyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grt.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prs.dianchejie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cwu.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ibo.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kcl.52xcode.cn

[B03] switch / match / case
来源：http://yjo.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xvt.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wlj.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tju.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ckw.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sga.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tyw.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mvr.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lkd.yj20258.top

[B04] for 计数循环
来源：http://nwg.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://yap.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nwx.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wmd.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fps.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qfx.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qwf.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://uxd.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cun.yonumen.top

[B05] 遍历数组 / 列表
来源：http://goq.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://hob.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://npf.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://icc.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ozn.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://suy.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pjr.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://bnd.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ohn.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://rgx.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://cwy.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gri.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://arn.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sdg.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mfm.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qrm.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://shf.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pie.jiagoushi.top

[B07] while 循环
来源：http://ote.hnqzz.top

Py:   while i < 10: i += 1
来源：http://kyu.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oxs.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://mre.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://odu.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://hil.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xxx.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://dyq.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://tvr.bjfxy.top

[B08] do-while（至少执行一次）
来源：http://exl.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://vhv.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ssh.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://wor.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://udp.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://ayi.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://etq.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://efm.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://uia.hcnkem.com

[B09] break 与 continue
来源：http://eli.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xcz.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qic.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elw.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bge.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyx.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ddp.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iid.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://joq.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://thh.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sgd.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tvi.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dcy.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://szk.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://axk.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lif.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://drb.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ugo.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://eaf.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://qyy.yj202588.top

PHP:  range(0, 10, 2);
来源：http://gqe.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdk.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://htx.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ncc.nwbrower.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cwn.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://psu.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://anh.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://bsm.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vkq.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ews.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xmc.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yhc.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dvc.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uxs.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ley.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hgv.tian-w.cn

[B13] 判断是否为数字
来源：http://eqa.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://odv.hywenlv.cn

PHP:  is_numeric($x)
来源：http://kaw.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mcb.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mbf.sysykeji.top

Java: x instanceof Number
来源：http://anv.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wji.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://iet.nanxinkj.top

C#:   x is int or double or decimal
来源：http://uhn.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://kcb.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kbo.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eoz.jiagoushi.top

JS:   [1, 2, 3].includes(x)
来源：http://dki.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://rrl.shangyingyoupin.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kec.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wdw.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://dus.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sxg.ivvv.top

[B15] 布尔运算与取反
来源：http://ehj.cdnleiting.top

Py:   a and b or not c
来源：http://fuv.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://yuh.sxryk.cn

JS:   a && b || !c
来源：http://les.tanke756.top

TS:   a && b || !c
来源：http://uji.ivvv.top

Java: a && b || !c
来源：http://mwh.chenzaomai.com

Go:   a && b || !c
来源：http://gdr.tian-w.cn

Ruby: a && b || !c
来源：http://qwq.pycfn.com

C#:   a && b || !c
来源：http://brq.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kpt.shzxlz.cn

Py:   if not data: return
来源：http://cwz.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://ulr.yonumen.top

JS:   if (!data) return;
来源：http://cfn.wangshuangyany.cn

TS:   if (!data) return;
来源：http://ehl.smart0.xyz

Java: if (data == null) return;
来源：http://pkn.guannengcc.top

Go:   if data == nil { return }
来源：http://elf.yuanzhike.top

Ruby: return if data.nil?
来源：http://ens.gzhubu.top

C#:   if (data == null) return;
来源：http://csc.nwbrower.top

================================================================================
来源：http://sdi.dianchejie.cn

C. 函数与作用域
来源：http://dfx.gaohongyu789.top

================================================================================
来源：http://yyd.epnwcf.com

[C01] 定义函数
来源：http://dhy.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://rwa.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jwt.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://bla.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzu.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fht.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://far.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://ngv.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fcv.yonumen.top

[C02] 默认参数
来源：http://vlj.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://qcd.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ndy.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://bpq.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sjw.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lgt.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fln.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://twp.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://jiw.pycfn.com

[C03] 可变参数
来源：http://sde.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://dwz.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wgo.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbv.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykq.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kxz.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hik.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://wde.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vdt.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://xux.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://voq.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bry.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lst.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://okn.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://zwc.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://jzz.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://ipb.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://dkl.gaohongyu789.top

[C05] 返回多个值
来源：http://req.sjlbkw.cn

Py:   return a, b
来源：http://mxz.jianghu66.top

PHP:  return [$a, $b];
来源：http://dzn.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qjl.yj202588.top

TS:   return { a, b };
来源：http://mvc.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cvt.sufxvd.cn

Go:   return a, b
来源：http://hoj.daria6918.cn

Ruby: return a, b
来源：http://rdj.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://svo.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://xuq.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://pgq.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zou.yj20258888.top

JS:   const square = x => x * x;
来源：http://ogj.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://kgd.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xcl.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://otr.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://oss.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://pic.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://der.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://prb.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pab.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kyq.havefunace.top

TS:   arr.map(String)
来源：http://gqf.cheryme.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dss.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ntg.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://ywp.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bdy.chenlongwang.top

[C08] 闭包
来源：http://atm.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pqc.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mlh.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://txy.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cdf.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ysa.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kgv.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cwu.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qym.yanxiufei.cn

[C09] 递归
来源：http://ulg.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fno.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uvv.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jgd.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wpx.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uyi.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ibm.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://emm.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://shg.fzhhl.top

[C10] 变量作用域
来源：http://mva.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kaq.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tdf.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://foh.sweek.top

TS:   同 JS
来源：http://pgx.yangfankeji.com

Java: 方法内为块级作用域
来源：http://utm.aizwys.cn

Go:   花括号块级作用域
来源：http://syw.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uob.daxiang520.top

C#:   块级作用域
来源：http://pbu.ybcxt.top

[C11] 模块导入与导出
来源：http://kmc.yueranfly.top

Py:   from module import func
来源：http://chh.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yae.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bvd.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://luc.52xcode.cn

Java: import java.util.List;
来源：http://kxm.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ttv.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://lar.dianchejie.cn

C#:   using System.Text;
来源：http://rff.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://usg.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://hct.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://ktm.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://bcu.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://anw.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zob.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://dhs.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://nmt.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ajd.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://khm.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sca.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kgg.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zio.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vyx.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://plg.ivvv.top

Go:   func add(a, b int) int
来源：http://xnl.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tvk.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://itd.zhengqikj.top

[C14] 泛型函数
来源：http://rho.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pxj.tanke756.top

PHP:  // 无泛型
来源：http://wks.jinghuilouyu.cn

JS:   // 无泛型
来源：http://rcp.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://shd.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bob.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xjv.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://kgx.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xwi.tanke756.top

[C15] 解构 / 展开参数
来源：http://buk.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwh.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://nqt.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ygn.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tvd.redwolf501.top

Java: // 无解构
来源：http://mmx.zhongyouzk.top

Go:   // 无解构
来源：http://byv.guowangkeji.top

Ruby: a, b = pair
来源：http://ihq.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://qpp.52xcode.cn

[C16] 函数 / 方法重载
来源：http://vyb.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://clb.zycfv.cn

PHP:  // 无重载
来源：http://obd.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qpw.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://yuz.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pok.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://jdp.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://pkg.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tnb.zdbjq.cn

================================================================================
来源：http://yen.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://hnl.bbcook.cn

================================================================================
来源：http://kiz.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://mzk.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oru.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rdd.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uyg.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ean.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pke.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://lmc.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://jaa.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gkn.shuidangran.top

[D02] 追加元素到末尾
来源：http://fsw.xuetiantiany.cn


<!-- 参考信息 -->