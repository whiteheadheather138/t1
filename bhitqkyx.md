代发 wailian999

[A26] 类型转换总览
来源：http://dqc.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://egv.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gsl.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aax.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://jva.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ywb.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xea.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://era.aizwys.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pmo.xuetiantiany.cn

================================================================================
来源：http://ujt.yj202588.top

B. 流程控制
来源：http://kxw.fzhhl.top

================================================================================
来源：http://ptg.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://dwl.cdnleiting.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ode.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jlu.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dvz.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lvg.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://tsk.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gic.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mts.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sdf.zhijiandao.cn

[B02] 多分支 else if / elif
来源：http://nnr.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bew.sjlbkw.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nno.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdt.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ull.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khz.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ihd.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vpl.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zvm.yfazqb.com

[B03] switch / match / case
来源：http://anc.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gtc.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dkt.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zvf.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lmz.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gec.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://awj.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xrt.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nsb.svipenyu.cn

[B04] for 计数循环
来源：http://ywa.meibo888.top

Py:   for i in range(10): print(i)
来源：http://hdd.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vuv.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljn.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tvb.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ufl.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://klr.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://hrq.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mhf.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://wks.xuanzx.com

Py:   for item in arr: print(item)
来源：http://cii.ppjwa.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rgw.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://opp.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uyx.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yix.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dpx.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://dhy.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dsd.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://arh.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dmk.iojbl.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ujg.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hhh.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cow.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dva.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bdy.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tqj.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vup.jinqigufen.top

[B07] while 循环
来源：http://hqz.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://qjl.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://bex.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://tnv.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://byj.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://pys.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vcf.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://lfb.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://xfo.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://vdu.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://hiq.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bpe.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://alc.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://ydq.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://vgy.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ztd.tanke756.top

Ruby: begin; i += 1; end while i < 10
来源：http://mia.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://ssi.gogol.net.cn

[B09] break 与 continue
来源：http://bbn.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qzb.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ebz.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lwj.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yti.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgr.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://akr.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://alx.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqt.xylfe.cn

[B10] 遍历同时拿索引
来源：http://qdg.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fsp.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hxh.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wpg.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vix.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tmt.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xzw.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gbl.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://etq.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://wwr.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://smy.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://dct.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjn.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nmi.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://drf.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jjh.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://haf.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://biq.cdnleiting.top

[B12] 跳出多层循环
来源：http://chs.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jte.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://etv.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nvc.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gct.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rlk.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bad.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tbr.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vug.hnxiangtu.top

[B13] 判断是否为数字
来源：http://kys.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://jge.hcnkem.com

PHP:  is_numeric($x)
来源：http://ddn.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqz.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bgy.epnwcf.com

Java: x instanceof Number
来源：http://efi.yuxming.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oba.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://kpc.hfpthk.cn

C#:   x is int or double or decimal
来源：http://ols.hammf.cn

[B14] 判断值是否在集合内
来源：http://tfs.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azg.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jxo.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://aht.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://mnl.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://kfg.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nfh.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://zdp.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uvm.xinyue.icu

[B15] 布尔运算与取反
来源：http://xqw.316326.xyz

Py:   a and b or not c
来源：http://chj.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://dqa.svipenyu.cn

JS:   a && b || !c
来源：http://qfh.cdnleiting.top

TS:   a && b || !c
来源：http://ojr.fengsongda.top

Java: a && b || !c
来源：http://omz.daxiang520.top

Go:   a && b || !c
来源：http://ezx.jyoumei.cn

Ruby: a && b || !c
来源：http://isq.yvedp.cn

C#:   a && b || !c
来源：http://jnv.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qty.xziqi.cn

Py:   if not data: return
来源：http://ept.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://vkv.c1oappe.top

JS:   if (!data) return;
来源：http://htj.aizwys.cn

TS:   if (!data) return;
来源：http://qip.cdnleiting.top

Java: if (data == null) return;
来源：http://wla.fengsongda.top

Go:   if data == nil { return }
来源：http://rox.epnwcf.com

Ruby: return if data.nil?
来源：http://ppz.sjlbkw.cn

C#:   if (data == null) return;
来源：http://lkm.mhx1999.top

