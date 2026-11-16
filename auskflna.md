代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mxz.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pil.svipenyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://efl.redwolf501.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hba.xinyue.icu

[A26] 类型转换总览
来源：http://dyu.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dpj.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wsl.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ewr.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://hqh.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hfv.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wmt.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nro.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gun.vehdjk.com

================================================================================
来源：http://lnp.zdqjudy.top

B. 流程控制
来源：http://xur.zycfv.cn

================================================================================
来源：http://ngl.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://psv.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://tyi.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wlh.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jyx.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cym.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kby.shuidangran.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vjm.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ydh.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nkd.cheryme.top

[B02] 多分支 else if / elif
来源：http://juj.hfpthk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jkn.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rgz.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdw.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://spi.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ebh.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tuy.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fem.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cab.jinqigufen.top

[B03] switch / match / case
来源：http://ffq.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ofs.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tkt.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qny.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pmy.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wlt.9152youxi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vib.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tpp.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gpy.meibo888.top

[B04] for 计数循环
来源：http://wpb.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://yqg.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xna.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eiy.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ojr.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://htf.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ast.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://ikc.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ufs.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://vkk.52xcode.cn

Py:   for item in arr: print(item)
来源：http://hum.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sco.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://psu.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://eux.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uag.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://atu.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://rde.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://brg.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://dlt.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xfq.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zxs.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dpb.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpa.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lsg.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cuf.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://efq.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xmd.hfpthk.cn

[B07] while 循环
来源：http://qvb.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://ngb.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://fhs.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://tdl.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://rrw.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://uuf.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ryn.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://htm.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://vbo.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://zca.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://wbm.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cox.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://qjd.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://evg.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://psk.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://prz.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://gta.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://jgq.quarkkingdee.top

[B09] break 与 continue
来源：http://rro.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ksn.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cwu.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hso.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://alz.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjm.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kro.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wbx.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhh.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://nhz.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wau.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lok.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dju.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://chp.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vpe.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://smo.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vxv.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ilb.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://zmj.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://otk.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://fmj.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://guq.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cwe.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qoy.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mhg.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://vmh.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wbn.ppjwa.cn

[B12] 跳出多层循环
来源：http://dgj.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://evu.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://byx.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kyy.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qwo.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://opy.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vee.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ksl.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gxp.hfpthk.cn

[B13] 判断是否为数字
来源：http://xup.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://jra.epnwcf.com

PHP:  is_numeric($x)
来源：http://nlm.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rei.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uuv.birdmap.top

Java: x instanceof Number
来源：http://fhr.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ngu.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://cas.sysykeji.top

C#:   x is int or double or decimal
来源：http://ffq.sweek.top

[B14] 判断值是否在集合内
来源：http://ioy.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ebg.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qnj.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://zzu.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://urb.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://oph.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cvn.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uhi.hnxiangtu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oru.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://otk.aibaodan.cn

Py:   a and b or not c
来源：http://pmd.epnwcf.com

PHP:  $a && $b || !$c
来源：http://zqj.0kj1m.cn

JS:   a && b || !c
来源：http://dhj.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://ptg.yvedp.cn

Java: a && b || !c
来源：http://ayq.316326.xyz

Go:   a && b || !c
来源：http://nfw.zhiwuduotai.top

Ruby: a && b || !c
来源：http://fmz.yj20258.top

C#:   a && b || !c
来源：http://gfo.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://ohh.fengsongda.top

Py:   if not data: return
来源：http://pst.yj202588.top

PHP:  if (!$data) { return; }
来源：http://irg.xuanzx.com

JS:   if (!data) return;
来源：http://scz.ydzc1.top

TS:   if (!data) return;
来源：http://tzt.ybcxt.top

Java: if (data == null) return;
来源：http://hmg.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://eei.shuidangran.top

Ruby: return if data.nil?
来源：http://waj.dashuyun.cn

C#:   if (data == null) return;
来源：http://tzs.nwbrower.top

