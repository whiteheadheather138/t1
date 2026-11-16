代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://tfl.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fmz.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ikg.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://feu.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kje.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ciw.iojbl.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kzw.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qwe.xziqi.cn

[A26] 类型转换总览
来源：http://mkh.daxiang520.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uip.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://poc.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wzq.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://yfg.xuetiantiany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xan.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yga.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vqk.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://goh.chenzaomai.com

================================================================================
来源：http://mey.jqgfzy.top

B. 流程控制
来源：http://miv.tianlin.xyz

================================================================================
来源：http://tuq.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://dls.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://jht.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tnp.hammf.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://prp.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://agr.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://qxf.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nfr.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqr.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aqx.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://dvq.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xxg.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ule.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nbx.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ube.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehl.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lzs.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ksr.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exi.hcnkem.com

[B03] switch / match / case
来源：http://bvg.hcnkem.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uhs.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gjl.zhongyouzk.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://anm.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vpf.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wyz.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ekx.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mht.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mrv.sweek.top

[B04] for 计数循环
来源：http://owa.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://ybh.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://udf.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exj.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ooe.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xvw.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nyx.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://owt.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ffv.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://jep.pycfn.com

Py:   for item in arr: print(item)
来源：http://kew.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ipb.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xlk.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://jdg.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://rji.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pdv.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://wgf.zycfv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://foq.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://vyo.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ddw.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nil.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odu.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpn.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fot.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sex.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nrj.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gqo.bjfxy.top

[B07] while 循环
来源：http://lcq.xinyue.icu

Py:   while i < 10: i += 1
来源：http://dej.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://eoz.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://gsi.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://rkz.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://sky.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://soc.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://bcw.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://vol.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://phz.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://uqh.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lnn.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://exy.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://yrz.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://evg.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://guq.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://uqh.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://xuj.guowangkeji.top

[B09] break 与 continue
来源：http://sdw.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hvx.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://due.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzj.daria6918.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://urt.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pkh.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xwk.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ddp.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogn.nwbrower.top

[B10] 遍历同时拿索引
来源：http://xgs.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qrt.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jey.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dmw.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rgx.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yev.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ldv.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ezf.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eeu.smart0.xyz

[B11] 生成数字序列 / 区间
来源：http://tfn.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://jls.yonumen.top

PHP:  range(0, 10, 2);
来源：http://exc.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fay.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://acr.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fdo.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tfy.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://gjg.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mey.jqgfzy.top

[B12] 跳出多层循环
来源：http://sif.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://due.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://shc.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lri.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://njb.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jap.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vvj.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wum.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jjm.vqdsnc.cn

[B13] 判断是否为数字
来源：http://jyd.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://owy.52xcode.cn

PHP:  is_numeric($x)
来源：http://agq.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://snd.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wkl.yfazqb.com

Java: x instanceof Number
来源：http://gwk.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ucg.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://guz.jiagoushi.top

C#:   x is int or double or decimal
来源：http://tyu.daria6918.cn

[B14] 判断值是否在集合内
来源：http://vpk.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ydg.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tda.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://bxv.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://adm.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fsi.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rof.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xjd.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://buq.sweek.top

[B15] 布尔运算与取反
来源：http://xdg.ybcxt.top

Py:   a and b or not c
来源：http://yzy.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://ojo.wangdashe.top

JS:   a && b || !c
来源：http://pno.nanxinkj.top

TS:   a && b || !c
来源：http://mnb.sufxvd.cn

Java: a && b || !c
来源：http://mlj.ivvv.top

Go:   a && b || !c
来源：http://shu.dashuyun.cn

Ruby: a && b || !c
来源：http://xnn.316326.xyz

C#:   a && b || !c
来源：http://elh.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://bif.jlsjyb.cn

Py:   if not data: return
来源：http://jyg.yj202588.top

PHP:  if (!$data) { return; }
来源：http://wwd.jqgufenzy.top

JS:   if (!data) return;
来源：http://uai.cqqwz.cn

TS:   if (!data) return;
来源：http://owh.yongpay.top

Java: if (data == null) return;
来源：http://hje.fzhhl.top

