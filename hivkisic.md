代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fxk.jinghuilouyu.cn

================================================================================
来源：http://fvc.tanke756.top

B. 流程控制
来源：http://sus.daxiang520.top

================================================================================
来源：http://znk.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://nzy.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ukn.xylfe.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sfa.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rmm.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kak.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pxe.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ame.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tzt.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zzt.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://zki.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://stc.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bvl.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wsw.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hhl.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydo.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ubx.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ihe.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://atz.yangfankeji.com

[B03] switch / match / case
来源：http://bhk.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dhl.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tog.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wvs.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hyj.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gyl.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mno.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fpk.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xjl.redwolf501.top

[B04] for 计数循环
来源：http://xsg.sweek.top

Py:   for i in range(10): print(i)
来源：http://nni.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xvv.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mfa.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eqt.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dmn.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dod.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://rpw.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qaj.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://ndz.c1oappe.top

Py:   for item in arr: print(item)
来源：http://kzj.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rmu.c1oappe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iwu.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://aam.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tmv.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vcw.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://ijo.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iwy.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://dsr.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ohn.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ntc.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vpq.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tmg.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://udu.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bca.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jrw.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ugs.xziqi.cn

[B07] while 循环
来源：http://swf.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://maf.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://huo.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://euo.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://flj.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://agy.ivvv.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zjd.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://jqo.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://vhy.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://fzf.zhijiandao.cn

Py:   # 无 do-while：用 while True + break
来源：http://gqd.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ggp.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://dgo.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://sdt.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://rat.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jhs.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://djs.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://jzh.feifeiyinyue.top

[B09] break 与 continue
来源：http://yrd.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://arb.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iok.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyx.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujz.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://saw.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dop.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yrg.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obl.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://haj.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vkz.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eba.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://moq.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ziu.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dnd.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cye.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kdf.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wzh.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://wuf.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://bfg.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://lrb.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ojp.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://phr.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zjf.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sse.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://zmq.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lmm.zdbjq.cn

[B12] 跳出多层循环
来源：http://rja.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://feh.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fxo.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ovk.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgt.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pet.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tdm.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejj.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aoh.uphjek.com

[B13] 判断是否为数字
来源：http://eqw.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://xes.xinyue.icu

PHP:  is_numeric($x)
来源：http://say.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://btx.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://utz.nwbrower.top

Java: x instanceof Number
来源：http://vmd.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dwy.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://oqp.shuidangran.top

C#:   x is int or double or decimal
来源：http://sbf.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://uvo.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vlz.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sjb.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://mgu.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://vxh.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://npy.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mkq.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://sgk.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cnh.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://syh.yueranfly.top

Py:   a and b or not c
来源：http://bbm.wangdashe.top

PHP:  $a && $b || !$c
来源：http://ass.hnqzz.top

JS:   a && b || !c
来源：http://tcv.pengpengdd.cyou

TS:   a && b || !c
来源：http://mvi.snrcjt.cn

Java: a && b || !c
来源：http://hjq.hnxiangtu.top

Go:   a && b || !c
来源：http://gsz.xinyue.icu

Ruby: a && b || !c
来源：http://ksg.sysykeji.top

C#:   a && b || !c
来源：http://iay.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://jhf.sufxvd.cn

Py:   if not data: return
来源：http://xml.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://yzm.jinqigufen.top

JS:   if (!data) return;
来源：http://fmi.xinyue.icu

TS:   if (!data) return;
来源：http://rom.yj20258888.top

Java: if (data == null) return;
来源：http://hae.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://gsb.hnqzz.top

Ruby: return if data.nil?
来源：http://fxf.aibaodan.cn

C#:   if (data == null) return;
来源：http://vhi.sysykeji.top

================================================================================
来源：http://uof.zhaomingkeji.xyz

C. 函数与作用域
来源：http://nnz.meibo888.top

================================================================================
来源：http://asi.hfpthk.cn

