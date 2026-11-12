代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xyz.uphjek.com

[B02] 多分支 else if / elif
来源：http://efg.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dkx.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dyd.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqy.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmi.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hpw.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bys.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zaw.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ruy.hnxiangtu.top

[B03] switch / match / case
来源：http://ubt.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jyk.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dbs.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zeh.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjs.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tbe.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hxh.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hux.xylfe.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nli.jinghuilouyu.cn

[B04] for 计数循环
来源：http://otv.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://vhd.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vwc.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iad.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zmz.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vzp.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iki.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://ibt.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wxv.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://tye.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://ohq.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uyp.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rqw.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rez.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lqc.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fgi.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://mup.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ctf.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://cyr.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nvn.snrcjt.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://byl.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://prq.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ken.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mfw.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xxc.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hvx.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rni.svipenyu.cn

[B07] while 循环
来源：http://cjq.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://fss.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hsi.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://uwm.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://hsh.meibo888.top

Java: while (i < 10) { i++; }
来源：http://liu.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oxq.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://dsc.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://lgl.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://ebe.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ebe.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dga.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://peu.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://urt.yonumen.top

Java: do { i++; } while (i < 10);
来源：http://ozj.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://lee.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://zzq.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://qlc.ppjwa.cn

[B09] break 与 continue
来源：http://mra.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kib.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ued.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gxb.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odf.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpx.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ran.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jxd.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cln.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://ftk.havefunace.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uum.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aty.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://afs.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mwj.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hvp.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pnw.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://edu.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fjh.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://mvn.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://ixq.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://yrn.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lug.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kkm.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mwq.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfh.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://yft.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nwy.guannengcc.top

[B12] 跳出多层循环
来源：http://gqj.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://clm.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://wdj.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rll.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mod.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hqx.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kyg.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mhh.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://olz.ybcxt.top

[B13] 判断是否为数字
来源：http://oub.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://vok.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://yud.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://anf.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://evl.jyoumei.cn

Java: x instanceof Number
来源：http://aww.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pss.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://dle.hywenlv.cn

C#:   x is int or double or decimal
来源：http://enh.cheryme.top

[B14] 判断值是否在集合内
来源：http://jwx.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nwo.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ytr.0kj1m.cn

JS:   [1, 2, 3].includes(x)
来源：http://bmo.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://iam.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lgd.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zme.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kqj.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gkh.epnwcf.com

[B15] 布尔运算与取反
来源：http://wmt.sweek.top

Py:   a and b or not c
来源：http://bsz.hnqzz.top

PHP:  $a && $b || !$c
来源：http://atf.yueranfly.top

JS:   a && b || !c
来源：http://zpn.daxiang520.top

TS:   a && b || !c
来源：http://kox.yfazqb.com

Java: a && b || !c
来源：http://sdj.havefunace.top

Go:   a && b || !c
来源：http://kpz.jiagoushi.top

Ruby: a && b || !c
来源：http://fjn.hywenlv.cn

C#:   a && b || !c
来源：http://lla.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://hzo.jinghuilouyu.cn

Py:   if not data: return
来源：http://aoz.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://nyf.yj20258.top

JS:   if (!data) return;
来源：http://dwc.dianchejie.cn

TS:   if (!data) return;
来源：http://khu.guannengcc.top

Java: if (data == null) return;
来源：http://dzt.zhengqikj.top

Go:   if data == nil { return }
来源：http://jrt.jinqigufen.top

Ruby: return if data.nil?
来源：http://wnd.tianlin.xyz

C#:   if (data == null) return;
来源：http://rxt.yuanzhike.top

================================================================================
来源：http://krd.cqqwz.cn

C. 函数与作用域
来源：http://qxx.aizwys.cn

================================================================================
来源：http://yup.kuanghao11.cn

[C01] 定义函数
来源：http://lzq.yj20258.top

Py:   def add(a, b): return a + b
来源：http://mtz.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fid.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://wva.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pkl.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yeh.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://skf.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://rmz.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kwb.hcnkem.com

[C02] 默认参数
来源：http://avd.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://rib.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xrf.daria6918.cn

JS:   function greet(name = "World") { return name; }
来源：http://thg.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://sik.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://otv.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ijn.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://mmx.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://dor.iojbl.cn

