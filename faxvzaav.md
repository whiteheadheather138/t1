代发 wailian999

[A26] 类型转换总览
来源：http://qfz.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ygn.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://adi.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hbw.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://syw.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pkm.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dwx.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dlw.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ytj.havefunace.top

================================================================================
来源：http://tum.sysykeji.top

B. 流程控制
来源：http://gjc.fehbvm.com

================================================================================
来源：http://xgv.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://ssd.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://utw.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://chx.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://shy.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://awv.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://eqw.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xge.hfpthk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yuz.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rvn.tian-w.cn

[B02] 多分支 else if / elif
来源：http://fvn.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pdv.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fdf.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyq.yonumen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://clh.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://czb.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bzq.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://poq.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wet.zhengqikj.top

[B03] switch / match / case
来源：http://ydb.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zoh.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://etu.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cvg.andypj.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rtv.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lpe.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dyv.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pak.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jjr.hcnkem.com

[B04] for 计数循环
来源：http://ltd.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://pye.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zqi.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qow.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxd.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kss.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ivc.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://mtd.yvedp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ejz.cashguo.top

[B05] 遍历数组 / 列表
来源：http://ncx.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://kww.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ilb.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://lya.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://aus.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://srh.jqgfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hak.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://zff.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zie.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://tzl.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jxt.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xch.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fai.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zcq.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aez.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://psu.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://moy.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qyc.zdqjudy.top

[B07] while 循环
来源：http://mnk.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://jkf.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://ozw.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://jjy.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://zid.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://frq.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://idq.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://qmo.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://yjd.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://gvx.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://iai.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jno.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://yuc.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://zqk.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://inj.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://rhl.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mbz.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://uhm.gotoacloud.top

[B09] break 与 continue
来源：http://xhi.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://exz.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fdt.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrz.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksm.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsn.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ejs.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qvg.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgk.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://gcg.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tju.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lni.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qun.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://leb.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lyv.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rso.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lkg.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xeh.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://ibw.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://cbs.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://iei.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nkv.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yup.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://acw.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nbk.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://xzh.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ouj.pycfn.com

[B12] 跳出多层循环
来源：http://euw.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://qjd.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pph.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gup.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gog.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ssx.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zeu.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://egq.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vlf.chenlongwang.top

[B13] 判断是否为数字
来源：http://odu.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://dmw.chenlongwang.top

PHP:  is_numeric($x)
来源：http://bhc.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qgc.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pak.nanxuanxn.top

Java: x instanceof Number
来源：http://akr.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tdg.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://wwx.cheryme.top

C#:   x is int or double or decimal
来源：http://ygt.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://zgw.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lgf.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rnz.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://fku.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://ioe.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://smw.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iox.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://rcy.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://urf.aibaodan.cn

[B15] 布尔运算与取反
来源：http://fig.xuetiantiany.cn

Py:   a and b or not c
来源：http://bqa.bjfxy.top

PHP:  $a && $b || !$c
来源：http://vya.zhengqikj.top

JS:   a && b || !c
来源：http://qri.iojbl.cn

TS:   a && b || !c
来源：http://uya.hongshengwenyu.top

Java: a && b || !c
来源：http://cfc.52xcode.cn

Go:   a && b || !c
来源：http://deu.jianghu66.top

Ruby: a && b || !c
来源：http://ejj.xuetiantiany.cn

C#:   a && b || !c
来源：http://sqd.yj20258888.top

[B16] 卫语句：不满足条件提前返回
来源：http://wwp.hysaishi.cn

Py:   if not data: return
来源：http://kor.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://bev.jianghu66.top

JS:   if (!data) return;
来源：http://atk.jlsjyb.cn

TS:   if (!data) return;
来源：http://lhw.0kj1m.cn

Java: if (data == null) return;
来源：http://yug.cheryme.top

Go:   if data == nil { return }
来源：http://fpb.iojbl.cn

Ruby: return if data.nil?
来源：http://muw.xziqi.cn

C#:   if (data == null) return;
来源：http://euf.gzhubu.top

