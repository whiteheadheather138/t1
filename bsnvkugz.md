代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fpr.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://wsp.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kdg.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://puh.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ino.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://das.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozr.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wyf.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vxn.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gsz.dashuyun.cn

[B03] switch / match / case
来源：http://xdm.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fpu.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jia.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zdw.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xjf.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ydw.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gkq.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ulr.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gds.zhixingplan.top

[B04] for 计数循环
来源：http://ayr.bjfxy.top

Py:   for i in range(10): print(i)
来源：http://dtn.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hxd.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofs.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fql.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kpa.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hxq.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://qlp.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pms.316326.xyz

[B05] 遍历数组 / 列表
来源：http://zrf.redwolf501.top

Py:   for item in arr: print(item)
来源：http://mbe.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://shx.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://ypv.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yuq.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qeo.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jnv.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://iwd.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vsc.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://ndv.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mtp.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gkb.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kro.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gse.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://esh.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xkp.0kj1m.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://poi.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yve.fktsv.cn

[B07] while 循环
来源：http://vvj.yj20258888.top

Py:   while i < 10: i += 1
来源：http://upx.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ean.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://xfo.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://otg.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://zdd.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hrn.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://ymf.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://ivn.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://ubj.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://kou.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qwz.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://pfj.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://woo.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://otv.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ybm.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://qfj.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://coj.zdbjq.cn

[B09] break 与 continue
来源：http://kfl.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bmo.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pbo.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gre.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pon.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://puy.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uvu.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uaq.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcy.cheryme.top

[B10] 遍历同时拿索引
来源：http://cmc.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xty.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dol.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ueg.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tow.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kaj.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tla.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://egc.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ezg.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://kfg.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://ebc.yj202588.top

PHP:  range(0, 10, 2);
来源：http://czh.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uzv.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qoe.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nnb.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://grf.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://urj.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mnw.c1oappe.top

[B12] 跳出多层循环
来源：http://tam.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mfh.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yyj.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rug.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qtu.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hgj.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zni.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oup.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rzi.ppjwa.cn

[B13] 判断是否为数字
来源：http://tyo.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://csf.cheryme.top

PHP:  is_numeric($x)
来源：http://okb.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://siz.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xeo.bjfxy.top

Java: x instanceof Number
来源：http://qbs.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yum.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://fbn.yfazqb.com

C#:   x is int or double or decimal
来源：http://juk.c1oappe.top

[B14] 判断值是否在集合内
来源：http://klr.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jaa.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://smv.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://zcp.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://vvd.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ydg.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fro.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://nci.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wfw.bjfxy.top

[B15] 布尔运算与取反
来源：http://vql.zhixingplan.top

Py:   a and b or not c
来源：http://mru.fengsongda.top

PHP:  $a && $b || !$c
来源：http://dna.hywenlv.cn

JS:   a && b || !c
来源：http://nue.zycfv.cn

TS:   a && b || !c
来源：http://gnu.yueranfly.top

Java: a && b || !c
来源：http://fgd.hfpthk.cn

Go:   a && b || !c
来源：http://rei.cucudq.cn

Ruby: a && b || !c
来源：http://yoz.guowangkeji.top

C#:   a && b || !c
来源：http://oai.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://zhu.redwolf501.top

Py:   if not data: return
来源：http://gyj.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://hrp.chenlongwang.top

JS:   if (!data) return;
来源：http://xao.nanxinkj.top

TS:   if (!data) return;
来源：http://vrd.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://fgu.shzxlz.cn

Go:   if data == nil { return }
来源：http://kej.yueranfly.top

Ruby: return if data.nil?
来源：http://cal.yanxiufei.cn

C#:   if (data == null) return;
来源：http://hwz.nanxinkj.top

================================================================================
来源：http://eql.ydjk.org.cn

C. 函数与作用域
来源：http://dvs.jinqigufen.top

================================================================================
来源：http://njk.hysaishi.cn

[C01] 定义函数
来源：http://tvz.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://hre.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wrp.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://qgt.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://msr.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://doh.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cqa.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://jqs.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://imn.xylfe.cn

[C02] 默认参数
来源：http://kei.hammf.cn

Py:   def greet(name="World"): return name
来源：http://mcu.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dzj.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://kzt.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qbt.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eox.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://acc.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://ayz.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://mzt.zhaomingkeji.xyz

