代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ayi.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ass.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iau.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fij.zhengqikj.top

[A26] 类型转换总览
来源：http://dgz.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pbu.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uit.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zsk.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://gzv.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ihe.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qcq.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qvy.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ksv.chenjidiqi.icu

================================================================================
来源：http://xgx.gaohongyu789.top

B. 流程控制
来源：http://awl.redwolf501.top

================================================================================
来源：http://onj.bjfxy.top

[B01] 条件判断 if / else
来源：http://god.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ggv.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://orv.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zzo.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cvm.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kam.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lbo.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gas.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fou.pycfn.com

[B02] 多分支 else if / elif
来源：http://dfx.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jvg.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ejq.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://soa.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnn.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvu.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qii.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dfw.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tko.jqgufenzy.top

[B03] switch / match / case
来源：http://aht.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://des.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ize.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://you.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jbb.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aga.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rrt.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gdv.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://viz.tianlin.xyz

[B04] for 计数循环
来源：http://vfw.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://oru.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://amu.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gqw.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jbk.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zlm.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gze.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://syf.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://saz.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://eeb.daxiang520.top

Py:   for item in arr: print(item)
来源：http://knr.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://clm.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fwg.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nqg.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eup.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tyb.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://umo.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://erp.yj202588.top

[B06] 遍历字典 / 对象
来源：http://crr.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://zey.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lsa.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ptt.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cuo.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ezq.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://izw.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hne.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hac.ywan-chungtsiang.top

[B07] while 循环
来源：http://lft.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://jcs.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oln.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://fty.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://shy.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://ffi.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lid.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://xuu.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://fhk.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://qdc.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://ozq.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ovg.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://dcz.jinghuilouyu.cn

TS:   do { i++; } while (i < 10);
来源：http://bjm.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://cvv.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fyj.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://xbb.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://gum.yj202588.top

[B09] break 与 continue
来源：http://ttp.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yrm.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://epc.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zjc.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkt.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tio.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mel.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hso.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngw.cqqwz.cn

[B10] 遍历同时拿索引
来源：http://vsl.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nck.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://inb.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wmw.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mgw.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pcu.ywan-chungtsiang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cyi.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qvq.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eic.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://xkb.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://tbi.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://onv.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kaj.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ubo.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tgg.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qfs.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://vfe.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pzb.yonumen.top

[B12] 跳出多层循环
来源：http://iqf.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bdl.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wwk.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vhq.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fql.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ckw.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://evh.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xdg.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hie.tarul.cn

[B13] 判断是否为数字
来源：http://yup.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://pob.tarul.cn

PHP:  is_numeric($x)
来源：http://olo.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vry.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lzt.xylfe.cn

Java: x instanceof Number
来源：http://ggp.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iyu.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://jbl.xziqi.cn

C#:   x is int or double or decimal
来源：http://rjp.tanke756.top

[B14] 判断值是否在集合内
来源：http://rjo.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gsu.haohaochexian.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sof.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://zmu.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://dhb.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eys.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hgj.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://daz.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ojq.epnwcf.com

[B15] 布尔运算与取反
来源：http://giy.daria6918.cn

Py:   a and b or not c
来源：http://kjs.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://gku.cheryme.top

JS:   a && b || !c
来源：http://mal.tianlin.xyz

TS:   a && b || !c
来源：http://oup.birdmap.top

Java: a && b || !c
来源：http://ahs.shanyushiyangtech.top

Go:   a && b || !c
来源：http://qbf.uphjek.com

Ruby: a && b || !c
来源：http://jyx.sweek.top

C#:   a && b || !c
来源：http://thl.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://wrq.zdqjudy.top

Py:   if not data: return
来源：http://vis.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://uyu.nwbrower.top

JS:   if (!data) return;
来源：http://sqx.yanxiufei.cn

TS:   if (!data) return;
来源：http://tfc.fktsv.cn

