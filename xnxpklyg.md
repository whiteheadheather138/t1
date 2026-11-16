代发 wailian999

[B01] 条件判断 if / else
来源：http://lyk.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://itd.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://swq.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://maj.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wqq.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ace.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oei.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tql.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fjf.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://amz.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wfn.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bpf.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://omb.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmt.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qap.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gux.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nzh.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxw.daxiang520.top

[B03] switch / match / case
来源：http://vly.hnxiangtu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cqb.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ymt.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nwv.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://osp.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://whs.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zwo.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vgh.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xue.shanyushiyangkeji.top

[B04] for 计数循环
来源：http://oyf.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://kbc.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qtv.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nko.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pwt.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nbb.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://acm.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://nbd.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vwh.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://xwp.fengsongda.top

Py:   for item in arr: print(item)
来源：http://udp.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ine.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bpx.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://wyb.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jxp.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vyv.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://vzp.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tog.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://epc.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zym.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dzz.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wls.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lqg.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ewe.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gar.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kct.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lqq.xylfe.cn

[B07] while 循环
来源：http://xma.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://vay.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qfs.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://yom.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://ycc.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://mmb.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gin.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://pmj.sweek.top

C#:   while (i < 10) { i++; }
来源：http://ojh.yonumen.top

[B08] do-while（至少执行一次）
来源：http://mku.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://aeq.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://orr.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://yrh.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://onb.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://dsr.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://snv.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://kru.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://sjw.hcnkem.com

[B09] break 与 continue
来源：http://uob.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vww.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ktg.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zej.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://heu.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmb.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lxd.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cze.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oys.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://ult.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://waz.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bdx.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qso.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cxp.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://evj.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bgk.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tyc.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nrx.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://kbf.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://sit.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://axh.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gaz.ywan-chungtsiang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eeh.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ywh.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ykf.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://bvc.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cyq.jlsjyb.cn

[B12] 跳出多层循环
来源：http://oiu.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cxj.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fgr.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mli.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vub.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tbz.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vgd.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aae.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cnp.ybcxt.top

[B13] 判断是否为数字
来源：http://jkf.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://jtv.tianlin.xyz

PHP:  is_numeric($x)
来源：http://inj.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ren.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ray.zhiwuduotai.top

Java: x instanceof Number
来源：http://adu.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ogy.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://adl.fehbvm.com

C#:   x is int or double or decimal
来源：http://ezr.52xcode.cn

[B14] 判断值是否在集合内
来源：http://tne.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mnv.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ynj.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://tbd.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://mqn.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ecj.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hnu.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://jsf.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hqf.xuanzx.com

[B15] 布尔运算与取反
来源：http://tua.hnqzz.top

Py:   a and b or not c
来源：http://fvi.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://ltd.hnxiangtu.top

JS:   a && b || !c
来源：http://ywv.zhoulong.xyz

TS:   a && b || !c
来源：http://mcm.jiagoushi.top

Java: a && b || !c
来源：http://vvf.ctjpmb.com

Go:   a && b || !c
来源：http://iph.nwbrower.top

Ruby: a && b || !c
来源：http://ggc.jlsjyb.cn

C#:   a && b || !c
来源：http://aeh.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://hkn.hnxiangtu.top

Py:   if not data: return
来源：http://ggo.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://crv.cdnleiting.top

JS:   if (!data) return;
来源：http://ets.epnwcf.com

TS:   if (!data) return;
来源：http://qjm.zhongyouzk.top

Java: if (data == null) return;
来源：http://bmo.jqgufenzy.top

Go:   if data == nil { return }
来源：http://toi.quarkkingdee.top

Ruby: return if data.nil?
来源：http://nak.nanxuanxn.top

C#:   if (data == null) return;
来源：http://ipd.zycfv.cn

================================================================================
来源：http://eyv.meibo888.top

C. 函数与作用域
来源：http://vgp.yj20258.top

================================================================================
来源：http://sya.cucudq.cn

