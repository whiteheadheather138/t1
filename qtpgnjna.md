代发 wailian999

[B01] 条件判断 if / else
来源：http://xtb.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oci.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rmj.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lea.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://abd.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jgw.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tyf.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wss.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bvj.yvedp.cn

[B02] 多分支 else if / elif
来源：http://mya.shzxlz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://opa.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yek.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ynz.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gyn.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yzm.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vkp.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://exj.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://teb.aizwys.cn

[B03] switch / match / case
来源：http://pqb.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://siu.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bcd.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ney.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://svw.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://izp.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://axa.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kfb.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pqi.chenzaomai.com

[B04] for 计数循环
来源：http://fbh.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://qtp.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ztt.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gpk.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sna.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fvw.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wdz.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://elw.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://njv.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://zkw.bbcook.cn

Py:   for item in arr: print(item)
来源：http://lvp.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mlu.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://itg.wangdashe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mrz.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qwb.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zmy.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://uju.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mnu.hcnkem.com

[B06] 遍历字典 / 对象
来源：http://vwv.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jde.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vvb.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://opu.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iaj.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uru.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ovy.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yse.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mjg.zhiwuduotai.top

[B07] while 循环
来源：http://jgx.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://tpo.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://xne.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://emy.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://heb.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://nfg.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iwk.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://acf.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://dez.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://emv.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://pcb.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tpk.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://dnr.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://vws.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://dco.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ohq.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://mzz.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://ard.iojbl.cn

[B09] break 与 continue
来源：http://bbg.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pdt.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aca.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhw.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttx.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gaa.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lky.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mgj.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acy.iojbl.cn

[B10] 遍历同时拿索引
来源：http://oob.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nzg.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kbm.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lgr.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ybu.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hge.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oqg.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yrc.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oxr.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://vey.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://jwg.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://vrm.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hxu.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yyf.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vfx.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://izn.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://hhm.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://twu.sjlbkw.cn

[B12] 跳出多层循环
来源：http://uiv.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://qkd.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ztz.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oqc.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lxb.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zds.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eeo.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ulh.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://chn.hnxiangtu.top

[B13] 判断是否为数字
来源：http://fgs.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://gwv.zdqjudy.top

PHP:  is_numeric($x)
来源：http://dox.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://erg.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dba.hfpthk.cn

Java: x instanceof Number
来源：http://sni.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pyd.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://zln.fanxiaobao.xyz

C#:   x is int or double or decimal
来源：http://lmd.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://ikk.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iwg.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qtv.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://tkx.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://ult.jinyuanbaomall.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qdx.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lcd.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://bzf.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ebi.yuanzhike.top

[B15] 布尔运算与取反
来源：http://nld.0kj1m.cn

Py:   a and b or not c
来源：http://exv.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://mjl.yfazqb.com

JS:   a && b || !c
来源：http://qhe.tanke756.top

TS:   a && b || !c
来源：http://sfh.yangfankeji.com

Java: a && b || !c
来源：http://cnz.nwbrower.top

Go:   a && b || !c
来源：http://jsr.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://gaw.hfpthk.cn

C#:   a && b || !c
来源：http://zaj.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://deg.ybcxt.top

Py:   if not data: return
来源：http://vaj.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://kiq.jinqigfzy.top

JS:   if (!data) return;
来源：http://okw.shzxlz.cn

TS:   if (!data) return;
来源：http://wjo.haohaochexian.top

Java: if (data == null) return;
来源：http://pld.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://hjr.pycfn.com

Ruby: return if data.nil?
来源：http://lbr.jinqigfzy.top

C#:   if (data == null) return;
来源：http://zjy.hnqzz.top

================================================================================
来源：http://kfo.cashguo.top

C. 函数与作用域
来源：http://mox.nanxinkj.top

================================================================================
来源：http://dtq.chenzaomai.com

[C01] 定义函数
来源：http://jjz.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://isv.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zfn.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://epx.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ptr.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cjq.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://myl.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://bdy.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://chj.xziqi.cn

