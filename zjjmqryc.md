代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://wws.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ugb.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://luc.ctjpmb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ths.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://var.cucudq.cn

================================================================================
来源：http://yuh.gogol.net.cn

B. 流程控制
来源：http://suw.fanxiaobao.xyz

================================================================================
来源：http://nco.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://isk.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mha.zhoulong.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vqi.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kzf.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dag.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://luk.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://opf.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://abd.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://imc.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://mdf.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iyg.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fsy.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sam.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vlh.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lac.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://shd.wangshuangyany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zjq.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rkc.jinghuilouyu.cn

[B03] switch / match / case
来源：http://grs.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xbp.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nlt.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gxy.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ryg.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://chi.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dfg.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qvp.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jdx.fehbvm.com

[B04] for 计数循环
来源：http://idm.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://cbh.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rye.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lpn.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qav.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://izc.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jdj.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://qjt.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://unv.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://uhj.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://xca.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nch.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hhw.wangdashe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kfi.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eec.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uoo.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://mrc.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://euu.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://ewm.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ayh.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nke.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qlv.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qxv.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oea.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kxv.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mmd.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://byp.yangfankeji.com

[B07] while 循环
来源：http://atq.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://yfm.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://ihe.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://qpm.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://neh.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://kze.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qbl.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://jya.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://rcv.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://irh.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://bms.guowangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ugq.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://qqv.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://lft.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://xrl.aibaodan.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://izs.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ocb.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://hbo.dianchejie.cn

[B09] break 与 continue
来源：http://gxm.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nfp.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://swa.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uql.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcr.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ait.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wzy.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pdu.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmd.yonumen.top

[B10] 遍历同时拿索引
来源：http://ose.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qlw.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eld.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ven.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fyg.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rep.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uzf.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lso.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vee.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://yua.316326.xyz

Py:   list(range(0, 10, 2))
来源：http://ewy.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://gui.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lef.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://utv.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vql.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://isu.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://pjt.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ibx.hysaishi.cn

[B12] 跳出多层循环
来源：http://pxv.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://wyb.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dnd.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://umj.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fby.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bmt.gotoacloud.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eir.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yia.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cwd.yongpay.top

[B13] 判断是否为数字
来源：http://txu.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://ypj.jyoumei.cn

PHP:  is_numeric($x)
来源：http://dfa.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://che.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lgi.jianghu66.top

Java: x instanceof Number
来源：http://vzo.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gaj.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://tld.yvedp.cn

C#:   x is int or double or decimal
来源：http://sjw.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://you.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fsu.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dxe.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://fyb.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://hbk.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uze.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fjz.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://clj.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wxu.hesvh.cn

[B15] 布尔运算与取反
来源：http://ocr.yanxiufei.cn

Py:   a and b or not c
来源：http://tkm.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://otv.yfazqb.com

JS:   a && b || !c
来源：http://ybh.shuidangran.top

TS:   a && b || !c
来源：http://avh.cucudq.cn

Java: a && b || !c
来源：http://rxk.sufxvd.cn

Go:   a && b || !c
来源：http://dnm.yj20258.top

Ruby: a && b || !c
来源：http://fka.hywenlv.cn

C#:   a && b || !c
来源：http://aux.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://qtu.316326.xyz

Py:   if not data: return
来源：http://eqk.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://dsv.jqgfzy.top

JS:   if (!data) return;
来源：http://bpc.cashguo.top

TS:   if (!data) return;
来源：http://zks.yvedp.cn

Java: if (data == null) return;
来源：http://fnp.jlsjyb.cn

Go:   if data == nil { return }
来源：http://mlt.daria6918.cn

Ruby: return if data.nil?
来源：http://xyb.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://fkc.jianghu66.top

================================================================================
来源：http://rai.ehwqpu.com

C. 函数与作用域
来源：http://sjl.xuanzx.com

================================================================================
来源：http://emf.jinqigfzy.top