================================================================================
来源：http://sap.quarkkingdee.top

C. 函数与作用域
来源：http://ija.guowangkeji.top

================================================================================
来源：http://ouj.ydzc1.top

[C01] 定义函数
来源：http://hgl.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://snm.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vyc.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://jjl.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fiy.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rtj.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://fda.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://axz.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ylx.hnqzz.top

[C02] 默认参数
来源：http://pdd.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://tqe.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uru.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vfs.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fnl.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://izs.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yoo.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://wjc.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://ofx.yj20258.top

[C03] 可变参数
来源：http://pec.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://vxy.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gig.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aze.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hkp.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iid.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tmj.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://cue.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kjt.yfazqb.com

[C04] 命名参数 / 关键字参数
来源：http://ymh.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qkh.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://frr.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qtl.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://shx.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://ksx.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://ygx.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://vyx.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://anx.xuetiantiany.cn

[C05] 返回多个值
来源：http://tlj.fanxiaobao.xyz

Py:   return a, b
来源：http://rsr.yonumen.top

PHP:  return [$a, $b];
来源：http://wur.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://cyn.cqqwz.cn

TS:   return { a, b };
来源：http://spp.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oxg.birdmap.top

Go:   return a, b
来源：http://dir.yuanzhike.top

Ruby: return a, b
来源：http://svf.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://ptt.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://pac.yuxming.cn

Py:   square = lambda x: x * x
来源：http://paq.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qvw.zycfv.cn

JS:   const square = x => x * x;
来源：http://nhh.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://hbm.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ahn.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nqw.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://oyk.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://thq.xylfe.cn

[C07] 把函数作为参数传入
来源：http://vrk.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sae.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://iyr.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mvr.yfazqb.com

TS:   arr.map(String)
来源：http://izr.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oyi.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mat.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://nhw.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nfa.hfpthk.cn

[C08] 闭包
来源：http://yrq.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qtc.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uzj.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://htj.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ukw.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bjd.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://whn.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zrw.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oow.fanxiaobao.xyz

[C09] 递归
来源：http://btr.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpt.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mnt.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://icl.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qdj.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tyu.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jeg.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lhd.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://anl.svipenyu.cn

[C10] 变量作用域
来源：http://szo.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gfn.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gox.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://csc.xylfe.cn

TS:   同 JS
来源：http://jqa.9152youxi.cn

Java: 方法内为块级作用域
来源：http://pzc.hnqzz.top

Go:   花括号块级作用域
来源：http://wqn.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uvc.quarkkingdee.top

C#:   块级作用域
来源：http://xwy.yuanzhike.top

[C11] 模块导入与导出
来源：http://ago.jinqigfzy.top

Py:   from module import func
来源：http://nxq.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pkj.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://idm.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mhh.ppjwa.cn

Java: import java.util.List;
来源：http://neh.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bbp.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://vzf.ppjwa.cn

C#:   using System.Text;
来源：http://wjo.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://opg.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://kur.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://vtq.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://mub.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://lly.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eyh.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://wyx.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://tft.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://klc.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://qvn.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://onu.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bis.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://php.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xwr.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://hnc.andypj.xyz

Go:   func add(a, b int) int
来源：http://vqp.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://znh.shanyushiyangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://mfz.yonumen.top

[C14] 泛型函数
来源：http://vls.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xjx.bbcook.cn

PHP:  // 无泛型
来源：http://vko.guowangkeji.top

JS:   // 无泛型
来源：http://guh.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eyo.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ztb.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dco.pycfn.com

Ruby: # 无泛型
来源：http://ryn.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xmj.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://ilk.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pvf.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://tks.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nyr.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fdc.jinqigfzy.top

Java: // 无解构
来源：http://daz.daria6918.cn

Go:   // 无解构
来源：http://pic.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://iiu.havefunace.top

C#:   var (a, b) = pair;
来源：http://itc.yj20258888.top

[C16] 函数 / 方法重载
来源：http://sjb.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ukg.redwolf501.top

PHP:  // 无重载
来源：http://brv.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bdw.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://dys.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://jlw.sjlbkw.cn


<!-- 参考信息 -->