Java: if (data == null) return;
来源：http://zlv.hysaishi.cn

Go:   if data == nil { return }
来源：http://was.pycfn.com

Ruby: return if data.nil?
来源：http://ljq.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://hdi.nwbrower.top

================================================================================
来源：http://fng.cdnleiting.top

C. 函数与作用域
来源：http://pwc.316326.xyz

================================================================================
来源：http://szd.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://eti.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://idu.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqz.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://ypf.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eqy.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gtv.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://kkh.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://ald.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fuz.nwbrower.top

[C02] 默认参数
来源：http://ubj.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://hqm.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ktt.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://kkq.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://plx.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://boa.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cgz.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://sut.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://tgn.jyoumei.cn

[C03] 可变参数
来源：http://uwe.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://rkc.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qrk.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sah.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ojc.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mqm.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jed.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xos.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iil.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://pvo.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fjg.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zwz.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uok.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uky.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://qvb.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://cqb.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://sis.smart0.xyz

C#:   f(a: 1, b: 2)
来源：http://jam.iojbl.cn

[C05] 返回多个值
来源：http://rko.hesvh.cn

Py:   return a, b
来源：http://ylk.bbcook.cn

PHP:  return [$a, $b];
来源：http://ysk.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pfm.gzhubu.top

TS:   return { a, b };
来源：http://cdk.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mgy.chenjidiqi.icu

Go:   return a, b
来源：http://ked.jlsjyb.cn

Ruby: return a, b
来源：http://iuk.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://nwg.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://pvf.daxiang520.top

Py:   square = lambda x: x * x
来源：http://yyw.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lzg.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://alg.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://pcj.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wnn.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://mmw.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://lpe.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://dic.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://zgv.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xlp.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://abi.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tan.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://fkc.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yjb.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zwj.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://lsb.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://toi.gaohongyu789.top

[C08] 闭包
来源：http://dsp.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rhl.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jfs.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ndc.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jov.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rbz.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://olc.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ftw.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nom.vqdsnc.cn

[C09] 递归
来源：http://yja.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eyy.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bnv.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vdu.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ctn.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tud.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oqx.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xob.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lyp.yvedp.cn

[C10] 变量作用域
来源：http://wlp.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gcg.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jww.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qhq.daxiang520.top

TS:   同 JS
来源：http://lps.zdbjq.cn

Java: 方法内为块级作用域
来源：http://puz.nanxuanxn.top

Go:   花括号块级作用域
来源：http://hlo.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://piy.jinqigfzy.top

C#:   块级作用域
来源：http://nsj.gotoacloud.top

[C11] 模块导入与导出
来源：http://hyt.ywan-chungtsiang.top

Py:   from module import func
来源：http://qbs.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nmf.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ayl.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mgh.zhixingplan.top

Java: import java.util.List;
来源：http://qeb.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://snf.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://rrp.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://hzg.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://rdt.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://tio.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://cmg.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://cwv.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://cfn.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lyc.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://zsz.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://qcu.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yim.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://bmu.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zrw.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tgn.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gbi.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hlf.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tql.cashguo.top

Go:   func add(a, b int) int
来源：http://cgi.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mjp.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://hpc.yj20258888.top

[C14] 泛型函数
来源：http://nhk.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bqq.sweek.top

PHP:  // 无泛型
来源：http://rmc.quarkkingdee.top

JS:   // 无泛型
来源：http://tmg.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wrs.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qao.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hjr.aizwys.cn

Ruby: # 无泛型
来源：http://zki.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yaq.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://qxi.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gur.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://ewd.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wmc.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cdx.bjfxy.top

Java: // 无解构
来源：http://tno.daxiang520.top

Go:   // 无解构
来源：http://ivx.ivvv.top

Ruby: a, b = pair
来源：http://jpz.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://oxu.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://ugo.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ilt.zdqjudy.top


<!-- 参考信息 -->