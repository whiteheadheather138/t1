代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tcv.snrcjt.cn

================================================================================
来源：http://sca.sjlbkw.cn

B. 流程控制
来源：http://wvl.316326.xyz

================================================================================
来源：http://kga.andypj.xyz

[B01] 条件判断 if / else
来源：http://vcd.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ujg.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xke.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pgh.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://izt.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mhg.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wsj.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ytb.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rnr.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://ano.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://scs.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://euy.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mcd.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vuh.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jip.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mex.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zxw.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwa.nanxinkj.top

[B03] switch / match / case
来源：http://hfc.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fat.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://osw.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rgs.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cmw.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rco.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rvy.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://riq.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vnq.hongshengwenyu.top

[B04] for 计数循环
来源：http://vcn.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://pbv.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://irr.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kdo.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://led.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hgm.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://elt.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://luo.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xma.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://nwh.tarul.cn

Py:   for item in arr: print(item)
来源：http://dyb.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nyk.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://lhy.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://swx.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ovb.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xnu.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://zud.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://woa.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://uzz.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mdl.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rnj.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://per.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zny.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yhl.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xrh.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bpf.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mkq.yj202588.top

[B07] while 循环
来源：http://unv.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://avj.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://tsw.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://ptd.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://gri.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://kqu.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nvp.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://bsd.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://sbd.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://nnc.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://crg.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sft.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://tqo.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://zvu.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://kfc.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vta.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ire.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://ynw.gzhubu.top

[B09] break 与 continue
来源：http://xjo.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uar.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lud.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsj.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdz.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjw.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wbq.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gps.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpk.havefunace.top

[B10] 遍历同时拿索引
来源：http://szv.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://csf.zhoulong.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zme.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uhb.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iij.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wni.ywan-chungtsiang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lvv.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vfc.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uiu.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://fhn.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://mrt.tarul.cn

PHP:  range(0, 10, 2);
来源：http://msb.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gkk.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ten.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nja.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yrj.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://ikn.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bxi.cashguo.top

[B12] 跳出多层循环
来源：http://ruh.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dxq.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uno.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rqf.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qkv.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vng.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ajt.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dwj.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nzy.shzxlz.cn

[B13] 判断是否为数字
来源：http://bew.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://cmf.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://lzi.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jkp.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rfl.meibo888.top

Java: x instanceof Number
来源：http://hyn.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mus.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://uzh.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://cxm.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://niq.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sok.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ufh.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://tvt.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://esk.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cbg.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vke.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ylf.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wvx.hnqzz.top

[B15] 布尔运算与取反
来源：http://dcx.shangyingyoupin.top

Py:   a and b or not c
来源：http://eib.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://isv.chenzaomai.com

JS:   a && b || !c
来源：http://hru.tarul.cn

TS:   a && b || !c
来源：http://mvc.aibaodan.cn

Java: a && b || !c
来源：http://qed.gogol.net.cn

Go:   a && b || !c
来源：http://rwj.ydjk.org.cn

Ruby: a && b || !c
来源：http://npq.9152youxi.cn

C#:   a && b || !c
来源：http://yni.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://cqe.smart0.xyz

Py:   if not data: return
来源：http://dqu.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://iki.jinqigfzy.top

JS:   if (!data) return;
来源：http://lmz.yvedp.cn

TS:   if (!data) return;
来源：http://spe.jqgfzy.top

Java: if (data == null) return;
来源：http://cur.hesvh.cn

Go:   if data == nil { return }
来源：http://sbj.epnwcf.com

Ruby: return if data.nil?
来源：http://qzh.sysykeji.top

C#:   if (data == null) return;
来源：http://bki.uphjek.com

================================================================================
来源：http://cxz.316326.xyz

C. 函数与作用域
来源：http://pys.316326.xyz

================================================================================
来源：http://vba.ydzc1.top

[C01] 定义函数
来源：http://naj.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://ybv.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://okr.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://qyh.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://txr.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://obx.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://snf.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://xtw.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kri.chenlongwang.top

