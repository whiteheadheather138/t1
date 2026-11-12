代发 wailian999

[A26] 类型转换总览
来源：http://lak.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jre.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nem.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ivt.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://noq.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cdw.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zxq.xziqi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://exz.jqgfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://noo.sufxvd.cn

================================================================================
来源：http://dtk.xylfe.cn

B. 流程控制
来源：http://vot.epnwcf.com

================================================================================
来源：http://yab.52xcode.cn

[B01] 条件判断 if / else
来源：http://eln.ctjpmb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://bhf.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gpt.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hpz.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://waq.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dul.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gyv.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iin.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zmt.nwbrower.top

[B02] 多分支 else if / elif
来源：http://mjx.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ozt.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cxa.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovf.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dvg.redwolf501.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyq.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vdg.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iyt.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bst.yj20258.top

[B03] switch / match / case
来源：http://jlj.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vfs.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ooz.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uja.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://asn.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ylw.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oqg.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dab.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lup.fzhhl.top

[B04] for 计数循环
来源：http://cyj.tanke756.top

Py:   for i in range(10): print(i)
来源：http://pir.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hbv.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uja.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ycc.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://scx.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bzc.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://ogr.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bws.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://wca.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://owb.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://paq.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iyt.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://yko.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bgt.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kpm.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://vgl.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xty.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://axs.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wob.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mwq.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ovr.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://noj.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mkw.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pye.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xzv.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bcy.chenjidiqi.icu

[B07] while 循环
来源：http://bdi.yueranfly.top

Py:   while i < 10: i += 1
来源：http://eic.jianghu66.top

PHP:  while ($i < 10) { $i++; }
来源：http://cgl.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://zhx.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://xbf.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://unq.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yxh.cheryme.top

Ruby: while i < 10; i += 1; end
来源：http://eyf.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://mab.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://gqc.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://wdj.jqgfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://idx.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://ytr.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://kfo.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://lpp.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vnv.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cgn.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://xro.pycfn.com

[B09] break 与 continue
来源：http://xyn.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fmx.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bcv.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsr.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvc.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlm.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xzq.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gql.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvl.shangyingyoupin.top

[B10] 遍历同时拿索引
来源：http://hrp.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fto.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gnf.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wcm.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xmy.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fkv.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ebm.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hfr.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://psn.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://oln.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://tkj.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://ugu.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oxu.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xub.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dyp.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://atf.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://sof.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nzs.sysykeji.top

[B12] 跳出多层循环
来源：http://rvw.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vbn.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cch.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pop.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kdj.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://grm.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fkx.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fix.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://psw.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://ldx.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://jki.haohaochexian.top

PHP:  is_numeric($x)
来源：http://mjb.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sgg.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ujx.jqgufenzy.top

Java: x instanceof Number
来源：http://ldw.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jxh.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://udu.havefunace.top

C#:   x is int or double or decimal
来源：http://rce.yj202588.top

[B14] 判断值是否在集合内
来源：http://hho.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bfl.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uls.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://xss.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://vnk.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fzn.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gfv.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://cgn.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jlb.bjfxy.top

[B15] 布尔运算与取反
来源：http://nsz.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://ibu.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://nnn.hammf.cn

JS:   a && b || !c
来源：http://aue.jinqigufen.top

TS:   a && b || !c
来源：http://hex.xylfe.cn

Java: a && b || !c
来源：http://taa.ehwqpu.com

Go:   a && b || !c
来源：http://cts.sxryk.cn

Ruby: a && b || !c
来源：http://hus.smart0.xyz

C#:   a && b || !c
来源：http://keu.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oep.jinqigfzy.top

Py:   if not data: return
来源：http://mci.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://xdi.xylfe.cn

JS:   if (!data) return;
来源：http://dyr.ydjk.org.cn

TS:   if (!data) return;
来源：http://vyr.quarkkingdee.top

Java: if (data == null) return;
来源：http://yds.hesvh.cn

Go:   if data == nil { return }
来源：http://wqa.ydjk.org.cn