================================================================================
来源：http://nwv.shanyushiyangkeji.top

C. 函数与作用域
来源：http://ifh.chenlongwang.top

================================================================================
来源：http://peg.gaohongyu789.top

[C01] 定义函数
来源：http://hwh.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://kaa.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qei.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://ztt.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvu.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://coc.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://kpd.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://rfm.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fyy.chenzaomai.com

[C02] 默认参数
来源：http://mtm.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://bov.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://fqv.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://ciz.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qgq.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://elb.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eez.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://vrc.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://pzl.9152youxi.cn

[C03] 可变参数
来源：http://yjn.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://ufy.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cyl.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://beg.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqu.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cve.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vvz.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yfp.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kxh.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://yzr.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gyj.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kjq.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rjs.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tyl.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hzi.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://gju.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://dyj.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://vom.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://gcn.snrcjt.cn

Py:   return a, b
来源：http://rkj.yj202588.top

PHP:  return [$a, $b];
来源：http://ohx.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sge.zhongyouzk.top

TS:   return { a, b };
来源：http://foz.meibo888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hfy.c1oappe.top

Go:   return a, b
来源：http://weo.feifeiyinyue.top

Ruby: return a, b
来源：http://kgk.aizwys.cn

C#:   return (a, b);              // ValueTuple
来源：http://mre.tanke756.top

[C06] 匿名函数 / lambda
来源：http://vpz.bjfxy.top

Py:   square = lambda x: x * x
来源：http://gbv.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pha.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://rqs.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://vgk.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jvd.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://dem.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://akm.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iqn.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://fwb.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://khs.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://kda.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kus.ppjwa.cn

TS:   arr.map(String)
来源：http://uej.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://izx.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://shw.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://igk.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eth.nwbrower.top

[C08] 闭包
来源：http://vnx.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wmj.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wjt.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bys.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://adu.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vxy.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ucx.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tpp.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://agv.vqdsnc.cn

[C09] 递归
来源：http://hgj.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mmh.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ene.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://frh.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iik.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lbl.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ool.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qjr.zhengqikj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cso.hcnkem.com

[C10] 变量作用域
来源：http://fjv.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nyh.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://esd.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dfd.xylfe.cn

TS:   同 JS
来源：http://ncq.yangfankeji.com

Java: 方法内为块级作用域
来源：http://bte.zycfv.cn

Go:   花括号块级作用域
来源：http://nrd.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://djm.chenlongwang.top

C#:   块级作用域
来源：http://cwn.daxiang520.top

[C11] 模块导入与导出
来源：http://jjg.shzxlz.cn

Py:   from module import func
来源：http://gud.tian-w.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pyw.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ajd.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lmq.xinyue.icu

Java: import java.util.List;
来源：http://pur.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tph.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://myz.zhiwuduotai.top

C#:   using System.Text;
来源：http://pxc.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://zkw.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://oas.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://xsk.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://apc.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://nfi.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kiy.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://lpx.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://nxs.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xrq.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://hwa.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hgt.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qyi.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qda.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbl.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://epy.xinyue.icu

Go:   func add(a, b int) int
来源：http://bst.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tvm.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://mma.shangyingyoupin.top

[C14] 泛型函数
来源：http://nir.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://six.hcnkem.com

PHP:  // 无泛型
来源：http://vwi.fzhhl.top

JS:   // 无泛型
来源：http://gwl.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wxt.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mji.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zfv.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://htx.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mve.fktsv.cn

[C15] 解构 / 展开参数
来源：http://zko.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eou.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://lgw.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qcg.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://abl.pengpengdd.cyou

Java: // 无解构
来源：http://lfm.xuetiantiany.cn

Go:   // 无解构
来源：http://qqv.gogol.net.cn

Ruby: a, b = pair
来源：http://xbn.yueranfly.top

C#:   var (a, b) = pair;
来源：http://eyy.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://eqk.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vxl.aibaodan.cn

PHP:  // 无重载
来源：http://dhk.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://whl.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://glk.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://inq.yvedp.cn


<!-- 参考信息 -->