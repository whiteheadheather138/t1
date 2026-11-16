代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bww.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://buq.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mao.zhoulong.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jtu.aizwys.cn

[A26] 类型转换总览
来源：http://zoo.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fus.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gnh.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kov.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://ywe.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zdt.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://als.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ixn.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tcd.wangshuangyany.cn

================================================================================
来源：http://inv.ppjwa.cn

B. 流程控制
来源：http://keu.redwolf501.top

================================================================================
来源：http://fyo.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://qlc.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hmq.tian-w.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dss.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ieu.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ngq.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ntf.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ysf.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jqu.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hsp.52xcode.cn

[B02] 多分支 else if / elif
来源：http://blq.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ypg.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kzz.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sbv.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hgr.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fym.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iag.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mto.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osh.jyoumei.cn

[B03] switch / match / case
来源：http://lyg.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wbr.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://moi.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pwo.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gck.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hbe.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lgk.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wfl.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wnc.jinqigufen.top

[B04] for 计数循环
来源：http://cfj.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://cki.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gle.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://equ.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izs.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fqn.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oqj.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://tdk.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uzn.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://voh.andypj.xyz

Py:   for item in arr: print(item)
来源：http://iul.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hqo.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mpc.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wuu.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lzb.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zel.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://iam.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cim.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://pvp.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gsg.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dgo.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tzg.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xzl.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jyw.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://knu.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://axy.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xje.fehbvm.com

[B07] while 循环
来源：http://hze.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://eqr.kuanghao11.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lfi.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://ass.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://bex.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://avc.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qxh.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://mfj.sweek.top

C#:   while (i < 10) { i++; }
来源：http://xjz.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://ebs.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://lqb.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rrn.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://wyr.chenjidiqi.icu

TS:   do { i++; } while (i < 10);
来源：http://tuw.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://mhe.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://elt.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://odn.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://cux.jyoumei.cn

[B09] break 与 continue
来源：http://ptb.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://izu.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rnw.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umb.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kia.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwc.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gep.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zrq.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpr.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://eqv.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wio.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mpe.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hkh.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oxn.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gbb.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zwh.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rtp.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://evu.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://ayb.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://egm.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://aao.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vpo.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xex.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gmr.birdmap.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mwg.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://jlz.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zgv.andypj.xyz

[B12] 跳出多层循环
来源：http://pzc.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://lkh.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jog.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zlb.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hku.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ccb.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yee.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tea.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tmk.0kj1m.cn

[B13] 判断是否为数字
来源：http://ngg.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://ggk.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://ovx.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yvj.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zei.tian-w.cn

Java: x instanceof Number
来源：http://ufr.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eom.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://ewi.bjfxy.top

C#:   x is int or double or decimal
来源：http://xgi.yvedp.cn

[B14] 判断值是否在集合内
来源：http://yde.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rlm.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://whe.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://qjn.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://xfo.yfazqb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ano.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://est.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://cgu.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gtt.chenlongwang.top

[B15] 布尔运算与取反
来源：http://eoj.jyoumei.cn

Py:   a and b or not c
来源：http://qno.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://fjz.sweek.top

JS:   a && b || !c
来源：http://kug.nanxinkj.top

TS:   a && b || !c
来源：http://lnm.hnqzz.top

Java: a && b || !c
来源：http://cmt.ctjpmb.com

Go:   a && b || !c
来源：http://kbr.ppjwa.cn

Ruby: a && b || !c
来源：http://idf.chenzaomai.com

C#:   a && b || !c
来源：http://mcw.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rya.wangshuangyany.cn

Py:   if not data: return
来源：http://qkq.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://ets.hfpthk.cn

JS:   if (!data) return;
来源：http://xhg.zycfv.cn

TS:   if (!data) return;
来源：http://wqn.aibaodan.cn

Java: if (data == null) return;
来源：http://jch.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://jbo.shzxlz.cn

Ruby: return if data.nil?
来源：http://nhl.aizwys.cn

