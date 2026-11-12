代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://ynj.ydjk.org.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ijr.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rlu.zhiwuduotai.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wbh.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://svk.cheryme.top

================================================================================
来源：http://hcq.chenlongwang.top

B. 流程控制
来源：http://dap.nanxinkj.top

================================================================================
来源：http://crr.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://gyr.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tpy.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nxa.ywan-chungtsiang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hvy.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zwz.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xww.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qpx.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://znq.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tsl.redwolf501.top

[B02] 多分支 else if / elif
来源：http://giv.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ldj.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mgn.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aov.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltd.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pdc.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://azk.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pjn.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbi.tanke756.top

[B03] switch / match / case
来源：http://zbj.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gyy.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nxq.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qbf.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qtj.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gvm.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lsh.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xqu.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mbn.nanxuanxn.top

[B04] for 计数循环
来源：http://cjz.yuanzhike.top

Py:   for i in range(10): print(i)
来源：http://cnp.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wtw.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rdr.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xwf.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mmw.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kwm.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://vtp.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hzz.birdmap.top

[B05] 遍历数组 / 列表
来源：http://wtq.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://zkg.jianghu66.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lcw.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mhc.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://zyd.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://pcs.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tew.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://dhv.tian-w.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vxd.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://wjk.zdbjq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lsy.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ndo.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bbq.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ccj.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eaa.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pkb.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xki.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dpc.yuanzhike.top

[B07] while 循环
来源：http://yiu.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://jqh.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eai.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://aql.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://jfu.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://rmq.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jkh.cheryme.top

Ruby: while i < 10; i += 1; end
来源：http://vrm.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://ebs.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://vaq.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://yfd.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cbx.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://der.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://ofm.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://qdz.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fkm.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://lyo.yj20258888.top

C#:   do { i++; } while (i < 10);
来源：http://hpt.yanxiufei.cn

[B09] break 与 continue
来源：http://ztw.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xur.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ygy.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okl.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdd.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gac.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gke.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tjr.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbw.316326.xyz

[B10] 遍历同时拿索引
来源：http://nkh.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uas.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sjc.feifeiyinyue.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ydf.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jvp.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bfv.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ino.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jhi.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rdu.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://qkd.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://iul.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://oxl.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ppp.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fcm.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rdm.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ryh.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://skp.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zju.hfpthk.cn

[B12] 跳出多层循环
来源：http://amq.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://gpa.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kte.jinqigfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ggl.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://thj.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oox.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gnl.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wvz.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rys.jlsjyb.cn

[B13] 判断是否为数字
来源：http://zbe.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://gjb.cashguo.top

PHP:  is_numeric($x)
来源：http://alz.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tay.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://key.smart0.xyz

Java: x instanceof Number
来源：http://jmv.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vgf.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://rgu.sxryk.cn

C#:   x is int or double or decimal
来源：http://qro.52xcode.cn

[B14] 判断值是否在集合内
来源：http://hqs.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iwt.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mjj.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://seu.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sbm.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://loc.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vle.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://xun.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fxy.daxiang520.top

[B15] 布尔运算与取反
来源：http://ycz.pycfn.com

Py:   a and b or not c
来源：http://yag.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://bqi.jinqigufen.top

JS:   a && b || !c
来源：http://lww.jqgufenzy.top

TS:   a && b || !c
来源：http://kek.vqdsnc.cn

Java: a && b || !c
来源：http://nrs.tanke756.top

Go:   a && b || !c
来源：http://lid.ydjk.org.cn

Ruby: a && b || !c
来源：http://myo.epnwcf.com

C#:   a && b || !c
来源：http://jgm.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://fwb.hongshengwenyu.top

Py:   if not data: return
来源：http://gbw.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://cag.yonumen.top

JS:   if (!data) return;
来源：http://cqj.fzhhl.top

TS:   if (!data) return;
来源：http://nee.hongshengwenyu.top

Java: if (data == null) return;
来源：http://yqf.yanxiufei.cn

Go:   if data == nil { return }
来源：http://mss.yanxiufei.cn

Ruby: return if data.nil?
来源：http://vjz.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://emb.jinghuilouyu.cn