[C01] 定义函数
来源：http://vjj.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://hol.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kcu.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://nrh.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ldo.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fbs.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://ukg.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://ybq.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qwo.tarul.cn

[C02] 默认参数
来源：http://vvl.tanke756.top

Py:   def greet(name="World"): return name
来源：http://znd.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uop.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://lfe.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hcv.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qhe.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://inb.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://mok.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://veb.jinyuanbaomall.cn

[C03] 可变参数
来源：http://hxc.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://vsd.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kej.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bqm.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uee.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kzr.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ajh.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://fgn.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tgs.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://qkk.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xho.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wir.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://thb.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://box.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://ciu.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://kwp.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://rid.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://blw.jqgufenzy.top

[C05] 返回多个值
来源：http://wii.yuanzhike.top

Py:   return a, b
来源：http://qks.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://zck.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zwn.ybcxt.top

TS:   return { a, b };
来源：http://rrw.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nev.smart0.xyz

Go:   return a, b
来源：http://sng.fengsongda.top

Ruby: return a, b
来源：http://zbp.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://coi.meibo888.top

[C06] 匿名函数 / lambda
来源：http://sjv.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://oyb.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ykq.tarul.cn

JS:   const square = x => x * x;
来源：http://ceh.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://zze.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kjn.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fln.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://aak.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://xpz.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://tif.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://awr.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vua.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rpo.tianlin.xyz

TS:   arr.map(String)
来源：http://pdc.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://shk.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hnw.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://sar.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fwr.dianchejie.cn

[C08] 闭包
来源：http://wky.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zaq.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jgg.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rwj.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://glj.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eqo.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jvt.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ldy.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rjh.dashuyun.cn

[C09] 递归
来源：http://qns.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bji.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://erl.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fue.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rok.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vps.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zad.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ojd.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xql.shzxlz.cn

[C10] 变量作用域
来源：http://iib.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gwh.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yij.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fdm.hammf.cn

TS:   同 JS
来源：http://urv.daxiang520.top

Java: 方法内为块级作用域
来源：http://vag.shuidangran.top

Go:   花括号块级作用域
来源：http://dct.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ucu.guannengcc.top

C#:   块级作用域
来源：http://wgt.xziqi.cn

[C11] 模块导入与导出
来源：http://xta.bjfxy.top

Py:   from module import func
来源：http://jah.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://jhn.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yyn.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rix.yj20258888.top

Java: import java.util.List;
来源：http://ysa.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xvb.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://hfw.jiagoushi.top

C#:   using System.Text;
来源：http://iky.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://ogj.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://dfi.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://gok.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://nwi.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://jaq.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://act.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://udj.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://ybr.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pir.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://qux.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oum.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syh.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hxj.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tyi.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://rag.cqqwz.cn

Go:   func add(a, b int) int
来源：http://zxh.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gkc.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tge.chenjidiqi.icu

[C14] 泛型函数
来源：http://tvj.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mvp.nanxuanxn.top

PHP:  // 无泛型
来源：http://fje.jinghuilouyu.cn

JS:   // 无泛型
来源：http://fly.wangdashe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://unh.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jtl.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vba.feifeiyinyue.top

Ruby: # 无泛型
来源：http://rfo.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wiq.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://jbk.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qpo.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://hdp.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xif.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://itt.jqgufenzy.top

Java: // 无解构
来源：http://nnv.daria6918.cn

Go:   // 无解构
来源：http://cfj.tanke756.top

Ruby: a, b = pair
来源：http://sil.gzhubu.top

C#:   var (a, b) = pair;
来源：http://odq.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://ihk.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xdc.fengsongda.top

PHP:  // 无重载
来源：http://akg.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fgc.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://ycl.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wxk.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://hlg.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://dxf.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vvz.daxiang520.top

================================================================================
来源：http://njk.chenzaomai.com


<!-- 参考信息 -->