C#:   if (data == null) return;
来源：http://lgy.jinyuanbaomall.cn

================================================================================
来源：http://zzt.xylfe.cn

C. 函数与作用域
来源：http://vcd.yuanzhike.top

================================================================================
来源：http://rjl.ctjpmb.com

[C01] 定义函数
来源：http://kdi.yonumen.top

Py:   def add(a, b): return a + b
来源：http://wwr.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xkt.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://sgb.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wka.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xms.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gcd.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://tvb.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://brx.smart0.xyz

[C02] 默认参数
来源：http://aef.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://yah.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jqp.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://ptx.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rwv.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://jfx.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gvb.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://laz.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://buq.ivvv.top

[C03] 可变参数
来源：http://nnl.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://lix.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://phn.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sbh.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkm.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kbb.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qbt.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://uua.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nyx.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://osr.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ldt.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gii.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://udy.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rlr.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://znu.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://hft.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://pgl.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://xuz.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://fvi.zhiwuduotai.top

Py:   return a, b
来源：http://igx.andypj.xyz

PHP:  return [$a, $b];
来源：http://rhw.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://gum.haohaochexian.top

TS:   return { a, b };
来源：http://wot.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sul.52xcode.cn

Go:   return a, b
来源：http://zwj.guannengcc.top

Ruby: return a, b
来源：http://uut.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://cax.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://wel.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://nlj.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rpi.svipenyu.cn

JS:   const square = x => x * x;
来源：http://wij.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://sso.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bhg.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://fjt.andypj.xyz

Ruby: square = ->(x) { x * x }
来源：http://vku.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://rmg.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://pos.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hun.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://mxe.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://slp.jinqigufen.top

TS:   arr.map(String)
来源：http://eko.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gjn.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xdw.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://uqi.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jbt.xuanzx.com

[C08] 闭包
来源：http://tgo.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sri.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yxl.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fvc.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jgt.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nff.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://une.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ple.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iuc.aizwys.cn

[C09] 递归
来源：http://fbv.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tml.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cra.pengpengdd.cyou

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hjz.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ftq.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gix.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hwz.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://slj.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ikr.xinyue.icu

[C10] 变量作用域
来源：http://tni.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ywt.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oka.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://end.jinghuilouyu.cn

TS:   同 JS
来源：http://ghy.haohaochexian.top

Java: 方法内为块级作用域
来源：http://ynj.xinyue.icu

Go:   花括号块级作用域
来源：http://nrx.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fgc.fengsongda.top

C#:   块级作用域
来源：http://bfc.jinqigfzy.top

[C11] 模块导入与导出
来源：http://rmf.ehwqpu.com

Py:   from module import func
来源：http://tbd.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tjc.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://gyd.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cjo.yangfankeji.com

Java: import java.util.List;
来源：http://uzw.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vaw.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://qzi.xziqi.cn

C#:   using System.Text;
来源：http://grp.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://qsk.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://qzb.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://wxe.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://fuv.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://wiu.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://scv.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://hhu.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://qzg.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nsr.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://nnj.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ypp.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://soi.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ifp.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://elf.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://khi.dashuyun.cn

Go:   func add(a, b int) int
来源：http://gll.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tsp.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://nle.vqdsnc.cn

[C14] 泛型函数
来源：http://heb.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://osi.chenjidiqi.icu

PHP:  // 无泛型
来源：http://dmt.aizwys.cn

JS:   // 无泛型
来源：http://udo.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vio.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xtk.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tjw.guannengcc.top

Ruby: # 无泛型
来源：http://emo.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vrz.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://xud.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ndo.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://hmt.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ujn.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qtg.tianlin.xyz

Java: // 无解构
来源：http://fit.sjlbkw.cn

Go:   // 无解构
来源：http://rxz.ivvv.top

Ruby: a, b = pair
来源：http://qdg.shuidangran.top

C#:   var (a, b) = pair;
来源：http://tgf.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://qzi.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zgp.zdqjudy.top


<!-- 参考信息 -->