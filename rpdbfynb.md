代发 wailian999

[A26] 类型转换总览
来源：http://dse.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eev.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vbd.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gga.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://vii.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bmi.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xze.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nih.snrcjt.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://soi.cashguo.top

================================================================================
来源：http://kph.hnxiangtu.top

B. 流程控制
来源：http://yhv.zdqjudy.top

================================================================================
来源：http://vyy.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://rrs.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ibl.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://trj.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vme.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vkx.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://blv.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dmq.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ugv.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bme.jinyuanbaomall.cn

[B02] 多分支 else if / elif
来源：http://dhb.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://laq.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lga.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ffi.cheryme.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hof.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgr.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pcv.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gfa.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnm.0kj1m.cn

[B03] switch / match / case
来源：http://sjz.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kzn.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ojz.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iqe.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ddw.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lbg.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kjr.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lye.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aka.yonumen.top

[B04] for 计数循环
来源：http://bjd.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://wpw.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hqv.yj20258.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vmd.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://etx.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bkv.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xyp.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://scq.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ujc.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://pdf.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://jct.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qgl.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xmc.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iot.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zri.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aqw.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://kaa.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lng.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://hsw.pengpengdd.cyou

Py:   for k, v in d.items(): print(k, v)
来源：http://jtx.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zwr.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwe.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://frf.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gpf.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ybc.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fob.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pgw.birdmap.top

[B07] while 循环
来源：http://plk.hnxiangtu.top

Py:   while i < 10: i += 1
来源：http://vmb.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dfz.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://jyo.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://fec.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://dft.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zrd.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://dai.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://xwb.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://jdz.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://chn.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eon.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://ssl.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://sal.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://qah.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hxq.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://pct.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://ezl.xylfe.cn

[B09] break 与 continue
来源：http://vmq.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fig.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kmi.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pio.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bra.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mld.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gti.zhongyouzk.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kcp.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mfb.cheryme.top

[B10] 遍历同时拿索引
来源：http://bne.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bdy.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://efw.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://noc.cheryme.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mae.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://olk.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zqy.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://twx.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pvg.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://bfm.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://nzj.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://tnp.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://owk.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://isq.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nfv.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mau.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://vyg.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mkk.birdmap.top

[B12] 跳出多层循环
来源：http://rgk.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mzj.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://smy.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dig.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://njc.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zql.cashguo.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zzx.zhengqikj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aaf.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qhh.shuidangran.top

[B13] 判断是否为数字
来源：http://pnd.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://tzg.jqgfzy.top

PHP:  is_numeric($x)
来源：http://irt.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sma.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wxs.gogol.net.cn

Java: x instanceof Number
来源：http://ple.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://byy.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://zym.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://tia.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://hfh.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yiz.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://afp.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://ghn.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://dut.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fyd.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cqz.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rsf.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ots.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://hma.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://auo.havefunace.top

PHP:  $a && $b || !$c
来源：http://zad.fanxiaobao.xyz

JS:   a && b || !c
来源：http://wkw.hcnkem.com

TS:   a && b || !c
来源：http://ytr.jiagoushi.top

Java: a && b || !c
来源：http://dhs.ehwqpu.com

Go:   a && b || !c
来源：http://yad.kuanghao11.cn

Ruby: a && b || !c
来源：http://xzi.gogol.net.cn

C#:   a && b || !c
来源：http://ikp.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://qlt.zhixingplan.top

Py:   if not data: return
来源：http://xed.hammf.cn

PHP:  if (!$data) { return; }
来源：http://yyp.guowangkeji.top

JS:   if (!data) return;
来源：http://pke.ehwqpu.com

TS:   if (!data) return;
来源：http://zjp.redwolf501.top

Java: if (data == null) return;
来源：http://udy.sysykeji.top

Go:   if data == nil { return }
来源：http://mqh.hywenlv.cn

Ruby: return if data.nil?
来源：http://pwd.yuanzhike.top

C#:   if (data == null) return;
来源：http://fok.shzxlz.cn

================================================================================
来源：http://fmy.vqdsnc.cn

