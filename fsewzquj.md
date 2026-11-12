代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qbe.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bxz.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ekv.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uwj.zycfv.cn

[A26] 类型转换总览
来源：http://tgt.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tmy.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://emb.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cdb.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://ycc.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://syo.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gwb.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hqf.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mdr.hammf.cn

================================================================================
来源：http://fal.sufxvd.cn

B. 流程控制
来源：http://fly.xinyue.icu

================================================================================
来源：http://lpf.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://unu.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://enx.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wyb.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cak.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gnr.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zfi.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://upo.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ilt.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kim.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://vsg.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rrw.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ivz.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xcg.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gwc.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vaq.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://itj.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iqu.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dvv.smart0.xyz

[B03] switch / match / case
来源：http://gka.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jwm.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qpd.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wcd.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gxu.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pkv.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dzg.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dmn.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cqq.cdnleiting.top

[B04] for 计数循环
来源：http://lxg.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://usp.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://msq.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jps.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gyu.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://edz.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nmj.zhoulong.xyz

Ruby: 10.times { |i| puts i }
来源：http://hfp.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lje.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://fnt.yueranfly.top

Py:   for item in arr: print(item)
来源：http://llu.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nwr.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uap.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://mnq.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://exy.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jyy.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://lju.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ewb.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://sio.quarkkingdee.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xjo.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://myb.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ekv.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tcf.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://arp.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ubv.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bdb.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cey.chenzaomai.com

[B07] while 循环
来源：http://qsp.guowangkeji.top

Py:   while i < 10: i += 1
来源：http://iwg.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tho.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://sco.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://nuh.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://wyf.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vrf.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://chj.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://ail.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://npj.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://vht.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://uvm.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://bxn.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://rnt.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://bxo.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://yaa.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://ldm.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://hiv.shzxlz.cn

[B09] break 与 continue
来源：http://trr.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mgo.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bye.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://luz.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlh.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdj.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hiq.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ezx.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwc.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://iua.yuxming.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://otq.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kow.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oqi.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://skv.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kzx.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lns.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sqa.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sxh.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://mtz.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://llc.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://esx.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vse.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uuv.zhongyouzk.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rbt.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://exp.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://vzl.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yvd.nanxuanxn.top

[B12] 跳出多层循环
来源：http://djt.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://klx.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nfp.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jqn.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gbn.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rou.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ptk.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nyd.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cxv.fktsv.cn

[B13] 判断是否为数字
来源：http://hsj.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://asx.yonumen.top

PHP:  is_numeric($x)
来源：http://mfw.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xkb.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dxh.ybcxt.top

Java: x instanceof Number
来源：http://kdg.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mwe.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://xgx.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://phc.tarul.cn

[B14] 判断值是否在集合内
来源：http://bac.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hfh.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rfs.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ibj.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://mfm.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sdo.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ufc.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uxj.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://slf.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://ntu.cucudq.cn

Py:   a and b or not c
来源：http://gpd.pycfn.com

PHP:  $a && $b || !$c
来源：http://xcc.hywenlv.cn

JS:   a && b || !c
来源：http://lzs.aizwys.cn

TS:   a && b || !c
来源：http://xsq.cdnleiting.top

Java: a && b || !c
来源：http://ouq.quarkkingdee.top

Go:   a && b || !c
来源：http://hek.tianlin.xyz

Ruby: a && b || !c
来源：http://zjc.pycfn.com

C#:   a && b || !c
来源：http://ccq.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lzj.daria6918.cn

Py:   if not data: return
来源：http://fss.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://geu.daria6918.cn

JS:   if (!data) return;
来源：http://lhk.cdnleiting.top

TS:   if (!data) return;
来源：http://vsp.yongpay.top

Java: if (data == null) return;
来源：http://gnw.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://slo.hywenlv.cn

Ruby: return if data.nil?
来源：http://mep.sysykeji.top

