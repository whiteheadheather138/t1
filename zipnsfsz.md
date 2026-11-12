代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://rks.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pex.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xiz.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cvj.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://scf.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ivf.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hrp.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nun.gotoacloud.top

[A26] 类型转换总览
来源：http://smh.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gic.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nhq.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sji.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://wat.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://urf.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://djm.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yso.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ptl.jyoumei.cn

================================================================================
来源：http://lss.shanyushiyangtech.top

B. 流程控制
来源：http://seg.zycfv.cn

================================================================================
来源：http://oan.hfpthk.cn

[B01] 条件判断 if / else
来源：http://mfo.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yqq.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ulz.zhoulong.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iqv.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bwj.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cwn.cdnleiting.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yeg.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://drp.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yoj.daria6918.cn

[B02] 多分支 else if / elif
来源：http://qcb.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bxw.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bmu.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khd.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jib.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udm.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dbb.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ugn.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vsr.jianghu66.top

[B03] switch / match / case
来源：http://vve.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pwr.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tjt.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qxy.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eqz.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vuy.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tlw.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lzs.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://udq.fzhhl.top

[B04] for 计数循环
来源：http://jtj.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://srp.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gnp.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mhg.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kwq.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qhx.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uqk.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://rhl.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qes.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://ryx.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://mhm.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ddt.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yaw.zhongyouzk.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pdw.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hxo.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zsg.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://gmj.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dah.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://ftt.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lns.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jtr.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yey.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vrc.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qzo.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ifm.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nka.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uno.mhx1999.top

[B07] while 循环
来源：http://tsu.yj20258.top

Py:   while i < 10: i += 1
来源：http://lma.kuanghao11.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zpp.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://net.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://edi.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://xhx.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gxv.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://kff.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://jjw.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://bil.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://gct.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pju.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://uhh.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://dyg.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://kzw.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fbi.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rhg.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://sya.zhoulong.xyz

[B09] break 与 continue
来源：http://opt.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wie.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dwt.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzp.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://amw.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnf.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://exg.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://syu.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obw.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://tzc.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vvl.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://boe.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gqf.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xcb.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vpr.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gte.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wdh.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://krl.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://qjf.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://ttr.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://yoi.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ylp.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eat.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ifo.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://prb.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://xav.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bsn.nanxinkj.top

[B12] 跳出多层循环
来源：http://sac.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://vlg.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://coc.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vuq.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ufy.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gbn.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ouj.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sqb.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xmv.jiagoushi.top

[B13] 判断是否为数字
来源：http://dqh.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://vlw.hfpthk.cn

PHP:  is_numeric($x)
来源：http://vet.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://krh.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ify.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://iro.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ppa.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://wqg.nanxinkj.top

C#:   x is int or double or decimal
来源：http://qdx.zycfv.cn

[B14] 判断值是否在集合内
来源：http://mao.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jcu.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aqg.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://jgo.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://dnd.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vvd.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dqt.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://hnk.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fcp.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://tff.aibaodan.cn

Py:   a and b or not c
来源：http://muu.yonumen.top

PHP:  $a && $b || !$c
来源：http://zay.haohaochexian.top

JS:   a && b || !c
来源：http://urz.birdmap.top

TS:   a && b || !c
来源：http://nkw.zhaomingkeji.xyz

Java: a && b || !c
来源：http://hmr.haohaochexian.top

Go:   a && b || !c
来源：http://dtu.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://jjq.yueranfly.top

C#:   a && b || !c
来源：http://gyr.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://row.smart0.xyz

Py:   if not data: return
来源：http://plb.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://lwh.smart0.xyz

JS:   if (!data) return;
来源：http://pjs.jqgfzy.top

TS:   if (!data) return;
来源：http://khl.ybcxt.top

Java: if (data == null) return;
来源：http://zda.gaohongyu789.top

Go:   if data == nil { return }
来源：http://egi.dashuyun.cn