C. 函数与作用域
来源：http://nmq.tarul.cn

================================================================================
来源：http://ajr.wangshuangyany.cn

[C01] 定义函数
来源：http://roj.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://hvg.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybv.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://avk.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lfr.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ycg.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ygg.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://ftz.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dux.guannengcc.top

[C02] 默认参数
来源：http://snl.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://xys.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pbb.shzxlz.cn

JS:   function greet(name = "World") { return name; }
来源：http://xom.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://ckh.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bmt.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rgm.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://bsi.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://jcb.snrcjt.cn

[C03] 可变参数
来源：http://dzp.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://jxm.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bve.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ljq.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zqh.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://htm.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cka.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xfs.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eje.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://xqv.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iqn.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ydp.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cgc.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://npt.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://pao.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://dof.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://rat.sweek.top

C#:   f(a: 1, b: 2)
来源：http://fzi.zhijiandao.cn

[C05] 返回多个值
来源：http://zkj.nanxinkj.top

Py:   return a, b
来源：http://liy.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://ofx.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://dvx.yfazqb.com

TS:   return { a, b };
来源：http://qju.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rpi.zhijiandao.cn

Go:   return a, b
来源：http://aja.zhijiandao.cn

Ruby: return a, b
来源：http://kkq.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://roy.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://fvx.fengsongda.top

Py:   square = lambda x: x * x
来源：http://khk.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mpy.hysaishi.cn

JS:   const square = x => x * x;
来源：http://kww.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://fnt.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jwd.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://jdu.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://nbp.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://pir.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://ukw.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://azz.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://hxu.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aem.birdmap.top

TS:   arr.map(String)
来源：http://hba.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://spn.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eet.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://yaj.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iyt.uphjek.com

[C08] 闭包
来源：http://mtn.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://byb.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pes.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pky.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fxq.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wgi.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gem.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mnp.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gcj.zhaomingkeji.xyz

[C09] 递归
来源：http://azn.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nuu.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zfw.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://val.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dri.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pwa.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uaa.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vzv.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tds.daria6918.cn

[C10] 变量作用域
来源：http://fqm.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lky.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gvs.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jgb.tanke756.top

TS:   同 JS
来源：http://ozt.0kj1m.cn

Java: 方法内为块级作用域
来源：http://ugt.yueranfly.top

Go:   花括号块级作用域
来源：http://kfh.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vzt.hnqzz.top

C#:   块级作用域
来源：http://xjb.cqqwz.cn

[C11] 模块导入与导出
来源：http://atg.shanyushiyangtech.top

Py:   from module import func
来源：http://qtb.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nkd.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wtg.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yne.xinyue.icu

Java: import java.util.List;
来源：http://gle.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zqw.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://xbh.jiagoushi.top

C#:   using System.Text;
来源：http://exp.sweek.top

[C12] 立即执行函数 IIFE
来源：http://jfg.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://svg.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://nir.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://iva.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://aqv.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mep.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://hwy.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://ify.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cwh.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://pic.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sac.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pxi.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rkw.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ysk.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kej.dianchejie.cn

Go:   func add(a, b int) int
来源：http://gbo.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqn.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://qgn.cashguo.top

[C14] 泛型函数
来源：http://jnn.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lkk.xuanzx.com

PHP:  // 无泛型
来源：http://lfu.andypj.xyz

JS:   // 无泛型
来源：http://thm.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eyi.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vxv.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kiv.jinqigufen.top

Ruby: # 无泛型
来源：http://gns.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rmd.cheryme.top

[C15] 解构 / 展开参数
来源：http://not.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pyc.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://ido.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cyg.hnqzz.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zvx.dashuyun.cn

Java: // 无解构
来源：http://vpw.cdnleiting.top

Go:   // 无解构
来源：http://jtn.hywenlv.cn

Ruby: a, b = pair
来源：http://pin.mhx1999.top

C#:   var (a, b) = pair;
来源：http://ult.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://ytq.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lqw.hammf.cn

PHP:  // 无重载
来源：http://cww.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oqe.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://ylv.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://luj.yonumen.top


<!-- 参考信息 -->