[C03] 可变参数
来源：http://yli.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://nzf.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lvi.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tei.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypv.aibaodan.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cfu.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wqa.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://ncw.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kaf.yfazqb.com

[C04] 命名参数 / 关键字参数
来源：http://wql.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://spn.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wuh.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xyd.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zhq.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://cac.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://cnd.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://tnt.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://sza.zdqjudy.top

[C05] 返回多个值
来源：http://ipk.jlsjyb.cn

Py:   return a, b
来源：http://eft.jiagoushi.top

PHP:  return [$a, $b];
来源：http://bjw.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dtz.hfpthk.cn

TS:   return { a, b };
来源：http://sab.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kxy.hnqzz.top

Go:   return a, b
来源：http://erc.jqgufenzy.top

Ruby: return a, b
来源：http://wjs.zhaomingkeji.xyz

C#:   return (a, b);              // ValueTuple
来源：http://itu.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://dze.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://jgn.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://szr.xziqi.cn

JS:   const square = x => x * x;
来源：http://enr.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://iyx.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rbd.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://lku.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://uuq.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vsp.gzhubu.top

[C07] 把函数作为参数传入
来源：http://irg.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vhl.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://xpm.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nze.smart0.xyz

TS:   arr.map(String)
来源：http://rkp.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://soc.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cay.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://yty.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://alk.nwbrower.top

[C08] 闭包
来源：http://jnc.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bdx.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qjo.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mld.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ulr.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jwl.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qcu.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jum.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://djp.iojbl.cn

[C09] 递归
来源：http://odg.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bbp.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://avo.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzr.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xwe.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ket.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gsz.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ijv.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dte.aizwys.cn

[C10] 变量作用域
来源：http://vis.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ucc.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pis.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iyw.fehbvm.com

TS:   同 JS
来源：http://klf.vehdjk.com

Java: 方法内为块级作用域
来源：http://oko.aibaodan.cn

Go:   花括号块级作用域
来源：http://dcr.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qny.pengpengdd.cyou

C#:   块级作用域
来源：http://one.sufxvd.cn

[C11] 模块导入与导出
来源：http://wfh.hcnkem.com

Py:   from module import func
来源：http://zvx.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fkl.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vdh.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wdi.kuanghao11.cn

Java: import java.util.List;
来源：http://kum.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gxk.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://pnm.zhongyouzk.top

C#:   using System.Text;
来源：http://tap.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://qgv.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://zsi.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://njm.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://znt.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://qfb.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cfp.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://hrt.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://pxg.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ozb.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://lga.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rzy.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ehc.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ykn.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ktk.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://sho.sufxvd.cn

Go:   func add(a, b int) int
来源：http://dhh.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://emz.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://nmr.tarul.cn

[C14] 泛型函数
来源：http://oxw.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aok.andypj.xyz

PHP:  // 无泛型
来源：http://dgw.havefunace.top

JS:   // 无泛型
来源：http://azr.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kii.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wgb.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mdy.hcnkem.com

Ruby: # 无泛型
来源：http://xfp.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uca.jianghu66.top

[C15] 解构 / 展开参数
来源：http://ysz.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ulh.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://tnn.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://clo.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kec.cashguo.top

Java: // 无解构
来源：http://gyo.iojbl.cn

Go:   // 无解构
来源：http://nxn.tianlin.xyz

Ruby: a, b = pair
来源：http://sie.xylfe.cn

C#:   var (a, b) = pair;
来源：http://zap.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://uzf.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tnw.bbcook.cn

PHP:  // 无重载
来源：http://xsa.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wdb.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://vkj.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gto.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://hvj.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://xqd.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jdf.xziqi.cn

================================================================================
来源：http://mdo.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://lxp.zhiwuduotai.top

================================================================================
来源：http://byx.ydzc1.top

[D01] 创建数组 / 列表
来源：http://tps.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sok.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kel.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://abx.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gza.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qah.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://ryo.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://rmc.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qse.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://vef.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gva.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://arx.guannengcc.top

JS:   arr.push(4);
来源：http://spt.yangfankeji.com

TS:   arr.push(4);
来源：http://bmi.cdnleiting.top


<!-- 参考信息 -->