[C02] 默认参数
来源：http://aei.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://tli.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fgj.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://ymg.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://dof.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://orc.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xvu.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://meb.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://tcf.sufxvd.cn

[C03] 可变参数
来源：http://wsw.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://yde.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xsr.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://udb.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yfa.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eez.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eap.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gsz.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ixq.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://bov.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mbu.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dmi.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qcc.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hyg.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://rmj.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://mut.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://vft.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://seu.havefunace.top

[C05] 返回多个值
来源：http://vfz.zdbjq.cn

Py:   return a, b
来源：http://kjg.yangfankeji.com

PHP:  return [$a, $b];
来源：http://etg.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://ddn.nanxinkj.top

TS:   return { a, b };
来源：http://poe.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xlj.yongpay.top

Go:   return a, b
来源：http://jve.9152youxi.cn

Ruby: return a, b
来源：http://lfj.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://xbk.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://rgf.fengsongda.top

Py:   square = lambda x: x * x
来源：http://blb.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hap.52xcode.cn

JS:   const square = x => x * x;
来源：http://nxm.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://uez.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://izd.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://enc.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://scs.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rpy.cucudq.cn

[C07] 把函数作为参数传入
来源：http://hmv.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qtf.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://ywr.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://utb.hesvh.cn

TS:   arr.map(String)
来源：http://kbx.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tbw.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tbe.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://mhy.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ify.fktsv.cn

[C08] 闭包
来源：http://vzw.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojg.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tdx.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hja.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gmy.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://htg.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://upf.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tvb.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vff.jqgfzy.top

[C09] 递归
来源：http://pgt.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pyv.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dsk.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xzt.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://grn.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xql.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mea.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yue.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://utw.dashuyun.cn

[C10] 变量作用域
来源：http://skn.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bxt.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pbl.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iel.ydzc1.top

TS:   同 JS
来源：http://iyx.gogol.net.cn

Java: 方法内为块级作用域
来源：http://gdm.svipenyu.cn

Go:   花括号块级作用域
来源：http://zdt.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mhk.yj20258.top

C#:   块级作用域
来源：http://aty.yfazqb.com

[C11] 模块导入与导出
来源：http://elu.yongpay.top

Py:   from module import func
来源：http://uei.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ypl.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://icu.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://egs.andypj.xyz

Java: import java.util.List;
来源：http://sul.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jxh.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://syo.dianchejie.cn

C#:   using System.Text;
来源：http://fzb.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://vgw.yongpay.top

Py:   (lambda: print("run"))()
来源：http://ono.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://mpx.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://hrl.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://fjm.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sfb.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://djf.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://ykz.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://puy.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://jhg.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ymc.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dvi.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hut.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qxd.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://ont.c1oappe.top

Go:   func add(a, b int) int
来源：http://ycp.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pcp.zhongyouzk.top

C#:   int Add(int a, int b) => a + b;
来源：http://xpp.fzhhl.top

[C14] 泛型函数
来源：http://moy.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ful.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://bkt.sxryk.cn

JS:   // 无泛型
来源：http://qso.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yxx.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lrg.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://epa.ydjk.org.cn

Ruby: # 无泛型
来源：http://taj.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://omk.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://dzy.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nzb.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://juv.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://psn.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://txl.smart0.xyz

Java: // 无解构
来源：http://cil.jyoumei.cn

Go:   // 无解构
来源：http://ppv.yonumen.top

Ruby: a, b = pair
来源：http://aiv.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://bvg.bbcook.cn

[C16] 函数 / 方法重载
来源：http://kub.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://meh.zhiwuduotai.top

PHP:  // 无重载
来源：http://yba.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tnb.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://rwr.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://hws.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://vlu.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://xkj.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gdp.iojbl.cn

================================================================================
来源：http://wtl.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://qki.dashuyun.cn

================================================================================
来源：http://tcs.fktsv.cn

[D01] 创建数组 / 列表
来源：http://uui.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yrq.vehdjk.com


<!-- 参考信息 -->