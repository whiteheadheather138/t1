代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://eey.hesvh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lhd.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://szm.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qqn.smart0.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pyc.zhongyouzk.top

================================================================================
来源：http://gtu.kuanghao11.cn

B. 流程控制
来源：http://zlv.aibaodan.cn

================================================================================
来源：http://ksu.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://lgw.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nup.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hur.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ewo.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cxs.andypj.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://kly.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rnk.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fow.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hmi.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://qmf.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://juh.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://imz.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxw.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tap.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kkh.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rss.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oda.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmq.yj20258888.top

[B03] switch / match / case
来源：http://cbc.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://apr.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ing.feifeiyinyue.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ijf.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uzp.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dzd.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ish.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hhl.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mfs.aizwys.cn

[B04] for 计数循环
来源：http://cdw.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://qme.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ufl.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://icf.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bbo.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mzt.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://edn.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://haw.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bcj.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://hol.tanke756.top

Py:   for item in arr: print(item)
来源：http://wdb.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://neo.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wxf.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://hre.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rqi.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eey.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://mlq.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aeu.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://qna.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nxy.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tkz.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://elm.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvc.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hky.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zqo.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ntz.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://som.ydjk.org.cn

[B07] while 循环
来源：http://rie.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://ufm.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://nvb.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://xuj.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://gzk.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://pdh.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zwj.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://opa.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://nhj.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://zxg.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://bzm.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xjp.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://ejr.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://glu.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://wld.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aku.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://uby.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://wwl.fzhhl.top

[B09] break 与 continue
来源：http://fvo.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tkf.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wbt.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmq.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrd.ivvv.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ltv.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://acf.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ovt.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gew.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://rvc.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jtj.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xvt.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pbs.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qux.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://axb.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kwx.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://syn.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rtz.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://rkf.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://wkc.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://xnt.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gva.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yyg.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oyy.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tqy.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://rzt.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://okj.jinqigfzy.top

[B12] 跳出多层循环
来源：http://fmu.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dhe.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fhk.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzv.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iwu.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dbh.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fez.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yjj.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rtx.zdbjq.cn

[B13] 判断是否为数字
来源：http://sss.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://bom.yonumen.top

PHP:  is_numeric($x)
来源：http://rvq.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://puy.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dge.tianlin.xyz

Java: x instanceof Number
来源：http://ljo.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tjl.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://qpp.gotoacloud.top

C#:   x is int or double or decimal
来源：http://qdi.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://qgg.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xnr.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oug.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://rkg.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://xlf.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zky.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lde.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://umx.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mbg.pycfn.com

[B15] 布尔运算与取反
来源：http://ths.hongshengwenyu.top

Py:   a and b or not c
来源：http://ekv.jianghu66.top

PHP:  $a && $b || !$c
来源：http://cec.quarkkingdee.top

JS:   a && b || !c
来源：http://lwr.yanxiufei.cn

TS:   a && b || !c
来源：http://pum.xinyue.icu

Java: a && b || !c
来源：http://csz.zhiwuduotai.top

Go:   a && b || !c
来源：http://zsf.dashuyun.cn

Ruby: a && b || !c
来源：http://cqs.shangyingyoupin.top

C#:   a && b || !c
来源：http://rqj.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://bni.vqdsnc.cn

Py:   if not data: return
来源：http://drv.cashguo.top

PHP:  if (!$data) { return; }
来源：http://iof.zdbjq.cn

JS:   if (!data) return;
来源：http://xnd.chenjidiqi.icu

TS:   if (!data) return;
来源：http://ecw.bjfxy.top

Java: if (data == null) return;
来源：http://yya.sjlbkw.cn

Go:   if data == nil { return }
来源：http://ypk.jinqigfzy.top

Ruby: return if data.nil?
来源：http://yvx.iojbl.cn

C#:   if (data == null) return;
来源：http://rlr.zhixingplan.top

================================================================================
来源：http://ewe.zhaomingkeji.xyz

C. 函数与作用域
来源：http://koy.jyoumei.cn

