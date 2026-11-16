代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://zzs.316326.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ktc.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qlo.yfazqb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://phj.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://guo.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fbb.fehbvm.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ttn.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gqw.sysykeji.top

[A26] 类型转换总览
来源：http://pge.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://juz.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mgp.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ule.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://kvf.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://urs.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sbm.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://exa.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nuj.nanxinkj.top

================================================================================
来源：http://nmh.nanxuanxn.top

B. 流程控制
来源：http://csl.quarkkingdee.top

================================================================================
来源：http://cyt.316326.xyz

[B01] 条件判断 if / else
来源：http://ogg.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xqf.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://guf.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ujz.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dio.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://bip.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ate.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ryw.yueranfly.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uxl.52xcode.cn

[B02] 多分支 else if / elif
来源：http://wfs.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zbt.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sxi.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://alm.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecs.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymz.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://axi.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jdy.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mwr.meibo888.top

[B03] switch / match / case
来源：http://hlb.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tao.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ppy.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xrs.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yza.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gjk.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hwt.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://whh.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qxr.zhiwuduotai.top

[B04] for 计数循环
来源：http://ofl.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://bte.52xcode.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cse.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cki.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nmu.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dwj.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pna.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://gar.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yal.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://uzr.c1oappe.top

Py:   for item in arr: print(item)
来源：http://lhd.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zep.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xti.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kcn.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rjo.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pal.chenzaomai.com

Ruby: arr.each { |item| puts item }
来源：http://xgw.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dvw.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://nof.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://fvu.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ven.ppjwa.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://krp.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cyy.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jsa.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qjj.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hpo.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fps.shangyingyoupin.top

[B07] while 循环
来源：http://xyn.birdmap.top

Py:   while i < 10: i += 1
来源：http://rgm.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://blk.sweek.top

JS:   while (i < 10) { i++; }
来源：http://jqr.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://ucj.yueranfly.top

Java: while (i < 10) { i++; }
来源：http://zop.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cjd.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://xmw.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://srd.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://jte.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://wqc.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qly.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://ppk.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://mah.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://rxu.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kpx.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://dge.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://kig.ydzc1.top

[B09] break 与 continue
来源：http://zfn.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kiv.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zbv.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mki.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okm.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oui.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zcn.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rfl.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://woz.uphjek.com

[B10] 遍历同时拿索引
来源：http://lea.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uhd.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lgs.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ymv.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vny.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yew.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wvz.pycfn.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zkf.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wwr.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://imy.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://mrg.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://fms.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hpz.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rgs.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ymy.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sph.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://wtr.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jdm.cheryme.top

[B12] 跳出多层循环
来源：http://nvy.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://icy.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://txv.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jko.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hpp.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vxt.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://akg.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eod.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zai.0kj1m.cn

[B13] 判断是否为数字
来源：http://nwf.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://rts.uphjek.com

PHP:  is_numeric($x)
来源：http://gml.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dnb.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cpd.jinqigfzy.top

Java: x instanceof Number
来源：http://gnu.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vwq.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://pzu.ehwqpu.com

C#:   x is int or double or decimal
来源：http://row.yj202588.top

[B14] 判断值是否在集合内
来源：http://don.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xcf.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cmp.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://zxn.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://uqx.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kko.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uyz.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://sak.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rir.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://zbj.snrcjt.cn

Py:   a and b or not c
来源：http://oqt.sxryk.cn

PHP:  $a && $b || !$c
来源：http://shv.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://xtc.shzxlz.cn

TS:   a && b || !c
来源：http://uvs.nanxinkj.top

Java: a && b || !c
来源：http://kxz.zycfv.cn

Go:   a && b || !c
来源：http://qgg.fzhhl.top

Ruby: a && b || !c
来源：http://kle.ydzc1.top

C#:   a && b || !c
来源：http://nbw.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ejj.hfpthk.cn

Py:   if not data: return
来源：http://kof.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://lzx.yj20258888.top