Go:   if data == nil { return }
来源：http://rjj.uphjek.com

Ruby: return if data.nil?
来源：http://jeg.tarul.cn

C#:   if (data == null) return;
来源：http://efb.bbcook.cn

================================================================================
来源：http://lwo.sweek.top

C. 函数与作用域
来源：http://qus.tian-w.cn

================================================================================
来源：http://uws.snrcjt.cn

[C01] 定义函数
来源：http://gnu.uphjek.com

Py:   def add(a, b): return a + b
来源：http://tue.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ojb.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://nxs.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bhn.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zcp.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://grj.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://owy.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pmk.gogol.net.cn

[C02] 默认参数
来源：http://sce.uphjek.com

Py:   def greet(name="World"): return name
来源：http://zrx.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hrm.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://fjy.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uxw.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sax.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ckg.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://dwz.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://sjo.chenzaomai.com

[C03] 可变参数
来源：http://pzb.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://ecq.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gmi.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://psq.jqgufenzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzm.ivvv.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://byb.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vcb.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lay.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kxz.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://yao.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tyz.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mcg.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pzp.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ixg.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://tsc.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://enq.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://fyu.smart0.xyz

C#:   f(a: 1, b: 2)
来源：http://ynt.sysykeji.top

[C05] 返回多个值
来源：http://jud.yangfankeji.com

Py:   return a, b
来源：http://atd.ehwqpu.com

PHP:  return [$a, $b];
来源：http://vru.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eil.kuanghao11.cn

TS:   return { a, b };
来源：http://mbd.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qbq.zhongyouzk.top

Go:   return a, b
来源：http://toi.zdbjq.cn

Ruby: return a, b
来源：http://fuj.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://dfz.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://yvb.c1oappe.top

Py:   square = lambda x: x * x
来源：http://fwa.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aoj.iojbl.cn

JS:   const square = x => x * x;
来源：http://jsw.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://hgj.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oza.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ury.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://euw.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://buo.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://lta.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zrw.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://bbj.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qcj.zdqjudy.top

TS:   arr.map(String)
来源：http://lar.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://seu.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qix.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://fzk.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://prl.vehdjk.com

[C08] 闭包
来源：http://gml.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wbn.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://svl.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://drz.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hig.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oue.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ivv.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://odb.xziqi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zkd.jianghu66.top

[C09] 递归
来源：http://qax.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cin.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://spm.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://prp.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bjw.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vah.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cpd.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vue.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dkq.yuxming.cn

[C10] 变量作用域
来源：http://kze.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cty.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wbq.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahh.zhixingplan.top

TS:   同 JS
来源：http://bmt.jyoumei.cn

Java: 方法内为块级作用域
来源：http://kqv.jiagoushi.top

Go:   花括号块级作用域
来源：http://jnq.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://awx.yueranfly.top

C#:   块级作用域
来源：http://exp.cdnleiting.top

[C11] 模块导入与导出
来源：http://rku.pycfn.com

Py:   from module import func
来源：http://lje.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dxm.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://amn.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wlx.hysaishi.cn

Java: import java.util.List;
来源：http://oaz.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xnb.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://zgb.cashguo.top

C#:   using System.Text;
来源：http://kbs.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://qxd.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://dre.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://alx.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://kgl.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://zlc.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cep.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://sim.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://qdu.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://alx.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://nes.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vsb.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qqc.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ppx.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://keo.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://bku.wangdashe.top

Go:   func add(a, b int) int
来源：http://qlv.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://avr.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://swc.jiagoushi.top

[C14] 泛型函数
来源：http://nde.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bzr.fktsv.cn

PHP:  // 无泛型
来源：http://oxb.shuidangran.top

JS:   // 无泛型
来源：http://xtu.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nxe.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hvz.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://swe.fengsongda.top

Ruby: # 无泛型
来源：http://cot.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wyb.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://rke.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vsa.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://ksw.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ipt.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sxn.316326.xyz

Java: // 无解构
来源：http://wpk.ywan-chungtsiang.top

Go:   // 无解构
来源：http://nyt.0kj1m.cn


<!-- 参考信息 -->