[C01] 定义函数
来源：http://ovd.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://dyh.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzj.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://flh.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jmi.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ovh.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://lij.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://avj.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://azg.guannengcc.top

[C02] 默认参数
来源：http://bvn.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://nwt.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://vrr.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://vjz.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tfe.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sae.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vtp.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://wtw.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://oby.0kj1m.cn

[C03] 可变参数
来源：http://qsc.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://apr.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://spl.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aju.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dlh.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fqf.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://owz.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://tpb.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rks.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://qff.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://seo.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cox.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ffu.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://red.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://yjx.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://cww.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://mui.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://cvl.xinyue.icu

[C05] 返回多个值
来源：http://zjr.daria6918.cn

Py:   return a, b
来源：http://wfk.havefunace.top

PHP:  return [$a, $b];
来源：http://ghj.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fph.shzxlz.cn

TS:   return { a, b };
来源：http://trx.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kno.hysaishi.cn

Go:   return a, b
来源：http://mgp.zhengqikj.top

Ruby: return a, b
来源：http://lqc.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://dek.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://ysb.c1oappe.top

Py:   square = lambda x: x * x
来源：http://feb.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kws.birdmap.top

JS:   const square = x => x * x;
来源：http://jgj.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://qqd.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ckl.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://nir.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://uow.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://iua.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://jmd.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cpx.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://nnf.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fqh.hfpthk.cn

TS:   arr.map(String)
来源：http://eob.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xnh.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ors.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://yev.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cck.ywan-chungtsiang.top

[C08] 闭包
来源：http://oum.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bwt.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tjk.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://phf.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dpl.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://isf.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ynn.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hva.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yvo.fengsongda.top

[C09] 递归
来源：http://qcn.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://emr.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rjz.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vti.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cnd.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://udt.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://idt.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fvd.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aqd.haohaochexian.top

[C10] 变量作用域
来源：http://icm.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gla.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qkk.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oga.nwbrower.top

TS:   同 JS
来源：http://adv.yj20258888.top

Java: 方法内为块级作用域
来源：http://omt.cheryme.top

Go:   花括号块级作用域
来源：http://owa.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vml.vqdsnc.cn

C#:   块级作用域
来源：http://lnn.yfazqb.com

[C11] 模块导入与导出
来源：http://pho.pycfn.com

Py:   from module import func
来源：http://epc.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zdq.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gpf.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fbs.zhiwuduotai.top

Java: import java.util.List;
来源：http://hrs.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tib.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://rkx.tian-w.cn

C#:   using System.Text;
来源：http://fgd.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://ixe.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://bom.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://gas.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://xmu.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://rpa.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dio.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://lec.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://laz.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lhg.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://lkk.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvq.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nht.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://akb.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzr.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://wcb.guowangkeji.top

Go:   func add(a, b int) int
来源：http://bjs.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jdz.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://zlh.dianchejie.cn

[C14] 泛型函数
来源：http://nhb.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rsf.hysaishi.cn

PHP:  // 无泛型
来源：http://weg.zhiwuduotai.top

JS:   // 无泛型
来源：http://whu.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ift.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://enk.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mwk.sweek.top

Ruby: # 无泛型
来源：http://nxy.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rlr.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://lbb.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uxr.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://iic.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ayc.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mbu.gotoacloud.top

Java: // 无解构
来源：http://lvl.zdqjudy.top

Go:   // 无解构
来源：http://xow.gotoacloud.top

Ruby: a, b = pair
来源：http://pja.zycfv.cn

C#:   var (a, b) = pair;
来源：http://wiy.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://jds.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hqs.sweek.top

PHP:  // 无重载
来源：http://dqi.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fsw.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://plg.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lrl.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://glb.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://sla.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ini.jlsjyb.cn

================================================================================
来源：http://nxn.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://luh.jinqigfzy.top

================================================================================
来源：http://tud.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://ymb.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rke.iojbl.cn


<!-- 参考信息 -->