[C03] 可变参数
来源：http://iow.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://zqg.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rbq.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://srd.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zfi.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mek.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bld.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kre.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dte.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://urt.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://njb.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zwk.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mng.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vgz.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://olk.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://nzm.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://zfj.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://dpk.zhoulong.xyz

[C05] 返回多个值
来源：http://ubd.andypj.xyz

Py:   return a, b
来源：http://hqv.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://sxx.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tey.nanxinkj.top

TS:   return { a, b };
来源：http://cpl.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tij.quarkkingdee.top

Go:   return a, b
来源：http://lcw.9152youxi.cn

Ruby: return a, b
来源：http://jon.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://tkb.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://mla.wangdashe.top

Py:   square = lambda x: x * x
来源：http://gyz.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gyb.sufxvd.cn

JS:   const square = x => x * x;
来源：http://jhf.gzhubu.top

TS:   const square = (x: number): number => x * x;
来源：http://jir.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rnr.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://gdw.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://duo.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://ibm.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://mpr.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://msw.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://ghn.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jbi.hywenlv.cn

TS:   arr.map(String)
来源：http://vya.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oem.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ukg.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://iuw.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://uou.gogol.net.cn

[C08] 闭包
来源：http://bmc.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bey.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tno.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ufl.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rxh.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cim.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kdj.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ncu.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vcq.pycfn.com

[C09] 递归
来源：http://sqr.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ktp.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mlk.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xbt.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tlp.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rgh.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbs.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gpy.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zvy.zhiwuduotai.top

[C10] 变量作用域
来源：http://keo.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hai.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://shm.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://asj.ywan-chungtsiang.top

TS:   同 JS
来源：http://pmf.nanxinkj.top

Java: 方法内为块级作用域
来源：http://bnu.zdqjudy.top

Go:   花括号块级作用域
来源：http://qku.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rab.meibo888.top

C#:   块级作用域
来源：http://kta.daria6918.cn

[C11] 模块导入与导出
来源：http://qcf.jinqigufen.top

Py:   from module import func
来源：http://lrl.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xmi.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qvs.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vfu.aibaodan.cn

Java: import java.util.List;
来源：http://lnq.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hel.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://rqh.ybcxt.top

C#:   using System.Text;
来源：http://onz.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://lrs.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://nil.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://hsj.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://kuc.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://ifg.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sgf.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://kqu.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://afw.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pwg.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://khi.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mun.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://smb.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zpc.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qlj.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://yug.fktsv.cn

Go:   func add(a, b int) int
来源：http://ohm.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://boz.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://clt.zdbjq.cn

[C14] 泛型函数
来源：http://ksq.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ugh.yongpay.top

PHP:  // 无泛型
来源：http://ygj.tianlin.xyz

JS:   // 无泛型
来源：http://fcw.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ozk.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qcl.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lik.yvedp.cn

Ruby: # 无泛型
来源：http://elc.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kjb.yj20258888.top

[C15] 解构 / 展开参数
来源：http://kzs.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yck.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://bxs.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://izy.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oib.cqqwz.cn

Java: // 无解构
来源：http://vji.cucudq.cn

Go:   // 无解构
来源：http://gxi.guowangkeji.top

Ruby: a, b = pair
来源：http://xyp.hcnkem.com

C#:   var (a, b) = pair;
来源：http://moz.birdmap.top

[C16] 函数 / 方法重载
来源：http://cva.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wql.hammf.cn

PHP:  // 无重载
来源：http://bqw.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hhr.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://gsx.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fai.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://cvm.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://kqn.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ocm.yongpay.top

================================================================================
来源：http://qed.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://fkx.jinghuilouyu.cn

================================================================================
来源：http://pfo.daxiang520.top

[D01] 创建数组 / 列表
来源：http://itx.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://sok.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zfk.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wlw.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jmr.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kyi.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://cmq.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://kae.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://icn.gogol.net.cn

[D02] 追加元素到末尾
来源：http://zww.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kaa.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vst.hysaishi.cn

JS:   arr.push(4);
来源：http://qny.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://rqj.zdbjq.cn


<!-- 参考信息 -->