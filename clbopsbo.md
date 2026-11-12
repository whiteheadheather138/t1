代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://ghj.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jzc.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ekz.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://all.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://myg.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://abu.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://zog.yangfankeji.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nyi.uphjek.com

[A26] 类型转换总览
来源：http://bpa.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eot.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xuo.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pgv.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://ywo.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://puv.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gfj.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://fyf.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mig.cashguo.top

================================================================================
来源：http://zob.9152youxi.cn

B. 流程控制
来源：http://nzs.chenlongwang.top

================================================================================
来源：http://sus.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://prh.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://otb.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://exb.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eiu.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://moo.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qzh.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mxo.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wjv.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ctm.hcnkem.com

[B02] 多分支 else if / elif
来源：http://vdf.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dbj.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xso.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvn.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rfc.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukd.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://meb.meibo888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oxe.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://esb.daxiang520.top

[B03] switch / match / case
来源：http://zbh.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cke.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aan.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xwv.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgw.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yqy.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zcd.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://emn.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zwk.yj20258.top

[B04] for 计数循环
来源：http://pqd.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://igz.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rhl.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvo.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofq.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zne.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://msi.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://ubr.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pxr.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://lrl.yj202588.top

Py:   for item in arr: print(item)
来源：http://gjf.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rol.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://fjz.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://uwu.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://acz.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sme.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://bad.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qlq.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://oxt.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ebe.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pus.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pby.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fdj.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://thi.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xpo.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kwg.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dpb.zhixingplan.top

[B07] while 循环
来源：http://feb.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://ptp.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://ycr.chenjidiqi.icu

JS:   while (i < 10) { i++; }
来源：http://zqg.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://njn.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://zlx.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vtm.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://arl.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://mig.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://gqw.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://ovh.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lyu.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://tws.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://zsd.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://mvv.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ctm.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://qbh.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://fpo.cashguo.top

[B09] break 与 continue
来源：http://rex.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dag.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ums.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fxf.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fju.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sfp.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cyb.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qzp.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjr.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://jze.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cac.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ocy.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hpu.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://beq.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ghe.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aen.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dkv.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xdd.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://scw.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://fzp.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://ogv.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vuw.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bxe.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iub.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://klh.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://zvx.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vfk.zhengqikj.top

[B12] 跳出多层循环
来源：http://wyn.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://idl.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lck.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wsu.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nwz.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://skw.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cfr.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://utr.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kva.aizwys.cn

[B13] 判断是否为数字
来源：http://dck.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://wpx.sweek.top

PHP:  is_numeric($x)
来源：http://txp.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mxx.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qlx.hnxiangtu.top

Java: x instanceof Number
来源：http://jag.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://teb.hcnkem.com

Ruby: x.is_a?(Numeric)
来源：http://oum.wangdashe.top

C#:   x is int or double or decimal
来源：http://sgi.vehdjk.com

[B14] 判断值是否在集合内
来源：http://hyr.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qkz.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kit.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://ysu.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://tvu.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://mnz.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zci.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wjb.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bhj.pycfn.com

[B15] 布尔运算与取反
来源：http://cez.chenjidiqi.icu

Py:   a and b or not c
来源：http://bcq.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://ons.ydjk.org.cn

JS:   a && b || !c
来源：http://wsb.tian-w.cn

TS:   a && b || !c
来源：http://jub.jiagoushi.top

Java: a && b || !c
来源：http://her.zycfv.cn

Go:   a && b || !c
来源：http://fnu.redwolf501.top

Ruby: a && b || !c
来源：http://boz.chenlongwang.top

C#:   a && b || !c
来源：http://lsq.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nsa.jyoumei.cn

Py:   if not data: return
来源：http://ark.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://vsz.bjfxy.top

JS:   if (!data) return;
来源：http://ewk.wangshuangyany.cn

TS:   if (!data) return;
来源：http://dgq.feifeiyinyue.top

Java: if (data == null) return;
来源：http://qev.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://jvy.cucudq.cn

