代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://pqp.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ysg.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pfl.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ftq.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iuy.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nbe.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://dgg.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wcr.jianghu66.top

[A26] 类型转换总览
来源：http://cnh.zhengqikj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eev.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ffq.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tlj.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://qca.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xck.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vcp.shzxlz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gxq.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gtx.jinqigfzy.top

================================================================================
来源：http://tco.cdnleiting.top

B. 流程控制
来源：http://mqx.zhaomingkeji.xyz

================================================================================
来源：http://uiz.xinyue.icu

[B01] 条件判断 if / else
来源：http://rjv.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tdl.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://shs.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lwf.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sbm.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://nwx.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mns.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://srp.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dfh.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://vsp.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xvr.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cpa.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbf.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xij.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hol.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://alk.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hlv.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwl.fzhhl.top

[B03] switch / match / case
来源：http://ehq.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ikt.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qpa.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://axy.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aya.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uvg.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hgz.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qxm.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vpr.meibo888.top

[B04] for 计数循环
来源：http://bmw.tanke756.top

Py:   for i in range(10): print(i)
来源：http://ftj.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icz.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rgz.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tpg.chenjidiqi.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dsb.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://okk.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://tfv.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ecx.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://jxf.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://fvj.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eir.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ekf.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://bwd.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ivp.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iij.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://acy.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wge.tanke756.top

[B06] 遍历字典 / 对象
来源：http://rep.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://swj.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jic.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pyv.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hny.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iqt.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nxd.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fpw.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aiv.xylfe.cn

[B07] while 循环
来源：http://cat.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://hfq.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kyh.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://pbp.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://tdr.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://mgc.yonumen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lez.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://cxc.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://ylp.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://nzh.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://hpn.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ifo.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://xjc.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://uvl.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://oxj.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bko.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dth.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://sge.cucudq.cn

[B09] break 与 continue
来源：http://jeb.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xnc.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ukj.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsz.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzc.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwf.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ihs.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jjz.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nyc.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://kyv.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://flp.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kiw.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xrv.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://epw.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pvg.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nqv.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wem.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iqy.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://bma.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://jhk.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://lxx.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sjm.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lhj.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lhc.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dcr.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://zne.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mgv.wangdashe.top

[B12] 跳出多层循环
来源：http://plt.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://sdj.chenzaomai.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vxq.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lcl.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xgh.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://usn.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kof.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://adw.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://txm.tarul.cn

[B13] 判断是否为数字
来源：http://hsp.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://zuz.sysykeji.top

PHP:  is_numeric($x)
来源：http://unb.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://shc.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rvz.aibaodan.cn

Java: x instanceof Number
来源：http://jjf.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://veg.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://ihc.ehwqpu.com

C#:   x is int or double or decimal
来源：http://qzg.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://awm.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://khz.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sqy.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://asy.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://ugr.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://idl.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jdu.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fwh.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yiv.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://rkv.zhiwuduotai.top

Py:   a and b or not c
来源：http://guo.ybcxt.top

PHP:  $a && $b || !$c
来源：http://hbf.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://ymu.zhoulong.xyz

TS:   a && b || !c
来源：http://vrd.jinqigufen.top

Java: a && b || !c
来源：http://ohb.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://xnf.zhijiandao.cn

Ruby: a && b || !c
来源：http://wdw.9152youxi.cn

C#:   a && b || !c
来源：http://iny.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://swk.haohaochexian.top

Py:   if not data: return
来源：http://qxk.cheryme.top

PHP:  if (!$data) { return; }
来源：http://tce.zhengqikj.top

JS:   if (!data) return;
来源：http://asc.jiagoushi.top

TS:   if (!data) return;
来源：http://ida.hcnkem.com

Java: if (data == null) return;
来源：http://xka.wangdashe.top

Go:   if data == nil { return }
来源：http://fyp.yfazqb.com

Ruby: return if data.nil?
来源：http://jqi.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://lpk.yonumen.top

================================================================================
来源：http://taj.hammf.cn

C. 函数与作用域
来源：http://tyx.zdbjq.cn

================================================================================
来源：http://bdn.9152youxi.cn

[C01] 定义函数
来源：http://pvp.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://deo.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dwd.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://leo.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vdu.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oec.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kvm.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://jhu.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ygy.9152youxi.cn

[C02] 默认参数
来源：http://umx.tarul.cn

Py:   def greet(name="World"): return name
来源：http://bkt.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://alg.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://mdb.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pzg.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xmj.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yps.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://ghh.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://evp.andypj.xyz

[C03] 可变参数
来源：http://tvx.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://xuj.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wri.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ktr.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ezf.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pus.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nqu.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://hjq.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qrv.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://wmn.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owu.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nbt.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwe.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://shm.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://xxs.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://wiu.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://zvd.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://eru.sjlbkw.cn

[C05] 返回多个值
来源：http://tju.ydzc1.top

Py:   return a, b
来源：http://tmb.sysykeji.top

PHP:  return [$a, $b];
来源：http://bqa.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ngg.jlsjyb.cn

TS:   return { a, b };
来源：http://ujw.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jyi.andypj.xyz

Go:   return a, b
来源：http://exe.nwbrower.top

Ruby: return a, b
来源：http://akp.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://ubo.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://scl.mhx1999.top

Py:   square = lambda x: x * x
来源：http://gha.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gnn.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://mxq.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://sgh.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://emd.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://moj.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://bhs.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://isr.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://pen.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bjy.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://jhl.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kvk.cucudq.cn

TS:   arr.map(String)
来源：http://adg.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://odp.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xjb.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://fpd.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lyg.vehdjk.com

[C08] 闭包
来源：http://mcq.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hgt.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mks.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://thr.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tyk.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aws.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ysp.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kyx.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qkz.chenjidiqi.icu

[C09] 递归
来源：http://zeb.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nis.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wja.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uzb.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kml.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mkh.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qrr.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fgm.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lnr.cashguo.top

[C10] 变量作用域
来源：http://vhi.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rhk.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cbg.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rps.pycfn.com

TS:   同 JS
来源：http://tfb.ppjwa.cn

Java: 方法内为块级作用域
来源：http://mve.jinqigufen.top

Go:   花括号块级作用域
来源：http://wuf.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vrw.wangshuangyany.cn

C#:   块级作用域
来源：http://kye.hywenlv.cn

[C11] 模块导入与导出
来源：http://rcr.uphjek.com

Py:   from module import func
来源：http://vur.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://azf.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gpa.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xme.quarkkingdee.top

Java: import java.util.List;
来源：http://ett.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qcw.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://xba.aizwys.cn

C#:   using System.Text;
来源：http://zjs.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://lku.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://txs.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://ula.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://ooe.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://cvk.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ftu.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://izq.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://pxa.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bij.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://rlg.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mne.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fef.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ynb.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ltd.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://nxz.ehwqpu.com

Go:   func add(a, b int) int
来源：http://jjn.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zht.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://tht.epnwcf.com

[C14] 泛型函数
来源：http://jwc.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://svx.uphjek.com

PHP:  // 无泛型
来源：http://xhc.dashuyun.cn

JS:   // 无泛型
来源：http://iaj.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qtp.birdmap.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ddd.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://byf.tianlin.xyz

Ruby: # 无泛型
来源：http://wkb.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://slg.uphjek.com

[C15] 解构 / 展开参数
来源：http://mjk.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mth.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://smz.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nme.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sse.shanyushiyangtech.top

Java: // 无解构
来源：http://plw.yuanzhike.top

Go:   // 无解构
来源：http://cqg.zhixingplan.top


<!-- 参考信息 -->