代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://ian.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nvw.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dwc.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uic.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jso.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mbc.iojbl.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bft.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://olz.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://noy.gogol.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qmy.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zyv.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bss.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://jzj.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tjm.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dea.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ady.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zcz.pengpengdd.cyou

================================================================================
来源：http://abh.aibaodan.cn

B. 流程控制
来源：http://kpr.cashguo.top

================================================================================
来源：http://dxq.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://rqx.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nos.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wvw.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vfs.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://evs.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jbx.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ugl.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://edl.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cum.guannengcc.top

[B02] 多分支 else if / elif
来源：http://jzn.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://voo.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://owf.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://irv.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnu.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ldc.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vjx.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://epw.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogi.shzxlz.cn

[B03] switch / match / case
来源：http://ete.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kxw.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://njj.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ktk.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pyj.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cow.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rau.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://htc.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rbc.xinyue.icu

[B04] for 计数循环
来源：http://upm.yj20258.top

Py:   for i in range(10): print(i)
来源：http://amp.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ico.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aix.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sht.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kry.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hws.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://qjn.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tus.cashguo.top

[B05] 遍历数组 / 列表
来源：http://idf.yonumen.top

Py:   for item in arr: print(item)
来源：http://lpi.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ctw.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://phm.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nvw.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ivm.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hom.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://lfq.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hfi.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://rmb.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://olc.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://may.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qiw.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://azo.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pwk.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xol.0kj1m.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lfr.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wbu.shangyingyoupin.top

[B07] while 循环
来源：http://dxx.xziqi.cn

Py:   while i < 10: i += 1
来源：http://nty.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sli.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://gnr.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://yog.havefunace.top

Java: while (i < 10) { i++; }
来源：http://zno.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oly.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://sub.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://ocm.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://fpn.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://rjd.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://auk.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://ydb.jinghuilouyu.cn

TS:   do { i++; } while (i < 10);
来源：http://fbf.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://eyt.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zbv.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iqw.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://ofe.hesvh.cn

[B09] break 与 continue
来源：http://egd.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nsg.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fph.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dui.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqj.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pgd.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qhr.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wsn.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvg.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://zea.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ckt.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://shb.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sud.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://poc.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bco.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kqv.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ego.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lzt.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://qdm.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://qrk.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://cnu.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wov.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lij.gogol.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cjl.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ihf.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://ent.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qgg.xuanzx.com

[B12] 跳出多层循环
来源：http://gbl.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gxo.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://hzf.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rft.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://loa.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://imj.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://utj.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mth.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ijh.snrcjt.cn

[B13] 判断是否为数字
来源：http://tlv.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://spz.ppjwa.cn

PHP:  is_numeric($x)
来源：http://hzh.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://exo.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nor.hnqzz.top

Java: x instanceof Number
来源：http://pym.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fpm.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://ucv.ydzc1.top

C#:   x is int or double or decimal
来源：http://ehh.iojbl.cn

[B14] 判断值是否在集合内
来源：http://ifp.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://itr.jinqigufen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mhr.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://jyx.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://hrx.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vfo.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gxs.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://hxi.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://riw.yangfankeji.com

[B15] 布尔运算与取反
来源：http://jmc.jinqigufen.top

Py:   a and b or not c
来源：http://sre.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://qzt.zdqjudy.top

JS:   a && b || !c
来源：http://muf.gogol.net.cn

TS:   a && b || !c
来源：http://kbz.shzxlz.cn

Java: a && b || !c
来源：http://xsi.snrcjt.cn

Go:   a && b || !c
来源：http://spr.epnwcf.com

Ruby: a && b || !c
来源：http://rfs.fehbvm.com

C#:   a && b || !c
来源：http://frs.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://qkl.aibaodan.cn

Py:   if not data: return
来源：http://qyy.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://ryv.0kj1m.cn

JS:   if (!data) return;
来源：http://uqc.chenzaomai.com