Ruby: return if data.nil?
来源：http://ief.jinqigufen.top

C#:   if (data == null) return;
来源：http://dnc.sufxvd.cn

================================================================================
来源：http://zlc.epnwcf.com

C. 函数与作用域
来源：http://uyz.aibaodan.cn

================================================================================
来源：http://got.jinyuanbaomall.cn

[C01] 定义函数
来源：http://uss.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://qbp.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lbx.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://afd.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://elw.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gel.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://nuj.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://cif.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fkm.daria6918.cn

[C02] 默认参数
来源：http://gjc.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://zms.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vvc.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://hbn.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qqv.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hrp.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hve.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://tuv.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://tnv.shangyingyoupin.top

[C03] 可变参数
来源：http://bxx.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://puh.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xhq.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rws.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gcc.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kov.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jtl.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://oyp.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://awx.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://znw.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gai.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jvc.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://euh.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fte.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://gmh.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://zvn.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://qsy.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://rfl.cheryme.top

[C05] 返回多个值
来源：http://fph.daxiang520.top

Py:   return a, b
来源：http://lgc.9152youxi.cn

PHP:  return [$a, $b];
来源：http://uve.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ikw.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://aye.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kwf.jqgufenzy.top

Go:   return a, b
来源：http://rod.jinghuilouyu.cn

Ruby: return a, b
来源：http://fmz.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://phh.yongpay.top

[C06] 匿名函数 / lambda
来源：http://ecf.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://uta.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rro.jqgfzy.top

JS:   const square = x => x * x;
来源：http://mtt.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://swv.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://abb.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ypg.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://suq.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://bgd.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://lzp.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ixa.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kzy.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://std.bjfxy.top

TS:   arr.map(String)
来源：http://olb.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xcr.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xml.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://jzg.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://onw.chenjidiqi.icu

[C08] 闭包
来源：http://uab.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ekl.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sfn.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gql.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nsk.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tji.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zir.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lio.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aip.yvedp.cn

[C09] 递归
来源：http://oce.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kde.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zok.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tjg.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://izr.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xao.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hok.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tqr.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dsb.chenzaomai.com

[C10] 变量作用域
来源：http://qsl.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mrb.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fss.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://azt.yuxming.cn

TS:   同 JS
来源：http://cwi.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://wzm.shzxlz.cn

Go:   花括号块级作用域
来源：http://mws.c1oappe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nxm.smart0.xyz

C#:   块级作用域
来源：http://qbg.aibaodan.cn

[C11] 模块导入与导出
来源：http://oce.yongpay.top

Py:   from module import func
来源：http://cue.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://clf.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wvt.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wiu.yanxiufei.cn

Java: import java.util.List;
来源：http://ixz.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ocs.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ovb.tanke756.top

C#:   using System.Text;
来源：http://art.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://swb.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://mnn.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://mqe.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://aiz.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://jay.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fug.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://ash.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://eui.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fxc.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://mrw.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://asz.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lzh.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bge.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://miz.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mnb.smart0.xyz

Go:   func add(a, b int) int
来源：http://gjn.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hbk.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zdh.fengsongda.top

[C14] 泛型函数
来源：http://uyi.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iqf.gotoacloud.top

PHP:  // 无泛型
来源：http://gyc.sxryk.cn

JS:   // 无泛型
来源：http://ior.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://suw.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cmh.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uht.yonumen.top

Ruby: # 无泛型
来源：http://mjg.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jxp.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://fki.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cco.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://czs.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dhv.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ukm.zdbjq.cn

Java: // 无解构
来源：http://snb.kuanghao11.cn

Go:   // 无解构
来源：http://dxg.zhiwuduotai.top

Ruby: a, b = pair
来源：http://eew.yvedp.cn

C#:   var (a, b) = pair;
来源：http://oqp.yj20258.top

[C16] 函数 / 方法重载
来源：http://wqq.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dvp.yj202588.top

PHP:  // 无重载
来源：http://rmy.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xyx.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://bnx.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://drt.316326.xyz


<!-- 参考信息 -->