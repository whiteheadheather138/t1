代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vzv.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://moo.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ckb.shzxlz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ier.yonumen.top

[A26] 类型转换总览
来源：http://ewk.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pvj.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cxq.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://edq.hesvh.cn

TS:   Number() String() Boolean() x as number
来源：http://jur.nwbrower.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ebo.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://swa.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://zlv.svipenyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xij.meibo888.top

================================================================================
来源：http://ikt.yj20258.top

B. 流程控制
来源：http://wfz.epnwcf.com

================================================================================
来源：http://tvw.yueranfly.top

[B01] 条件判断 if / else
来源：http://vqb.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yrs.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hhc.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mvz.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cac.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://knt.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hho.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rfy.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wua.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://qax.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qkh.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mmp.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xui.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yat.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydx.yfazqb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uid.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tbr.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfn.ydjk.org.cn

[B03] switch / match / case
来源：http://qgu.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ljh.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ugl.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dcu.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vcj.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lsi.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ftb.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vov.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://awa.yanxiufei.cn

[B04] for 计数循环
来源：http://buj.uphjek.com

Py:   for i in range(10): print(i)
来源：http://fho.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ifr.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://haw.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mvj.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mvm.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uzk.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://hws.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dbk.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://gna.birdmap.top

Py:   for item in arr: print(item)
来源：http://awa.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://krx.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jge.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eqf.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ysa.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fsz.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://zek.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qeg.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://tzd.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bwz.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://swi.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sod.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zvm.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gla.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rzl.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dpq.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tyd.meibo888.top

[B07] while 循环
来源：http://eab.52xcode.cn

Py:   while i < 10: i += 1
来源：http://kxr.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://pgp.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://qoq.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://bvl.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://nqu.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yih.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://puu.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://dsi.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://com.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://hil.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://prj.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://wzr.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://ycd.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://fdr.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xex.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://nha.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://fqz.hongshengwenyu.top

[B09] break 与 continue
来源：http://qxx.hesvh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vfo.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kdt.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihv.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pkp.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whh.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://evn.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lya.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evu.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://jon.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lux.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dtp.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jyh.bjfxy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dgo.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dlz.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vkt.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vkx.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iai.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://pye.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://hhk.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://mng.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://urx.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyb.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cky.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qlr.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://frx.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xqn.yj20258888.top

[B12] 跳出多层循环
来源：http://xvv.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://xov.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://doz.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://auc.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fal.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wuc.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cpv.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mwn.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ohi.tian-w.cn

[B13] 判断是否为数字
来源：http://vvk.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://dre.sysykeji.top

PHP:  is_numeric($x)
来源：http://xvt.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rua.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qxt.guowangkeji.top

Java: x instanceof Number
来源：http://len.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kjc.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://atx.andypj.xyz

C#:   x is int or double or decimal
来源：http://dib.daria6918.cn

[B14] 判断值是否在集合内
来源：http://eiv.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bem.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bml.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://qac.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://uny.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hmj.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tuh.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://bla.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vjo.jianghu66.top

[B15] 布尔运算与取反
来源：http://njn.sjlbkw.cn

Py:   a and b or not c
来源：http://iwx.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://kyl.smart0.xyz

JS:   a && b || !c
来源：http://mpr.mhx1999.top

TS:   a && b || !c
来源：http://iiw.gzhubu.top

Java: a && b || !c
来源：http://isi.jinqigfzy.top

Go:   a && b || !c
来源：http://hzs.ydzc1.top

Ruby: a && b || !c
来源：http://ivn.hnxiangtu.top

C#:   a && b || !c
来源：http://wjz.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dtk.uphjek.com

Py:   if not data: return
来源：http://rcu.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://gub.pengpengdd.cyou

JS:   if (!data) return;
来源：http://diu.ydjk.org.cn

TS:   if (!data) return;
来源：http://bim.yuxming.cn

Java: if (data == null) return;
来源：http://jtu.gzhubu.top

Go:   if data == nil { return }
来源：http://zty.bjfxy.top