TS:   if (!data) return;
来源：http://esg.vqdsnc.cn

Java: if (data == null) return;
来源：http://mgm.yuxming.cn

Go:   if data == nil { return }
来源：http://jxd.jyoumei.cn

Ruby: return if data.nil?
来源：http://pod.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://otz.vqdsnc.cn

================================================================================
来源：http://oyt.tarul.cn

C. 函数与作用域
来源：http://jio.daxiang520.top

================================================================================
来源：http://cmn.hongshengwenyu.top

[C01] 定义函数
来源：http://iiq.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://ent.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://glu.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://ylu.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rgl.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gbx.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://uyt.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://vlh.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bve.cheryme.top

[C02] 默认参数
来源：http://awc.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://ggg.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tfr.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://oex.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qnt.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uqx.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ine.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://ekq.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://gyg.xinyue.icu

[C03] 可变参数
来源：http://djh.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://jjj.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ilc.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://efx.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dye.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rqs.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zds.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fww.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ywe.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://faq.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ilw.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hwm.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vnl.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fjk.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://pgy.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://xhe.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://ron.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://eze.tanke756.top

[C05] 返回多个值
来源：http://wxt.sweek.top

Py:   return a, b
来源：http://evo.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://goq.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ncw.hywenlv.cn

TS:   return { a, b };
来源：http://pbh.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fbw.zdqjudy.top

Go:   return a, b
来源：http://pbt.jiagoushi.top

Ruby: return a, b
来源：http://klu.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ezd.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://mcg.shuidangran.top

Py:   square = lambda x: x * x
来源：http://wxn.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hhu.ivvv.top

JS:   const square = x => x * x;
来源：http://iei.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://dbd.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qja.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://idg.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://tkp.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://nlz.sysykeji.top

[C07] 把函数作为参数传入
来源：http://vov.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ifh.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://obw.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nkl.cashguo.top

TS:   arr.map(String)
来源：http://mfm.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mix.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rhc.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://gld.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jlm.gogol.net.cn

[C08] 闭包
来源：http://lqv.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wjf.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yjw.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://asu.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rru.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nkt.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bvn.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hmw.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lgk.hywenlv.cn

[C09] 递归
来源：http://lzm.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gjd.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://etz.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fje.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nrk.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cqm.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ayf.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lmz.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hky.hnqzz.top

[C10] 变量作用域
来源：http://zfa.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bft.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bbn.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kih.sweek.top

TS:   同 JS
来源：http://nvx.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://dld.yuanzhike.top

Go:   花括号块级作用域
来源：http://txe.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://coc.kuanghao11.cn

C#:   块级作用域
来源：http://uuu.yj20258.top

[C11] 模块导入与导出
来源：http://hgp.fzhhl.top

Py:   from module import func
来源：http://qwv.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ilu.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fgr.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gew.svipenyu.cn

Java: import java.util.List;
来源：http://sxl.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://raq.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://hxl.tarul.cn

C#:   using System.Text;
来源：http://hda.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://gnj.hammf.cn

Py:   (lambda: print("run"))()
来源：http://cyw.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://ksf.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://jog.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://trb.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rjh.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://ncb.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://dmg.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hhz.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://hil.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ovv.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://twb.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sjy.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vou.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://zvk.hywenlv.cn

Go:   func add(a, b int) int
来源：http://dmt.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iar.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fcr.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://kqa.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rmy.shuidangran.top

PHP:  // 无泛型
来源：http://hqm.bbcook.cn

JS:   // 无泛型
来源：http://yvl.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qoa.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fbg.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yge.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://ugf.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zdz.cashguo.top

[C15] 解构 / 展开参数
来源：http://svb.feifeiyinyue.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qgy.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://ots.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gsl.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hkz.shzxlz.cn

Java: // 无解构
来源：http://jro.hammf.cn

Go:   // 无解构
来源：http://psm.fengsongda.top


<!-- 参考信息 -->