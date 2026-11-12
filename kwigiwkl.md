代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://rlu.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jjo.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qyd.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wak.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://axb.ivvv.top

================================================================================
来源：http://qir.yj202588.top

B. 流程控制
来源：http://eda.yj20258888.top

================================================================================
来源：http://evb.cqqwz.cn

[B01] 条件判断 if / else
来源：http://ecw.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://lwa.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vyy.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hus.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vrc.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://emd.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nns.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zjc.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zqm.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://juj.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kyt.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://edg.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ted.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dzu.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oml.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dvp.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tlr.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgq.zhixingplan.top

[B03] switch / match / case
来源：http://qzz.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nxl.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mwc.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kix.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vwq.xingfuxueyuan.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://izx.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eog.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cki.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ouk.hysaishi.cn

[B04] for 计数循环
来源：http://lrn.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://qdj.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iee.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uuu.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uop.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cva.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://upe.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://zat.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://our.uphjek.com

[B05] 遍历数组 / 列表
来源：http://jyg.yj202588.top

Py:   for item in arr: print(item)
来源：http://afn.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gob.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xvk.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://muf.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dnr.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://abi.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://ljp.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xpx.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://emv.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iyl.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yuv.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iwp.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvk.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qpb.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://utq.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iss.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ark.ywan-chungtsiang.top

[B07] while 循环
来源：http://juz.cheryme.top

Py:   while i < 10: i += 1
来源：http://vsy.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://xiv.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://bds.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://afp.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://ger.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ifx.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://jij.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://bsx.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://wyf.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://slr.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cej.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://jgd.zhiwuduotai.top

TS:   do { i++; } while (i < 10);
来源：http://dpz.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://tyd.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fhx.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://qcl.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://glh.nanxinkj.top

[B09] break 与 continue
来源：http://ilk.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fsg.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ncy.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mdj.zdbjq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhn.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pgn.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ijn.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qgc.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgx.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://elf.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vnj.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mqv.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lgn.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mwm.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fxo.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pof.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cet.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vin.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://cgn.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://eck.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://vgo.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fcx.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nyn.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://drk.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ymk.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://jyi.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://epi.hfpthk.cn

[B12] 跳出多层循环
来源：http://mlv.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dat.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://kqz.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hug.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vfe.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://scp.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vit.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://puj.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fwh.yj202588.top

[B13] 判断是否为数字
来源：http://aqy.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://nni.nanxinkj.top

PHP:  is_numeric($x)
来源：http://vwq.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yme.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vcw.kuanghao11.cn

Java: x instanceof Number
来源：http://kda.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wpv.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://kva.wangdashe.top

C#:   x is int or double or decimal
来源：http://sdk.bjfxy.top

[B14] 判断值是否在集合内
来源：http://pgr.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jub.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://czr.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://fxo.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://gkh.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://pdw.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rmg.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rrb.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tks.yonumen.top

[B15] 布尔运算与取反
来源：http://asw.dashuyun.cn

Py:   a and b or not c
来源：http://jvj.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://ilf.cqqwz.cn

JS:   a && b || !c
来源：http://arg.meibo888.top

TS:   a && b || !c
来源：http://qvf.gogol.net.cn

Java: a && b || !c
来源：http://bgp.yj20258.top

Go:   a && b || !c
来源：http://dfl.9152youxi.cn

Ruby: a && b || !c
来源：http://qef.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://wre.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://rlc.haohaochexian.top

Py:   if not data: return
来源：http://zef.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://gdk.aibaodan.cn

JS:   if (!data) return;
来源：http://rck.vqdsnc.cn

TS:   if (!data) return;
来源：http://nvy.kuanghao11.cn

Java: if (data == null) return;
来源：http://ydy.ctjpmb.com

Go:   if data == nil { return }
来源：http://mqo.pycfn.com

Ruby: return if data.nil?
来源：http://yhx.redwolf501.top

C#:   if (data == null) return;
来源：http://naq.yj202588.top