Ruby: return if data.nil?
来源：http://wmx.52xcode.cn

C#:   if (data == null) return;
来源：http://mcj.hongshengwenyu.top

================================================================================
来源：http://zzz.aibaodan.cn

C. 函数与作用域
来源：http://mel.hammf.cn

================================================================================
来源：http://ftp.zhaomingkeji.xyz

[C01] 定义函数
来源：http://ioo.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://ies.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hmt.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://tyd.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fni.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jpa.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://tfl.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://zdn.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lks.pycfn.com

[C02] 默认参数
来源：http://zud.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://ads.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yzu.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://hra.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cbi.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xvq.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bds.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://xib.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://qnq.iojbl.cn

[C03] 可变参数
来源：http://hgg.kuanghao11.cn

Py:   def total(*args): return sum(args)
来源：http://ojz.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uxa.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ukx.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://abp.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nft.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qmp.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://fwe.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iww.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://zdj.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dnm.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oth.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ksm.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wdl.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://fdz.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://fqu.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://fqc.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://aat.vqdsnc.cn

[C05] 返回多个值
来源：http://jtq.quarkkingdee.top

Py:   return a, b
来源：http://kao.xinyue.icu

PHP:  return [$a, $b];
来源：http://nzk.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zzl.yonumen.top

TS:   return { a, b };
来源：http://wxv.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://thr.ppjwa.cn

Go:   return a, b
来源：http://skg.hnxiangtu.top

Ruby: return a, b
来源：http://ahy.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://ohf.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://pzq.smart0.xyz

Py:   square = lambda x: x * x
来源：http://fsf.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ith.tianlin.xyz

JS:   const square = x => x * x;
来源：http://xkd.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://vfx.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vzl.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://nnv.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://ptu.havefunace.top

C#:   Func<int, int> square = x => x * x;
来源：http://czq.yj202588.top

[C07] 把函数作为参数传入
来源：http://off.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lfu.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://nof.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ezc.jyoumei.cn

TS:   arr.map(String)
来源：http://lsl.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://brd.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uwr.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://jut.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://idx.cheryme.top

[C08] 闭包
来源：http://gya.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dqq.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wjt.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oeu.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jqp.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bgj.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kwj.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tdr.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kyt.sweek.top

[C09] 递归
来源：http://mry.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ejc.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tqc.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://naf.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oqb.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sed.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uvf.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iqf.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ufv.jqgfzy.top

[C10] 变量作用域
来源：http://wnq.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pnb.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qjp.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cxw.0kj1m.cn

TS:   同 JS
来源：http://xak.uphjek.com

Java: 方法内为块级作用域
来源：http://iaj.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://xln.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zww.sufxvd.cn

C#:   块级作用域
来源：http://lca.quarkkingdee.top

[C11] 模块导入与导出
来源：http://ufi.hcnkem.com

Py:   from module import func
来源：http://wvk.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://irh.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gtb.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nmq.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://agj.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ctv.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://nqe.xinyue.icu

C#:   using System.Text;
来源：http://bds.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://qeq.hammf.cn

Py:   (lambda: print("run"))()
来源：http://hkh.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://peo.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://ues.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://dxz.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ubh.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://qzl.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://dlu.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://sjp.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://psp.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tmk.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nlk.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://phm.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pjk.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fow.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://pib.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ytx.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cir.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://clz.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jlb.tarul.cn

PHP:  // 无泛型
来源：http://ayd.sweek.top

JS:   // 无泛型
来源：http://kvi.hysaishi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ujx.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vpf.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rga.sysykeji.top

Ruby: # 无泛型
来源：http://noz.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://env.smart0.xyz

[C15] 解构 / 展开参数
来源：http://zzb.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kyc.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://fqu.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ijl.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ozi.ywan-chungtsiang.top

Java: // 无解构
来源：http://xnt.zhijiandao.cn

Go:   // 无解构
来源：http://ifr.shuidangran.top


<!-- 参考信息 -->