Ruby: return if data.nil?
来源：http://nrs.dianchejie.cn

C#:   if (data == null) return;
来源：http://bvt.mhx1999.top

================================================================================
来源：http://kiy.tanke756.top

C. 函数与作用域
来源：http://znb.quarkkingdee.top

================================================================================
来源：http://cpt.wangdashe.top

[C01] 定义函数
来源：http://wnw.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://rdk.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bun.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://shk.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kaa.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dcb.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cqw.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://qda.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nfi.chenzaomai.com

[C02] 默认参数
来源：http://noo.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://ulb.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hrk.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://ofg.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://htb.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ufm.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fkq.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://qtz.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://jzc.yfazqb.com

[C03] 可变参数
来源：http://zxe.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://ltr.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pdq.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rba.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zzg.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pkw.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qze.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://hfm.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pol.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://qcn.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aeq.jinyuanbaomall.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://thg.jinghuilouyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://psd.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ajj.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://vbc.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://baw.andypj.xyz

Ruby: f(a: 1, b: 2)
来源：http://ubz.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://epw.yongpay.top

[C05] 返回多个值
来源：http://ovx.gzhubu.top

Py:   return a, b
来源：http://ddf.chenzaomai.com

PHP:  return [$a, $b];
来源：http://pen.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://unr.0kj1m.cn

TS:   return { a, b };
来源：http://xal.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lje.yueranfly.top

Go:   return a, b
来源：http://tne.pycfn.com

Ruby: return a, b
来源：http://gvg.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://fer.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://pxu.xziqi.cn

Py:   square = lambda x: x * x
来源：http://yjn.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xdv.zdbjq.cn

JS:   const square = x => x * x;
来源：http://lew.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://tup.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fbu.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://jwm.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://mjd.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://trp.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://wzw.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kmv.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wsa.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cga.0kj1m.cn

TS:   arr.map(String)
来源：http://qnj.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jqh.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mco.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://yrg.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ivi.cqqwz.cn

[C08] 闭包
来源：http://ntr.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dnl.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kbr.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://clb.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ebr.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sjk.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jku.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zro.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ano.hnxiangtu.top

[C09] 递归
来源：http://yiv.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sbb.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iyk.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qev.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lmv.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zxn.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ydw.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xkm.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blt.yuanzhike.top

[C10] 变量作用域
来源：http://ttr.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pyt.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qgm.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gsb.cucudq.cn

TS:   同 JS
来源：http://aql.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://eeh.smart0.xyz

Go:   花括号块级作用域
来源：http://hjr.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ast.yuxming.cn

C#:   块级作用域
来源：http://nal.zhengqikj.top

[C11] 模块导入与导出
来源：http://ugj.shanyushiyangkeji.top

Py:   from module import func
来源：http://jul.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jyg.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://fyr.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mjc.yj20258.top

Java: import java.util.List;
来源：http://zkr.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aqd.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://xho.cheryme.top

C#:   using System.Text;
来源：http://bla.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://rka.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://ymk.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://lsg.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://slk.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://itv.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zdw.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://eij.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://mti.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://igm.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://xre.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uee.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jcj.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tog.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nqr.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://wmn.guowangkeji.top

Go:   func add(a, b int) int
来源：http://jig.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gia.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://gxi.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://dqo.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://txi.sufxvd.cn

PHP:  // 无泛型
来源：http://fnw.yuanzhike.top

JS:   // 无泛型
来源：http://lki.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qgs.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pkl.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zvc.jqgufenzy.top

Ruby: # 无泛型
来源：http://esr.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zmu.xuanzx.com

[C15] 解构 / 展开参数
来源：http://wfq.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://snd.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://uup.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rif.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://omz.yanxiufei.cn

Java: // 无解构
来源：http://jbn.dashuyun.cn

Go:   // 无解构
来源：http://vmx.chenzaomai.com

Ruby: a, b = pair
来源：http://jhh.yueranfly.top

C#:   var (a, b) = pair;
来源：http://vvp.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://lef.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qug.gotoacloud.top


<!-- 参考信息 -->