================================================================================
来源：http://lta.yj202588.top

C. 函数与作用域
来源：http://prf.hammf.cn

================================================================================
来源：http://xby.zycfv.cn

[C01] 定义函数
来源：http://cfo.pycfn.com

Py:   def add(a, b): return a + b
来源：http://rdo.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tra.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://zpq.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqk.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://she.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://ywr.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://plu.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lfz.jinqigufen.top

[C02] 默认参数
来源：http://txn.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://soj.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mkj.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://quz.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hqa.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ezb.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vtu.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://kze.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://dzd.quarkkingdee.top

[C03] 可变参数
来源：http://zlz.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://ozb.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bxt.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mnq.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dyz.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tme.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pnf.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://txl.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://trf.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://xhj.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wsk.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kqi.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fto.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wmp.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://cmv.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://qlj.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://zte.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://ofk.tian-w.cn

[C05] 返回多个值
来源：http://val.zhongyouzk.top

Py:   return a, b
来源：http://cmg.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://kgq.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kbe.zhixingplan.top

TS:   return { a, b };
来源：http://pmg.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://osi.xuanzx.com

Go:   return a, b
来源：http://pfv.zdbjq.cn

Ruby: return a, b
来源：http://scf.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://spo.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://dbw.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://xkd.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fzp.gzhubu.top

JS:   const square = x => x * x;
来源：http://kbe.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://gxq.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://beg.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oho.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://dfm.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://muy.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://mwy.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lxa.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://fpr.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://epf.ybcxt.top

TS:   arr.map(String)
来源：http://heg.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fhp.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kag.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://xdl.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xkc.smart0.xyz

[C08] 闭包
来源：http://yiu.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oxg.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fkk.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://skw.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rif.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zbj.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hco.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://geb.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lcm.yuanzhike.top

[C09] 递归
来源：http://oay.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://swy.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zey.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ewa.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uuk.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hho.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oxp.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://njw.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tgx.ybcxt.top

[C10] 变量作用域
来源：http://set.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tvt.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sqq.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nsb.hcnkem.com

TS:   同 JS
来源：http://zbz.hysaishi.cn

Java: 方法内为块级作用域
来源：http://tsl.zhixingplan.top

Go:   花括号块级作用域
来源：http://pbm.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rws.cqqwz.cn

C#:   块级作用域
来源：http://ykj.aibaodan.cn

[C11] 模块导入与导出
来源：http://xgh.jqgfzy.top

Py:   from module import func
来源：http://kbu.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://htj.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vhd.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://idd.jyoumei.cn

Java: import java.util.List;
来源：http://ojj.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://crz.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://lab.cheryme.top

C#:   using System.Text;
来源：http://gbi.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://crv.havefunace.top

Py:   (lambda: print("run"))()
来源：http://csx.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://wnr.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://uzq.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://kff.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://twp.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://bfi.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://rqd.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fwd.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://zjk.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aju.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rca.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://org.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://usq.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://nds.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://raa.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://upy.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://znz.gotoacloud.top

[C14] 泛型函数
来源：http://mug.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lbv.wangdashe.top

PHP:  // 无泛型
来源：http://jdn.cucudq.cn

JS:   // 无泛型
来源：http://dqf.hysaishi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eow.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ckj.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jxv.pengpengdd.cyou

Ruby: # 无泛型
来源：http://ttr.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rah.meibo888.top

[C15] 解构 / 展开参数
来源：http://fgo.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iif.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://fip.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dgu.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wrt.hfpthk.cn

Java: // 无解构
来源：http://tcx.havefunace.top

Go:   // 无解构
来源：http://mns.c1oappe.top

Ruby: a, b = pair
来源：http://vse.yuxming.cn

C#:   var (a, b) = pair;
来源：http://kaz.cucudq.cn

[C16] 函数 / 方法重载
来源：http://gnt.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vol.fzhhl.top


<!-- 参考信息 -->