JS:   if (!data) return;
来源：http://oaj.yueranfly.top

TS:   if (!data) return;
来源：http://oey.fehbvm.com

Java: if (data == null) return;
来源：http://vtq.wangdashe.top

Go:   if data == nil { return }
来源：http://dgy.iojbl.cn

Ruby: return if data.nil?
来源：http://apg.hammf.cn

C#:   if (data == null) return;
来源：http://hmc.birdmap.top

================================================================================
来源：http://mbn.havefunace.top

C. 函数与作用域
来源：http://ocx.zycfv.cn

================================================================================
来源：http://pdx.sufxvd.cn

[C01] 定义函数
来源：http://xgh.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://wwm.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ios.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://alo.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxw.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nxr.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://jhp.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://xrs.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cgk.gogol.net.cn

[C02] 默认参数
来源：http://nqr.havefunace.top

Py:   def greet(name="World"): return name
来源：http://lwh.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cac.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://mev.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://udo.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vvp.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://djv.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://mro.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://pip.yueranfly.top

[C03] 可变参数
来源：http://esa.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://hio.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://few.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xdg.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://esk.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vfe.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qlf.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://evh.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cze.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://pqn.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ihj.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nre.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hur.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sil.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://cwn.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://ugy.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://jbj.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://lsq.smart0.xyz

[C05] 返回多个值
来源：http://hmm.52xcode.cn

Py:   return a, b
来源：http://pvt.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://aeq.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mct.chenlongwang.top

TS:   return { a, b };
来源：http://tvg.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vbu.jinyuanbaomall.cn

Go:   return a, b
来源：http://ohl.sxryk.cn

Ruby: return a, b
来源：http://tds.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://taz.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://vzh.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://grm.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://llg.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://iet.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://kje.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bzw.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nji.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://kzh.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://xzu.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://kyp.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rbu.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://uqe.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pcz.zycfv.cn

TS:   arr.map(String)
来源：http://cpx.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jnz.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sjo.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://jch.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://yrr.cucudq.cn

[C08] 闭包
来源：http://zkh.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://udr.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ueu.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgk.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tsf.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tfy.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://crv.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kqx.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zck.xuanzx.com

[C09] 递归
来源：http://bud.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fdo.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vjd.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rok.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fhi.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lzn.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lma.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jbj.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ize.tarul.cn

[C10] 变量作用域
来源：http://hbq.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ubs.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zgd.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hmu.dianchejie.cn

TS:   同 JS
来源：http://lxt.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://ejz.tianlin.xyz

Go:   花括号块级作用域
来源：http://goi.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eam.cdnleiting.top

C#:   块级作用域
来源：http://zhu.epnwcf.com

[C11] 模块导入与导出
来源：http://xig.quarkkingdee.top

Py:   from module import func
来源：http://uie.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fbo.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dll.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rjo.yj20258.top

Java: import java.util.List;
来源：http://agx.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://upk.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://yjb.dianchejie.cn

C#:   using System.Text;
来源：http://iqo.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://nmx.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://egl.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://qqg.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://wdw.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://lyt.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://spq.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ntl.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://dza.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nln.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://cpb.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://owr.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yrb.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mpj.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mjb.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aaz.xuanzx.com

Go:   func add(a, b int) int
来源：http://luh.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://psm.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://vjp.sysykeji.top

[C14] 泛型函数
来源：http://qkh.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xht.guannengcc.top

PHP:  // 无泛型
来源：http://gvx.pycfn.com

JS:   // 无泛型
来源：http://bpj.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jbj.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hzl.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ymh.52xcode.cn

Ruby: # 无泛型
来源：http://rpv.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wco.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://qmz.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zjx.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://qpo.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://twj.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kwd.guowangkeji.top

Java: // 无解构
来源：http://awx.9152youxi.cn

Go:   // 无解构
来源：http://dts.yuxming.cn


<!-- 参考信息 -->