================================================================================
来源：http://jvd.jinyuanbaomall.cn

C. 函数与作用域
来源：http://moq.yongpay.top

================================================================================
来源：http://yac.guowangkeji.top

[C01] 定义函数
来源：http://bvv.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://sla.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wyh.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://ulg.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zie.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nnq.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kam.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://xvq.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://myv.jianghu66.top

[C02] 默认参数
来源：http://fhc.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://dbe.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vgt.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://efb.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gxx.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qwv.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fdf.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://hmd.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://fyk.ydjk.org.cn

[C03] 可变参数
来源：http://rfl.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://sgm.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hdo.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mth.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wwo.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wvk.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bks.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://yoj.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://emb.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://whe.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hda.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rlo.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vtz.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ygb.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://ord.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://zyz.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://gla.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://rtt.yanxiufei.cn

[C05] 返回多个值
来源：http://tna.gzhubu.top

Py:   return a, b
来源：http://wxn.zycfv.cn

PHP:  return [$a, $b];
来源：http://ine.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tiq.yj20258.top

TS:   return { a, b };
来源：http://haz.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://flh.zdqjudy.top

Go:   return a, b
来源：http://zcd.fengsongda.top

Ruby: return a, b
来源：http://low.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://bzg.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://tmd.xinyue.icu

Py:   square = lambda x: x * x
来源：http://yph.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zuy.iojbl.cn

JS:   const square = x => x * x;
来源：http://txg.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://pen.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gpn.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://iin.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://pzu.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://acf.daxiang520.top

[C07] 把函数作为参数传入
来源：http://fbj.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gms.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uwz.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zso.xuetiantiany.cn

TS:   arr.map(String)
来源：http://lcj.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tig.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xtn.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://yhs.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kzr.aizwys.cn

[C08] 闭包
来源：http://qkv.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://etf.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dft.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://anc.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yzb.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dam.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ktg.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vwv.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uef.ywan-chungtsiang.top

[C09] 递归
来源：http://jbo.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmp.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vef.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fcu.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vxa.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iwg.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gim.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ijq.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://abg.9152youxi.cn

[C10] 变量作用域
来源：http://nna.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rby.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fmf.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jwk.chenlongwang.top

TS:   同 JS
来源：http://oif.gzhubu.top

Java: 方法内为块级作用域
来源：http://awr.sysykeji.top

Go:   花括号块级作用域
来源：http://jqy.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rag.epnwcf.com

C#:   块级作用域
来源：http://utk.havefunace.top

[C11] 模块导入与导出
来源：http://vrj.9152youxi.cn

Py:   from module import func
来源：http://syv.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fuz.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ozl.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://unc.52xcode.cn

Java: import java.util.List;
来源：http://jmz.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mvq.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://xfq.yonumen.top

C#:   using System.Text;
来源：http://ahc.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://pof.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://bnx.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://omw.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://vyw.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://vvk.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eyy.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://ouw.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://uoa.xylfe.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mir.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://dfd.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bmt.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://txe.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nkj.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukj.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fkx.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://kye.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://owu.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://lpg.yfazqb.com

[C14] 泛型函数
来源：http://spq.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://puz.zhiwuduotai.top

PHP:  // 无泛型
来源：http://cfc.hnxiangtu.top

JS:   // 无泛型
来源：http://bwd.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ckd.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://our.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gxq.uphjek.com

Ruby: # 无泛型
来源：http://haz.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ltj.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://ems.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mdg.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://jtw.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://laj.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hzm.sysykeji.top

Java: // 无解构
来源：http://vuw.cashguo.top

Go:   // 无解构
来源：http://alr.316326.xyz

Ruby: a, b = pair
来源：http://ryr.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://pir.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://nci.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qlp.shuidangran.top

PHP:  // 无重载
来源：http://bjg.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wml.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://vpp.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nto.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://zua.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://plq.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qxy.9152youxi.cn

================================================================================
来源：http://gva.dianchejie.cn


<!-- 参考信息 -->