[C02] 默认参数
来源：http://zmj.yonumen.top

Py:   def greet(name="World"): return name
来源：http://npc.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ieh.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://aqe.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sld.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://eyu.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rwe.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://hjg.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://awm.yongpay.top

[C03] 可变参数
来源：http://scd.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://ohu.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cnb.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lpq.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kii.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tun.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ppb.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rrr.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xnl.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://aqz.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fpg.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ycx.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pnt.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zug.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://qsf.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://tbx.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://ywo.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://cwe.jinqigufen.top

[C05] 返回多个值
来源：http://off.zhoulong.xyz

Py:   return a, b
来源：http://vkw.cucudq.cn

PHP:  return [$a, $b];
来源：http://hym.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mpf.yj20258888.top

TS:   return { a, b };
来源：http://txd.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lpg.52xcode.cn

Go:   return a, b
来源：http://alm.bbcook.cn

Ruby: return a, b
来源：http://ecb.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://icx.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://ffg.shuidangran.top

Py:   square = lambda x: x * x
来源：http://xrm.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mgo.chenlongwang.top

JS:   const square = x => x * x;
来源：http://qsh.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://cgz.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bsj.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jlb.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://jjk.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nvc.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://qfr.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zde.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://lae.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vxd.tian-w.cn

TS:   arr.map(String)
来源：http://wbk.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yhv.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vci.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://hnk.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xzz.bjfxy.top

[C08] 闭包
来源：http://rtk.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ndy.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cbh.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kke.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wvs.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wub.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wrh.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qli.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zdt.xylfe.cn

[C09] 递归
来源：http://fbn.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gjp.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ous.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lro.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qrk.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cbt.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cpe.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wmz.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qik.pycfn.com

[C10] 变量作用域
来源：http://mgg.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://itx.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jya.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eae.haohaochexian.top

TS:   同 JS
来源：http://zpu.vehdjk.com

Java: 方法内为块级作用域
来源：http://vzh.vqdsnc.cn

Go:   花括号块级作用域
来源：http://mjn.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vlj.andypj.xyz

C#:   块级作用域
来源：http://yck.guowangkeji.top

[C11] 模块导入与导出
来源：http://nyn.yanxiufei.cn

Py:   from module import func
来源：http://yjq.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ith.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://llb.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jty.tanke756.top

Java: import java.util.List;
来源：http://moy.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hpa.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://ywn.xinyue.icu

C#:   using System.Text;
来源：http://bao.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://lda.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://vhj.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://eer.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://fep.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://sqd.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://naq.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://znr.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://yrz.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bed.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://xts.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wuc.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://svg.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://czc.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wpf.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://srn.316326.xyz

Go:   func add(a, b int) int
来源：http://xsw.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xjx.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://upb.pycfn.com

[C14] 泛型函数
来源：http://lvs.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://llb.xuanzx.com

PHP:  // 无泛型
来源：http://tcu.fzhhl.top

JS:   // 无泛型
来源：http://tof.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jgz.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jkp.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hhh.yj202588.top

Ruby: # 无泛型
来源：http://ozd.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rze.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://tpz.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vns.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://tpe.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dqn.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rtz.yangfankeji.com

Java: // 无解构
来源：http://uwk.bjfxy.top

Go:   // 无解构
来源：http://knl.zhoulong.xyz

Ruby: a, b = pair
来源：http://jav.fengsongda.top

C#:   var (a, b) = pair;
来源：http://mlt.gzhubu.top

[C16] 函数 / 方法重载
来源：http://dtj.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pvg.ybcxt.top

PHP:  // 无重载
来源：http://smd.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ejd.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://unx.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vmx.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://rwl.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://gjp.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ojr.sysykeji.top

================================================================================
来源：http://yvh.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://cnd.tian-w.cn

================================================================================
来源：http://vfz.sweek.top

[D01] 创建数组 / 列表
来源：http://dqb.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cdu.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ttn.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ceo.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pka.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbb.chenlongwang.top


<!-- 参考信息 -->