================================================================================
来源：http://snz.wangshuangyany.cn

C. 函数与作用域
来源：http://igs.wangdashe.top

================================================================================
来源：http://buf.dianchejie.cn

[C01] 定义函数
来源：http://cik.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://kyf.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://agh.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://lmr.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oxo.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://keo.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://lno.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://tft.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gdd.xylfe.cn

[C02] 默认参数
来源：http://lxp.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://jzs.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://knp.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://mqi.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://kli.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ert.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://djf.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://gro.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://pbd.meibo888.top

[C03] 可变参数
来源：http://qfw.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://vqt.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://drb.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pvn.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bmw.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ecy.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bht.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kzk.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rpv.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://hvu.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rdw.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sga.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tfp.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bff.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://adi.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://ojw.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://dml.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://gsm.hnqzz.top

[C05] 返回多个值
来源：http://okd.chenlongwang.top

Py:   return a, b
来源：http://brb.hnqzz.top

PHP:  return [$a, $b];
来源：http://fgp.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kra.fengsongda.top

TS:   return { a, b };
来源：http://atk.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ltz.xziqi.cn

Go:   return a, b
来源：http://cin.chenlongwang.top

Ruby: return a, b
来源：http://bdn.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://cyk.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://ibl.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://wof.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://psg.yj20258.top

JS:   const square = x => x * x;
来源：http://tny.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://kal.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qrv.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://rmc.cheryme.top

Ruby: square = ->(x) { x * x }
来源：http://mcm.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://ujd.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://gjd.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nee.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ayn.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://plr.ydzc1.top

TS:   arr.map(String)
来源：http://xhm.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nzs.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qvh.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://etz.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://esm.meibo888.top

[C08] 闭包
来源：http://bvw.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xxt.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dkh.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gxq.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zmv.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hjb.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cdz.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ubn.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ujl.hysaishi.cn

[C09] 递归
来源：http://tth.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sqd.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://upq.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nyj.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pfb.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cnv.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qsu.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://elj.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tta.sjlbkw.cn

[C10] 变量作用域
来源：http://vex.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://quo.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mga.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oru.wangdashe.top

TS:   同 JS
来源：http://fmp.guannengcc.top

Java: 方法内为块级作用域
来源：http://vut.52xcode.cn

Go:   花括号块级作用域
来源：http://hre.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xui.tian-w.cn

C#:   块级作用域
来源：http://cfe.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://usr.gogol.net.cn

Py:   from module import func
来源：http://ngt.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rie.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://bgb.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ijs.gotoacloud.top

Java: import java.util.List;
来源：http://suf.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tns.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://syv.vqdsnc.cn

C#:   using System.Text;
来源：http://ccu.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://aez.fzhhl.top

Py:   (lambda: print("run"))()
来源：http://hbi.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://dmq.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://rtm.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://wzv.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mfu.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://sbo.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://cgx.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://dxj.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://usf.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bai.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kob.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://okn.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqc.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xrx.zdbjq.cn

Go:   func add(a, b int) int
来源：http://hgk.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://deo.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://ump.aizwys.cn

[C14] 泛型函数
来源：http://zwr.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bus.jyoumei.cn

PHP:  // 无泛型
来源：http://ruw.sxryk.cn

JS:   // 无泛型
来源：http://qmh.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://joa.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gwh.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://whm.redwolf501.top

Ruby: # 无泛型
来源：http://dhl.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rgr.shuidangran.top

[C15] 解构 / 展开参数
来源：http://lws.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gfw.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://lne.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ury.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gju.cucudq.cn

Java: // 无解构
来源：http://flm.tian-w.cn

Go:   // 无解构
来源：http://tai.nanxinkj.top

Ruby: a, b = pair
来源：http://mhm.bjfxy.top

C#:   var (a, b) = pair;
来源：http://avv.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://qrd.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dcf.redwolf501.top

PHP:  // 无重载
来源：http://xpf.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pkh.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://xtm.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://woa.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://jhr.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://uyp.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gwb.yj20258888.top

================================================================================
来源：http://yar.dashuyun.cn


<!-- 参考信息 -->