================================================================================
来源：http://yzo.wangshuangyany.cn

[C01] 定义函数
来源：http://jim.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://dll.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://phn.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://ten.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tin.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://geb.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://peq.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://djj.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hhz.9152youxi.cn

[C02] 默认参数
来源：http://hbz.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://zqb.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ngd.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://sui.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bfp.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://edu.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xtd.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://lpk.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://fwp.nwbrower.top

[C03] 可变参数
来源：http://tpl.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://kxl.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://apl.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zbh.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://haq.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sed.jinqigufen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gny.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vai.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rdp.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://nlm.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wgj.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hee.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ltr.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tcv.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://vkv.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://ffs.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://tja.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://dga.chenjidiqi.icu

[C05] 返回多个值
来源：http://pvf.gogol.net.cn

Py:   return a, b
来源：http://mgw.daria6918.cn

PHP:  return [$a, $b];
来源：http://zcm.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://twq.cashguo.top

TS:   return { a, b };
来源：http://xdw.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bmx.zhaomingkeji.xyz

Go:   return a, b
来源：http://wla.hongshengwenyu.top

Ruby: return a, b
来源：http://uzl.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://ixq.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://dpe.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://bnn.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aex.yuxming.cn

JS:   const square = x => x * x;
来源：http://qmb.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://pfp.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zyk.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://yfv.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://gjc.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://nts.vehdjk.com

[C07] 把函数作为参数传入
来源：http://osr.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bcr.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fne.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hlp.jqgufenzy.top

TS:   arr.map(String)
来源：http://mlz.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ecr.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lpu.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://wsf.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wrd.sysykeji.top

[C08] 闭包
来源：http://pdo.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vgo.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hyp.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://who.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dph.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pqj.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yzp.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ext.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ypn.c1oappe.top

[C09] 递归
来源：http://paa.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hca.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uen.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://unv.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijx.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wbc.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wva.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ila.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ncl.hnqzz.top

[C10] 变量作用域
来源：http://wju.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lym.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://scs.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mqa.bbcook.cn

TS:   同 JS
来源：http://qxp.tianlin.xyz

Java: 方法内为块级作用域
来源：http://cre.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://lhe.daria6918.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ogv.gotoacloud.top

C#:   块级作用域
来源：http://lul.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://pmg.nanxuanxn.top

Py:   from module import func
来源：http://ixe.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kvt.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://ysg.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ufw.shanyushiyangkeji.top

Java: import java.util.List;
来源：http://zqe.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jaf.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://jao.vehdjk.com

C#:   using System.Text;
来源：http://ofw.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://szf.tanke756.top

Py:   (lambda: print("run"))()
来源：http://okr.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://kbj.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://don.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://vpb.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ivg.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://dgy.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://tzh.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mmm.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://cry.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sau.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pun.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bsi.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://evi.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tlp.snrcjt.cn

Go:   func add(a, b int) int
来源：http://trt.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://prl.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://rhf.hywenlv.cn

[C14] 泛型函数
来源：http://vjc.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tmm.daria6918.cn

PHP:  // 无泛型
来源：http://xga.zycfv.cn

JS:   // 无泛型
来源：http://sre.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jqi.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ljz.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jcv.mhx1999.top

Ruby: # 无泛型
来源：http://chx.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dep.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://gzm.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nwt.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://zxl.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qlf.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ibr.vehdjk.com

Java: // 无解构
来源：http://icv.xziqi.cn

Go:   // 无解构
来源：http://jgh.yuanzhike.top

Ruby: a, b = pair
来源：http://jcw.xziqi.cn

C#:   var (a, b) = pair;
来源：http://dgc.fehbvm.com

[C16] 函数 / 方法重载
来源：http://evy.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zgq.fengsongda.top

PHP:  // 无重载
来源：http://sjq.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ojm.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://evl.sufxvd.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hau.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://ika.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://uvx.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xal.jinghuilouyu.cn

================================================================================
来源：http://puv.yvedp.cn


<!-- 参考信息 -->