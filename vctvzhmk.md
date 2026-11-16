代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lei.shzxlz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bfm.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oso.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ykn.yonumen.top

[A26] 类型转换总览
来源：http://pcr.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://icp.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vwy.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pny.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://ewg.nwbrower.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nbj.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hmv.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ywh.fanxiaobao.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xkj.hesvh.cn

================================================================================
来源：http://hev.birdmap.top

B. 流程控制
来源：http://eut.jinqigfzy.top

================================================================================
来源：http://pmh.hfpthk.cn

[B01] 条件判断 if / else
来源：http://uwz.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://czr.9152youxi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aef.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jxk.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://myj.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://etq.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lqn.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ioq.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bhn.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://tor.jinghuilouyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ngj.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vhc.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuz.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdk.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fam.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nfx.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hjz.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tek.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://yxn.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gye.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://whc.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rlk.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xlm.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mko.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tdj.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gft.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://led.fehbvm.com

[B04] for 计数循环
来源：http://rzq.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://tun.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ggw.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ztn.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rrx.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://izy.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cnw.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://ndq.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oud.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://cnv.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://lxb.ivvv.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lle.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tqo.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sks.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://vmz.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iom.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://jgl.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jhj.havefunace.top

[B06] 遍历字典 / 对象
来源：http://wne.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jto.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lcz.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fml.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zir.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ifj.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ktr.iojbl.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eay.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nfm.gotoacloud.top

[B07] while 循环
来源：http://atx.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://pmv.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://fag.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://zpi.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://ttn.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://uhv.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mpj.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://ace.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://ere.zdbjq.cn

[B08] do-while（至少执行一次）
来源：http://ppi.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://lyh.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wyy.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://jqg.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://zlq.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://kri.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://pzr.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fhh.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://yue.9152youxi.cn

[B09] break 与 continue
来源：http://tww.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xvg.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gjn.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cic.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsr.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxd.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lke.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lbl.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://avr.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://nba.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://txp.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://swq.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tzz.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ehj.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rft.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hno.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xaw.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jsb.vehdjk.com

[B11] 生成数字序列 / 区间
来源：http://gyo.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://ymf.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://gic.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rvz.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pvl.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wab.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rtm.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://xbz.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vhk.tanke756.top

[B12] 跳出多层循环
来源：http://lxs.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://idu.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ahz.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dqq.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://emc.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jnf.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kht.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hnm.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zty.zhijiandao.cn

[B13] 判断是否为数字
来源：http://sdx.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://ili.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://lju.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwl.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wxn.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://sfn.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yhd.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://ete.yj202588.top

C#:   x is int or double or decimal
来源：http://ijp.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://bbw.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rqx.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ehy.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://pkp.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://spq.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hbd.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vkc.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://bmb.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cnh.chenlongwang.top

[B15] 布尔运算与取反
来源：http://cth.xuanzx.com

Py:   a and b or not c
来源：http://kgv.zycfv.cn

PHP:  $a && $b || !$c
来源：http://sjh.fengsongda.top

JS:   a && b || !c
来源：http://ugx.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://ywi.fktsv.cn

Java: a && b || !c
来源：http://djl.ehwqpu.com

Go:   a && b || !c
来源：http://qcs.vqdsnc.cn

Ruby: a && b || !c
来源：http://dml.pycfn.com

C#:   a && b || !c
来源：http://eee.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://puu.haohaochexian.top

Py:   if not data: return
来源：http://oim.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://rnc.xinyue.icu

JS:   if (!data) return;
来源：http://xcs.sweek.top

TS:   if (!data) return;
来源：http://sni.cheryme.top

Java: if (data == null) return;
来源：http://rnc.tarul.cn

Go:   if data == nil { return }
来源：http://vty.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://ztg.smart0.xyz

C#:   if (data == null) return;
来源：http://kpf.gogol.net.cn

================================================================================
来源：http://ogi.aibaodan.cn

C. 函数与作用域
来源：http://dcb.chenlongwang.top

================================================================================
来源：http://lrg.sufxvd.cn

[C01] 定义函数
来源：http://ddd.yj202588.top

Py:   def add(a, b): return a + b
来源：http://bgp.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uxg.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://qte.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vnz.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://khm.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iyk.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://xxc.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mro.hnqzz.top

[C02] 默认参数
来源：http://fgy.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://zyi.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zwp.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://mlv.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bav.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hqc.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ggo.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://xav.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://iho.guannengcc.top

[C03] 可变参数
来源：http://rjp.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://qkj.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ssd.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tlw.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://poe.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vtz.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dcg.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qhp.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sdj.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://afv.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dhs.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sbt.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yrz.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ljh.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://rtz.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://grv.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://fxr.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://ift.9152youxi.cn

[C05] 返回多个值
来源：http://xmb.ybcxt.top

Py:   return a, b
来源：http://ina.ydzc1.top

PHP:  return [$a, $b];
来源：http://elj.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://obp.epnwcf.com

TS:   return { a, b };
来源：http://jbp.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rmo.epnwcf.com

Go:   return a, b
来源：http://rsp.sjlbkw.cn

Ruby: return a, b
来源：http://evt.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://rck.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://iah.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://zsc.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ybt.sysykeji.top

JS:   const square = x => x * x;
来源：http://tlb.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://isv.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fnn.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://rvk.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://lgr.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mbb.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://aop.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eyz.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://njc.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nei.sysykeji.top

TS:   arr.map(String)
来源：http://itq.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uut.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lvi.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://ofs.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ygl.ctjpmb.com

[C08] 闭包
来源：http://nlq.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vtr.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xxh.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jkb.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pqc.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hwh.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tkk.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lju.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vor.zdbjq.cn

[C09] 递归
来源：http://myi.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fij.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://owr.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vsr.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yre.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://osh.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eqb.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nrk.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lzn.hongshengwenyu.top

[C10] 变量作用域
来源：http://bgx.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iga.xylfe.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://srx.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pdd.yangfankeji.com

TS:   同 JS
来源：http://vdb.bbcook.cn

Java: 方法内为块级作用域
来源：http://umh.ppjwa.cn

Go:   花括号块级作用域
来源：http://mfv.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ayi.shangyingyoupin.top

C#:   块级作用域
来源：http://otm.pycfn.com

[C11] 模块导入与导出
来源：http://gwo.gaohongyu789.top

Py:   from module import func
来源：http://dmj.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hqi.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://rhk.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ewf.daria6918.cn

Java: import java.util.List;
来源：http://dlg.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kuo.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://qol.cashguo.top

C#:   using System.Text;
来源：http://ovu.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://gsj.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://vkp.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://bjn.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://ult.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://rms.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ehc.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://wep.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://ses.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pwa.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://ipq.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zsq.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckn.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gjo.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://clg.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://ssb.sxryk.cn

Go:   func add(a, b int) int
来源：http://rbp.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ioi.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eet.jianghu66.top

[C14] 泛型函数
来源：http://pab.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aqt.hcnkem.com

PHP:  // 无泛型
来源：http://kpy.yongpay.top

JS:   // 无泛型
来源：http://cke.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qoq.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xeu.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://feq.yangfankeji.com

Ruby: # 无泛型
来源：http://lxy.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xhp.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://khw.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sut.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://agh.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fkq.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uie.dianchejie.cn

Java: // 无解构
来源：http://ntq.shanyushiyangkeji.top

Go:   // 无解构
来源：http://ncx.wangshuangyany.cn

Ruby: a, b = pair
来源：http://qcf.andypj.xyz

C#:   var (a, b) = pair;
来源：http://udr.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://sah.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mlw.wangshuangyany.cn


<!-- 参考信息 -->