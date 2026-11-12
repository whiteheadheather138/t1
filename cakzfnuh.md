代发 wailian999

[B01] 条件判断 if / else
来源：http://cww.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mbe.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qzx.guowangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ves.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lbg.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://umu.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nxw.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wpb.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vhv.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://huv.yonumen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wal.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oix.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yjo.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://otk.zhixingplan.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxa.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xuc.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ent.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fiq.yj20258888.top

[B03] switch / match / case
来源：http://ywu.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vbg.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://amg.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ahs.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jqc.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rpl.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jil.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xrk.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jnv.gaohongyu789.top

[B04] for 计数循环
来源：http://fnm.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://zna.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gch.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://duo.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jxw.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dke.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lyo.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://eik.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://slm.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://mao.tian-w.cn

Py:   for item in arr: print(item)
来源：http://vkh.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hum.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tno.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xgg.dashuyun.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oie.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rju.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://hio.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oos.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://vfh.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://izn.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rlc.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tmf.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tmj.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uxj.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tdz.0kj1m.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jpr.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hms.jianghu66.top

[B07] while 循环
来源：http://rir.aizwys.cn

Py:   while i < 10: i += 1
来源：http://snu.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cjg.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://uih.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://svc.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://njx.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lbo.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://vjm.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://bpm.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://vxs.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://tlg.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ahr.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://mno.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://nyy.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://onl.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ouu.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ykc.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://iel.uphjek.com

[B09] break 与 continue
来源：http://zaf.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://epe.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dwn.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ljm.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryi.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jib.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lcj.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lxs.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thr.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://ans.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ysl.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ygl.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lrg.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nav.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hbl.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mpw.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jay.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rdl.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://zzf.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://imb.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://xcx.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ywu.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sud.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hem.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yve.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://jlt.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sxi.ehwqpu.com

[B12] 跳出多层循环
来源：http://feu.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sti.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://edn.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vvh.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kwo.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ziv.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vix.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vpi.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://itv.gotoacloud.top

[B13] 判断是否为数字
来源：http://abx.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://rvx.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://xxc.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqc.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jhy.andypj.xyz

Java: x instanceof Number
来源：http://qgx.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wxv.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://geq.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://zvd.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://uva.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tcd.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://enq.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://tix.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://ejn.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://slj.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wqp.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://bte.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bjw.zdbjq.cn

[B15] 布尔运算与取反
来源：http://nob.andypj.xyz

Py:   a and b or not c
来源：http://itv.hesvh.cn

PHP:  $a && $b || !$c
来源：http://jje.hnxiangtu.top

JS:   a && b || !c
来源：http://ujy.dianchejie.cn

TS:   a && b || !c
来源：http://xap.52xcode.cn

Java: a && b || !c
来源：http://jqn.chenzaomai.com

Go:   a && b || !c
来源：http://erw.jlsjyb.cn

Ruby: a && b || !c
来源：http://lql.316326.xyz

C#:   a && b || !c
来源：http://fqd.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rod.ehwqpu.com

Py:   if not data: return
来源：http://zsu.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://dzm.yj20258.top

JS:   if (!data) return;
来源：http://weh.gogol.net.cn

TS:   if (!data) return;
来源：http://npg.zhoulong.xyz

Java: if (data == null) return;
来源：http://wpf.shuidangran.top

Go:   if data == nil { return }
来源：http://zrd.jyoumei.cn

Ruby: return if data.nil?
来源：http://ufu.zhixingplan.top

C#:   if (data == null) return;
来源：http://rgg.hfpthk.cn

================================================================================
来源：http://bqr.pengpengdd.cyou

C. 函数与作用域
来源：http://eiu.svipenyu.cn

================================================================================
来源：http://nnt.shzxlz.cn

[C01] 定义函数
来源：http://epb.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://kxm.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hqj.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://jlg.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gym.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cne.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rkn.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://oxo.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eig.zhijiandao.cn

[C02] 默认参数
来源：http://rnm.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://yxd.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nlk.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://ccj.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://aol.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cmy.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uez.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://prr.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://hcc.sweek.top

[C03] 可变参数
来源：http://kdw.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://qtd.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://noh.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ebn.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmj.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mre.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yyh.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://vdz.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lxb.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://qfd.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nkb.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://goe.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bpc.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kwt.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://krk.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://sqa.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://ymt.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://agh.mhx1999.top

[C05] 返回多个值
来源：http://xmo.fzhhl.top

Py:   return a, b
来源：http://xdd.hfpthk.cn

PHP:  return [$a, $b];
来源：http://uqi.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fgy.jinghuilouyu.cn

TS:   return { a, b };
来源：http://lcr.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kvj.cashguo.top

Go:   return a, b
来源：http://epa.cucudq.cn

Ruby: return a, b
来源：http://ouc.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://gxa.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://rpe.yongpay.top

Py:   square = lambda x: x * x
来源：http://ubs.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://joy.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://lac.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://kle.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eyh.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xqa.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://ner.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://abf.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://jqa.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ziv.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://ngl.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pbl.tanke756.top

TS:   arr.map(String)
来源：http://kat.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://frj.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vdt.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://whs.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://plf.bbcook.cn

[C08] 闭包
来源：http://ngp.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qmb.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lrr.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cbg.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qgw.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ybo.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://scc.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://icq.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zcc.chenjidiqi.icu

[C09] 递归
来源：http://iqi.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ppu.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fob.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qlr.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://usi.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dzz.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aun.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bjp.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pwq.xziqi.cn

[C10] 变量作用域
来源：http://ypz.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rqy.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ysf.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://crk.tarul.cn

TS:   同 JS
来源：http://wzg.tanke756.top

Java: 方法内为块级作用域
来源：http://vbc.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://djm.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uhw.xinyue.icu

C#:   块级作用域
来源：http://yey.jinqigfzy.top

[C11] 模块导入与导出
来源：http://cdd.9152youxi.cn

Py:   from module import func
来源：http://oek.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zeh.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jvm.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zni.haohaochexian.top

Java: import java.util.List;
来源：http://jyw.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wlj.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://jcr.fzhhl.top

C#:   using System.Text;
来源：http://wvp.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://afp.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://she.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://syp.zhongyouzk.top

JS:   (() => { console.log("run"); })();
来源：http://rfh.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://ija.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zfs.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://jcg.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://sda.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hnf.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://hxs.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rnm.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iuk.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oth.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bke.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://tcx.fzhhl.top

Go:   func add(a, b int) int
来源：http://ddm.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xwc.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://toj.jinghuilouyu.cn

[C14] 泛型函数
来源：http://igv.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://czs.tarul.cn

PHP:  // 无泛型
来源：http://wro.fzhhl.top

JS:   // 无泛型
来源：http://usl.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ytc.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eeh.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://imy.9152youxi.cn

Ruby: # 无泛型
来源：http://fvx.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ouo.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://xob.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ktv.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://pnu.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tuf.hnqzz.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jcz.quarkkingdee.top

Java: // 无解构
来源：http://yrx.316326.xyz

Go:   // 无解构
来源：http://seq.shangyingyoupin.top

Ruby: a, b = pair
来源：http://tlg.tanke756.top

C#:   var (a, b) = pair;
来源：http://mct.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://ksb.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wib.wangdashe.top

PHP:  // 无重载
来源：http://skd.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nao.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://gvy.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://koz.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://ssl.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://eme.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vxa.vehdjk.com

================================================================================
来源：http://iru.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://ida.meibo888.top

================================================================================
来源：http://vnz.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://rxc.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ugw.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bja.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zoa.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fxt.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wua.ivvv.top


<!-- 参考信息 -->