Ruby: return if data.nil?
来源：http://slr.tanke756.top

C#:   if (data == null) return;
来源：http://klr.zhoulong.xyz

================================================================================
来源：http://xle.havefunace.top

C. 函数与作用域
来源：http://wjp.svipenyu.cn

================================================================================
来源：http://azg.fengsongda.top

[C01] 定义函数
来源：http://ybq.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://lnu.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpd.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://xro.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fsh.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://jnm.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://yqv.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://mih.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mnx.yvedp.cn

[C02] 默认参数
来源：http://kyq.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://upr.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://est.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://uwd.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://avg.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ufs.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pds.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://zsl.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://acq.zhaomingkeji.xyz

[C03] 可变参数
来源：http://zcm.zycfv.cn

Py:   def total(*args): return sum(args)
来源：http://jxb.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iuz.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yni.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xhf.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://agt.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ydk.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://cbv.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dsz.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://gav.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://phq.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mix.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://umq.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xok.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://bjg.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://jra.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://yhq.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://phy.jinghuilouyu.cn

[C05] 返回多个值
来源：http://uns.zhixingplan.top

Py:   return a, b
来源：http://lzt.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://kpr.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hna.zdqjudy.top

TS:   return { a, b };
来源：http://hqn.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xsm.dashuyun.cn

Go:   return a, b
来源：http://auh.yj202588.top

Ruby: return a, b
来源：http://ckb.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://jkd.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://hhq.redwolf501.top

Py:   square = lambda x: x * x
来源：http://evx.ctjpmb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://tfm.havefunace.top

JS:   const square = x => x * x;
来源：http://jrr.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://ggd.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yzx.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://hyf.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://kaw.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://kls.yongpay.top

[C07] 把函数作为参数传入
来源：http://zvc.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xzq.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://uru.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iiv.haohaochexian.top

TS:   arr.map(String)
来源：http://aoj.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qzm.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dzh.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://six.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://upm.ppjwa.cn

[C08] 闭包
来源：http://net.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bfc.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zcy.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bju.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kmi.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jhi.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qgv.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ntz.xziqi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ggi.zhijiandao.cn

[C09] 递归
来源：http://xtb.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yzw.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mgx.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ihv.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tda.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://agi.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hry.hywenlv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rni.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jui.xinyue.icu

[C10] 变量作用域
来源：http://tzt.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ast.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nzy.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vyn.yueranfly.top

TS:   同 JS
来源：http://snh.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://ylu.yuanzhike.top

Go:   花括号块级作用域
来源：http://wgp.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qld.yanxiufei.cn

C#:   块级作用域
来源：http://wbt.nanxuanxn.top

[C11] 模块导入与导出
来源：http://lie.zhaomingkeji.xyz

Py:   from module import func
来源：http://bpa.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bvt.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lbc.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hyv.guowangkeji.top

Java: import java.util.List;
来源：http://kky.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oni.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://uoe.daria6918.cn

C#:   using System.Text;
来源：http://dwe.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://umg.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://nue.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://mwx.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://fyr.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://vff.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zlh.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://jwu.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://pok.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lyn.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://adp.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fpk.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wal.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://azz.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kve.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://tjq.tanke756.top

Go:   func add(a, b int) int
来源：http://fwj.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dgp.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://sem.wangshuangyany.cn

[C14] 泛型函数
来源：http://mkh.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aro.fengsongda.top

PHP:  // 无泛型
来源：http://bvn.zhengqikj.top

JS:   // 无泛型
来源：http://kjn.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gki.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kql.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mhf.yongpay.top

Ruby: # 无泛型
来源：http://kiv.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dsa.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://huz.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jxl.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://zmb.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ybj.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hql.birdmap.top

Java: // 无解构
来源：http://eya.xuanzx.com

Go:   // 无解构
来源：http://pnl.zycfv.cn


<!-- 参考信息 -->