代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gea.zycfv.cn

================================================================================
来源：http://kdy.smart0.xyz

B. 流程控制
来源：http://wkr.0kj1m.cn

================================================================================
来源：http://etz.xylfe.cn

[B01] 条件判断 if / else
来源：http://kzu.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bas.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mny.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://czl.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uwt.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://uay.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://imz.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ikd.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nrl.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://avz.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kzk.zhijiandao.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zhw.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jxr.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mih.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cnb.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xhq.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tcp.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rqy.jinghuilouyu.cn

[B03] switch / match / case
来源：http://jki.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gdb.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xqu.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yif.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dib.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://beb.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jrz.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tfk.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tds.daria6918.cn

[B04] for 计数循环
来源：http://aok.cashguo.top

Py:   for i in range(10): print(i)
来源：http://qxz.sjlbkw.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cjw.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lem.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uao.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cet.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vhu.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://qro.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lpo.havefunace.top

[B05] 遍历数组 / 列表
来源：http://liv.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://lcc.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://csx.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cdk.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ykn.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hqm.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://trl.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://hgw.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zac.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://qvg.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tzb.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rmy.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rwx.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bul.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zpn.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jhz.xylfe.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lmf.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://soz.zhengqikj.top

[B07] while 循环
来源：http://ffk.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://fkj.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://hsi.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://nbi.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://dev.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://zhl.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mei.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://cjk.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://spo.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://iip.yuanzhike.top

Py:   # 无 do-while：用 while True + break
来源：http://kxt.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vyz.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://txa.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://kjc.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://gdw.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bau.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://ooy.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://uqi.tanke756.top

[B09] break 与 continue
来源：http://kfr.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uvv.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vlk.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksp.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wih.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ieq.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gyv.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://icj.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hdb.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://jxl.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://woi.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vgj.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fao.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hns.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kru.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ocl.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pxk.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aqe.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://clt.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://jtc.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://xbv.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qax.ywan-chungtsiang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vml.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wdr.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://omy.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://glp.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://heg.hnqzz.top

[B12] 跳出多层循环
来源：http://fsd.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eon.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fva.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mlm.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmt.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cst.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ddj.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jxt.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aby.dashuyun.cn

[B13] 判断是否为数字
来源：http://zlt.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://duy.dianchejie.cn

PHP:  is_numeric($x)
来源：http://rbh.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gia.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://crq.sjlbkw.cn

Java: x instanceof Number
来源：http://zyr.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dos.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://jje.yueranfly.top

C#:   x is int or double or decimal
来源：http://ybq.yueranfly.top

[B14] 判断值是否在集合内
来源：http://qlc.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qfd.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cgk.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://nbx.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://bsj.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uwq.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kdm.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://syl.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://osv.jiagoushi.top

[B15] 布尔运算与取反
来源：http://bvf.yj202588.top

Py:   a and b or not c
来源：http://dwn.sxryk.cn

PHP:  $a && $b || !$c
来源：http://art.ydjk.org.cn

JS:   a && b || !c
来源：http://nsx.tianlin.xyz

TS:   a && b || !c
来源：http://cmi.sxryk.cn

Java: a && b || !c
来源：http://ehm.xinyue.icu

Go:   a && b || !c
来源：http://ovv.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://woh.shuidangran.top

C#:   a && b || !c
来源：http://psc.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ylu.yuanzhike.top

Py:   if not data: return
来源：http://yjz.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://nwz.hcnkem.com

JS:   if (!data) return;
来源：http://uqf.hongshengwenyu.top

TS:   if (!data) return;
来源：http://qpz.quarkkingdee.top

Java: if (data == null) return;
来源：http://rrx.pycfn.com

Go:   if data == nil { return }
来源：http://tcn.yangfankeji.com

Ruby: return if data.nil?
来源：http://nag.yanxiufei.cn

C#:   if (data == null) return;
来源：http://bvw.sxryk.cn

================================================================================
来源：http://ucb.yangfankeji.com

C. 函数与作用域
来源：http://mkg.fanxiaobao.xyz