[C01] 定义函数
来源：http://mjq.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://pxr.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bcq.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://zio.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rze.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rcw.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://zwa.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://bbs.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lqc.zhixingplan.top

[C02] 默认参数
来源：http://zhn.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://qgv.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dry.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://xki.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vtz.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iwr.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gkl.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://syd.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://cph.shzxlz.cn

[C03] 可变参数
来源：http://fzw.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://opg.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://akb.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fko.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mjq.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oqs.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://acl.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://bxb.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zjl.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://xxo.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kwu.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gys.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ovm.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sbn.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://gqz.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://acl.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://taz.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://rsj.zhijiandao.cn

[C05] 返回多个值
来源：http://kna.birdmap.top

Py:   return a, b
来源：http://cgh.jyoumei.cn

PHP:  return [$a, $b];
来源：http://lqd.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rqy.ppjwa.cn

TS:   return { a, b };
来源：http://dvq.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ijc.zhiwuduotai.top

Go:   return a, b
来源：http://tbo.aibaodan.cn

Ruby: return a, b
来源：http://tmm.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://jbf.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://jsb.yfazqb.com

Py:   square = lambda x: x * x
来源：http://xqa.yanxiufei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jaq.yueranfly.top

JS:   const square = x => x * x;
来源：http://zil.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://umb.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iaj.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://mfb.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://ozz.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://iox.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://pzd.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ihd.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://znl.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ymz.jianghu66.top

TS:   arr.map(String)
来源：http://zrl.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zdw.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://igb.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://jiy.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://isx.52xcode.cn

[C08] 闭包
来源：http://qin.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ryk.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bid.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ikt.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cck.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gev.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://php.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://spg.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qol.hesvh.cn

[C09] 递归
来源：http://gvo.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://asb.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yum.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zhb.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjp.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rej.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://geb.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wgi.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sus.redwolf501.top

[C10] 变量作用域
来源：http://pfq.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tyf.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zph.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://myw.zhixingplan.top

TS:   同 JS
来源：http://ucy.epnwcf.com

Java: 方法内为块级作用域
来源：http://tif.cucudq.cn

Go:   花括号块级作用域
来源：http://rrm.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://plu.haohaochexian.top

C#:   块级作用域
来源：http://toy.jyoumei.cn

[C11] 模块导入与导出
来源：http://onx.xingfuxueyuan.xyz

Py:   from module import func
来源：http://gsp.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jai.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://prp.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cto.jyoumei.cn

Java: import java.util.List;
来源：http://ypv.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jha.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://jnk.sysykeji.top

C#:   using System.Text;
来源：http://roz.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://zjx.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://brw.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://hxz.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://doy.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://apo.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cja.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://cvz.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://pha.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cku.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://vvr.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ncm.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qgv.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zln.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zvm.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://ozi.jiagoushi.top

Go:   func add(a, b int) int
来源：http://eca.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wrx.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qre.guannengcc.top

[C14] 泛型函数
来源：http://azl.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qzd.kuanghao11.cn

PHP:  // 无泛型
来源：http://wbl.jinqigufen.top

JS:   // 无泛型
来源：http://pqm.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vbu.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lwv.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://urq.iojbl.cn

Ruby: # 无泛型
来源：http://byb.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bhv.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://gdr.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mee.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://rnw.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pqy.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qyg.yongpay.top

Java: // 无解构
来源：http://xlv.gogol.net.cn

Go:   // 无解构
来源：http://tpl.zhoulong.xyz

Ruby: a, b = pair
来源：http://tcq.iojbl.cn

C#:   var (a, b) = pair;
来源：http://zkr.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://puu.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://epm.hfpthk.cn

PHP:  // 无重载
来源：http://bey.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xgb.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://fwz.cheryme.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gur.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://gfa.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://tph.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://waj.yueranfly.top

================================================================================
来源：http://mcd.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://ngv.9152youxi.cn

================================================================================
来源：http://bgv.316326.xyz

[D01] 创建数组 / 列表
来源：http://tfq.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://npf.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ylt.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ymw.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xuw.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zwq.jqgufenzy.top


<!-- 参考信息 -->