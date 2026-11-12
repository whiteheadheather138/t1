代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://dyu.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hjj.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lzx.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bmu.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ypn.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pla.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kmt.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xox.tanke756.top

[A26] 类型转换总览
来源：http://sfy.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pal.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uhg.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fxp.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://aef.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hmi.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://thx.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sjy.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zat.hnqzz.top

================================================================================
来源：http://rlc.bjfxy.top

B. 流程控制
来源：http://ian.shanyushiyangtech.top

================================================================================
来源：http://mdv.cheryme.top

[B01] 条件判断 if / else
来源：http://izb.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lpa.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qyo.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mkv.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vab.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vri.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pla.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nhb.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tun.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://ude.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bja.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vwo.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yio.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://drd.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aig.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zww.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ari.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eem.shanyushiyangkeji.top

[B03] switch / match / case
来源：http://xvk.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uag.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fyx.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dbi.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bzg.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lpf.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mbb.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://end.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mox.wangdashe.top

[B04] for 计数循环
来源：http://ryl.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://owf.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hwk.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wml.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kyr.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hjq.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://grv.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://sop.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://biv.316326.xyz

[B05] 遍历数组 / 列表
来源：http://msn.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://kox.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lxi.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kdk.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rim.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dul.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jvg.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://crh.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kgy.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://pqg.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bjo.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://irz.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://phl.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vsf.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xvu.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mtg.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pdc.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ldx.hesvh.cn

[B07] while 循环
来源：http://rwj.guannengcc.top

Py:   while i < 10: i += 1
来源：http://ofw.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://yac.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://ndt.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://all.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://zff.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jaw.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://ykl.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://ify.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://bcu.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://adk.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jzi.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://ulj.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://eoh.cdnleiting.top

Java: do { i++; } while (i < 10);
来源：http://ysw.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ikq.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mdx.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://yhs.zhijiandao.cn

[B09] break 与 continue
来源：http://xak.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wvz.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pwk.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpa.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxe.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpu.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ukb.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xdj.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qam.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://mqw.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vqt.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wqj.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fls.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zbd.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sbi.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://erc.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uci.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://psr.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://wvk.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://cht.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://swe.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bev.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jja.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rdt.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eya.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://fee.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lsj.yonumen.top

[B12] 跳出多层循环
来源：http://tuu.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qcb.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fjj.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wtp.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvr.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://azc.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nia.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oag.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jvk.ydzc1.top

[B13] 判断是否为数字
来源：http://oqc.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://lbu.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://lmn.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gqn.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qry.nanxinkj.top

Java: x instanceof Number
来源：http://hsx.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jqy.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://qcs.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://vsh.c1oappe.top

[B14] 判断值是否在集合内
来源：http://vnc.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qgu.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://piq.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://idq.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://cby.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pod.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aoo.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://gzz.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tqt.bbcook.cn

[B15] 布尔运算与取反
来源：http://kgx.zhengqikj.top

Py:   a and b or not c
来源：http://yej.epnwcf.com

PHP:  $a && $b || !$c
来源：http://pxb.tianlin.xyz

JS:   a && b || !c
来源：http://vgd.9152youxi.cn

TS:   a && b || !c
来源：http://hre.9152youxi.cn

Java: a && b || !c
来源：http://zsd.svipenyu.cn

Go:   a && b || !c
来源：http://mdy.hcnkem.com

Ruby: a && b || !c
来源：http://zrt.shanyushiyangtech.top

C#:   a && b || !c
来源：http://ufl.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lzb.yuxming.cn

Py:   if not data: return
来源：http://voy.hammf.cn

PHP:  if (!$data) { return; }
来源：http://bvh.meibo888.top

JS:   if (!data) return;
来源：http://xuw.svipenyu.cn

TS:   if (!data) return;
来源：http://dmc.ppjwa.cn

Java: if (data == null) return;
来源：http://hlq.yj20258888.top

Go:   if data == nil { return }
来源：http://syv.52xcode.cn

Ruby: return if data.nil?
来源：http://uqa.jlsjyb.cn

C#:   if (data == null) return;
来源：http://chy.xziqi.cn

================================================================================
来源：http://xkr.hongshengwenyu.top

C. 函数与作用域
来源：http://bts.iojbl.cn

================================================================================
来源：http://dai.ivvv.top

[C01] 定义函数
来源：http://uvk.meibo888.top

Py:   def add(a, b): return a + b
来源：http://fwr.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dmn.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://vjw.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wad.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://roj.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://bgv.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://pvp.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qim.smart0.xyz

[C02] 默认参数
来源：http://mbd.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://nai.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ymy.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://umy.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tkg.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lhr.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mrt.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://oxs.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://bek.hfpthk.cn

[C03] 可变参数
来源：http://fpp.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://izu.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hhu.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sta.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ovw.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vih.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rbw.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tsd.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cze.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://qwi.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xlp.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uad.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ywq.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bux.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://xdi.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://iic.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://jse.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://ske.meibo888.top

[C05] 返回多个值
来源：http://uva.ywan-chungtsiang.top

Py:   return a, b
来源：http://jre.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://dnw.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cef.nanxinkj.top

TS:   return { a, b };
来源：http://bez.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qnf.ybcxt.top

Go:   return a, b
来源：http://fxn.wangshuangyany.cn

Ruby: return a, b
来源：http://phx.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://ftc.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://pzy.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://lmg.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://ytp.guannengcc.top

JS:   const square = x => x * x;
来源：http://tqy.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://ecc.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ucz.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iwt.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://gsr.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://svu.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://bph.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iff.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://oqe.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kkw.tian-w.cn

TS:   arr.map(String)
来源：http://ucb.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yjl.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nqp.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://ula.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hlx.xinyue.icu

[C08] 闭包
来源：http://yjd.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lgu.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ced.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yzj.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tfj.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xfr.ctjpmb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pcs.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fmp.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pzt.meibo888.top

[C09] 递归
来源：http://rcv.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://krh.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ili.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hcq.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ykj.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nun.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tqy.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tys.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ksr.nwbrower.top

[C10] 变量作用域
来源：http://ibx.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mij.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://egb.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cyn.yj202588.top

TS:   同 JS
来源：http://txc.ctjpmb.com

Java: 方法内为块级作用域
来源：http://utp.sufxvd.cn

Go:   花括号块级作用域
来源：http://knq.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xrz.cucudq.cn

C#:   块级作用域
来源：http://gzw.zhoulong.xyz

[C11] 模块导入与导出
来源：http://mzi.jqgufenzy.top

Py:   from module import func
来源：http://epe.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vps.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xqg.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qqv.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://grt.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ftg.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://mtg.52xcode.cn

C#:   using System.Text;
来源：http://urv.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://fsx.cashguo.top

Py:   (lambda: print("run"))()
来源：http://xhp.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://dmo.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://mon.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://cmy.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ree.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://qwl.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://ikw.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lpg.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://doi.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wqi.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uzs.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://row.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdk.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://wbk.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://kmp.quarkkingdee.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mro.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://obl.zhiwuduotai.top

[C14] 泛型函数
来源：http://ess.xingfuxueyuan.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oqt.zhoulong.xyz

PHP:  // 无泛型
来源：http://dpd.gotoacloud.top

JS:   // 无泛型
来源：http://ckq.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aiv.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vjn.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxx.feifeiyinyue.top

Ruby: # 无泛型
来源：http://axe.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cmh.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://pgv.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uiv.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://xul.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bei.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oqj.meibo888.top

Java: // 无解构
来源：http://qlc.xylfe.cn

Go:   // 无解构
来源：http://xup.shanyushiyangtech.top


<!-- 参考信息 -->