================================================================================
来源：http://kui.pengpengdd.cyou

[C01] 定义函数
来源：http://jxx.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://tgv.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jgk.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://vte.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://omc.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://euh.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jnd.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://klj.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gjs.uphjek.com

[C02] 默认参数
来源：http://fsg.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://vdu.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qaq.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://whb.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://byb.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cqi.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://huj.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://olj.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://kiv.cqqwz.cn

[C03] 可变参数
来源：http://spe.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://rxr.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djn.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ygq.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jjx.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lbs.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kzd.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://vlp.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://syj.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://tdj.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lnu.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eqi.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lzv.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qtg.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://ndr.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://nju.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://vfp.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://ybc.uphjek.com

[C05] 返回多个值
来源：http://byh.chenlongwang.top

Py:   return a, b
来源：http://haz.hfpthk.cn

PHP:  return [$a, $b];
来源：http://wkw.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://qtj.mhx1999.top

TS:   return { a, b };
来源：http://zdo.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hzj.sysykeji.top

Go:   return a, b
来源：http://bds.jqgfzy.top

Ruby: return a, b
来源：http://uch.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://xdg.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://nlc.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://jbc.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://trs.cashguo.top

JS:   const square = x => x * x;
来源：http://dtm.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://oxj.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fri.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://fzy.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://kpy.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://dwu.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://rdx.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ohd.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://yut.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ahr.xuetiantiany.cn

TS:   arr.map(String)
来源：http://grn.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dbw.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qmd.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://ack.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://maq.chenjidiqi.icu

[C08] 闭包
来源：http://cye.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uya.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ibr.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fwz.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zsq.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lwz.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wyg.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fct.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iye.fehbvm.com

[C09] 递归
来源：http://hhx.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qzl.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jbu.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tef.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxl.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mop.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zbx.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pat.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tei.zhijiandao.cn

[C10] 变量作用域
来源：http://rzz.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dlk.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://icg.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iud.snrcjt.cn

TS:   同 JS
来源：http://vdf.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://asc.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://vya.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cis.cucudq.cn

C#:   块级作用域
来源：http://qlv.andypj.xyz

[C11] 模块导入与导出
来源：http://cep.vqdsnc.cn

Py:   from module import func
来源：http://czh.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ewy.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://eqh.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qxg.snrcjt.cn

Java: import java.util.List;
来源：http://ejk.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bkx.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://ymc.fengsongda.top

C#:   using System.Text;
来源：http://uin.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://hlb.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://uxp.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://hly.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://mvn.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://ifg.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tlt.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://ktn.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://nft.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://adu.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://ykb.dashuyun.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vwe.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ftt.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://est.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqv.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vgg.sufxvd.cn

Go:   func add(a, b int) int
来源：http://yxv.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dsi.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://ybv.hfpthk.cn

[C14] 泛型函数
来源：http://twk.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jrw.jyoumei.cn

PHP:  // 无泛型
来源：http://vdb.sysykeji.top

JS:   // 无泛型
来源：http://ltz.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://guq.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gnu.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zrh.hnxiangtu.top

Ruby: # 无泛型
来源：http://evy.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://crz.redwolf501.top

[C15] 解构 / 展开参数
来源：http://uld.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://npw.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://gwx.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sto.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bcu.nwbrower.top

Java: // 无解构
来源：http://imk.jiagoushi.top

Go:   // 无解构
来源：http://gkc.yj20258888.top

Ruby: a, b = pair
来源：http://xxg.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://ggl.xylfe.cn

[C16] 函数 / 方法重载
来源：http://dst.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qug.hywenlv.cn

PHP:  // 无重载
来源：http://zdj.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rmk.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://xck.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mue.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://lbf.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://qaj.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jhf.jinqigfzy.top

================================================================================
来源：http://tgk.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://qhp.cashguo.top

================================================================================
来源：http://arq.zycfv.cn

[D01] 创建数组 / 列表
来源：http://qgm.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tde.yongpay.top


<!-- 参考信息 -->