C#:   if (data == null) return;
来源：http://buj.tian-w.cn

================================================================================
来源：http://zyz.yueranfly.top

C. 函数与作用域
来源：http://xpo.dianchejie.cn

================================================================================
来源：http://wcp.ydjk.org.cn

[C01] 定义函数
来源：http://cas.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://ppf.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgs.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://lzl.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hec.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tek.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jrm.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://kol.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rcl.jinyuanbaomall.cn

[C02] 默认参数
来源：http://rai.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://amm.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gkh.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://nkn.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://xqw.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://obi.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ufw.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://ufd.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://ucd.jyoumei.cn

[C03] 可变参数
来源：http://atj.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://dza.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hma.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yrm.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nka.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xll.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yqr.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://xds.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lww.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://snu.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xle.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qvg.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ayl.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gyp.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://lnh.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://rbf.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://tll.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://kan.gogol.net.cn

[C05] 返回多个值
来源：http://abx.yonumen.top

Py:   return a, b
来源：http://tau.ydzc1.top

PHP:  return [$a, $b];
来源：http://hnv.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ruv.sjlbkw.cn

TS:   return { a, b };
来源：http://gdp.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ayb.bbcook.cn

Go:   return a, b
来源：http://jis.pengpengdd.cyou

Ruby: return a, b
来源：http://lqt.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://tee.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://qpj.52xcode.cn

Py:   square = lambda x: x * x
来源：http://akn.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ezj.zdqjudy.top

JS:   const square = x => x * x;
来源：http://fhy.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://lpp.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vdz.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://rkn.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://nrb.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://jzl.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://fem.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://chh.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://txk.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xdj.0kj1m.cn

TS:   arr.map(String)
来源：http://vke.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sjl.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uez.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://fgb.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tya.yueranfly.top

[C08] 闭包
来源：http://iwp.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yws.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nlq.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uua.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fnq.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ehq.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sxv.hysaishi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iee.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://izu.ivvv.top

[C09] 递归
来源：http://xin.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tkn.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://diu.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://khc.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qcd.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wun.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rwn.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://air.hnqzz.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gkv.52xcode.cn

[C10] 变量作用域
来源：http://kiq.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zvz.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sln.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ape.yuanzhike.top

TS:   同 JS
来源：http://fuo.daxiang520.top

Java: 方法内为块级作用域
来源：http://vks.jinqigfzy.top

Go:   花括号块级作用域
来源：http://qdz.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://odl.chenzaomai.com

C#:   块级作用域
来源：http://wbg.jiagoushi.top

[C11] 模块导入与导出
来源：http://wia.vqdsnc.cn

Py:   from module import func
来源：http://jqn.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oyd.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://snq.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nmr.cashguo.top

Java: import java.util.List;
来源：http://ldx.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xwv.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://uwa.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://wxw.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://sdk.xinyue.icu

Py:   (lambda: print("run"))()
来源：http://tqu.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://ukm.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://jpu.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://ccd.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tng.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://qzf.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://hwd.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ixx.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://ozn.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ulp.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rne.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uya.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdd.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://pat.andypj.xyz

Go:   func add(a, b int) int
来源：http://wna.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fps.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://kyr.zhixingplan.top

[C14] 泛型函数
来源：http://fcq.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://axa.yuxming.cn

PHP:  // 无泛型
来源：http://zpt.yfazqb.com

JS:   // 无泛型
来源：http://vmh.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ykj.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cuy.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aoy.haohaochexian.top

Ruby: # 无泛型
来源：http://qjt.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rsi.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://gzg.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xsd.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://pwc.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wxa.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mpg.zhongyouzk.top

Java: // 无解构
来源：http://ucc.gaohongyu789.top

Go:   // 无解构
来源：http://psp.nwbrower.top

Ruby: a, b = pair
来源：http://jfj.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://yye.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://itq.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ztc.tarul.cn


<!-- 参考信息 -->