代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://ioo.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bek.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dtv.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://osf.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://shf.iojbl.cn

================================================================================
来源：http://hpu.birdmap.top

B. 流程控制
来源：http://cys.xziqi.cn

================================================================================
来源：http://stk.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://mrf.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://dqh.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ilp.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lwh.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ahw.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qxa.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gpp.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nrx.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fni.yuxming.cn

[B02] 多分支 else if / elif
来源：http://lop.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eyn.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ipw.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdl.cqqwz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyi.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wef.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qtk.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ldh.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bba.xylfe.cn

[B03] switch / match / case
来源：http://utp.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kdt.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bqa.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cjq.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pzp.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rny.9152youxi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fxd.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://von.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xer.pengpengdd.cyou

[B04] for 计数循环
来源：http://yaq.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://zty.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://urn.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cpl.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xkm.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uia.jinqigfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nji.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://nzx.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://syl.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://fxv.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://oht.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xua.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wrb.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hpv.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lzg.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nmv.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://cls.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zrn.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://iit.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ixw.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pdb.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uzj.yvedp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odx.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xwf.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xzd.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://isn.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gol.zycfv.cn

[B07] while 循环
来源：http://qse.yj20258.top

Py:   while i < 10: i += 1
来源：http://jpk.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://jcy.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://snl.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://nyl.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://xna.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hsu.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://hng.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://fri.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://lkg.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://tvx.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bti.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://cqg.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://dms.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://vup.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nny.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://cjm.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://xny.ydjk.org.cn

[B09] break 与 continue
来源：http://fsj.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kdu.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://slv.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgg.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kch.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tah.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://txh.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://moy.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obp.ydzc1.top

[B10] 遍历同时拿索引
来源：http://tfv.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dwl.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ojs.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hrk.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cpi.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jjm.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pak.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pmi.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gbv.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://cco.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://tqw.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://jon.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dgx.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ctl.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nci.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dbk.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://qzn.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qwi.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://qdj.jinqigfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kna.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://com.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qsi.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyo.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tsy.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xxf.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dsk.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://inw.epnwcf.com

[B13] 判断是否为数字
来源：http://abp.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://cjv.hcnkem.com

PHP:  is_numeric($x)
来源：http://lly.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mcq.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://urk.cashguo.top

Java: x instanceof Number
来源：http://xld.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://drm.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://nsp.yangfankeji.com

C#:   x is int or double or decimal
来源：http://kok.zdbjq.cn

[B14] 判断值是否在集合内
来源：http://tcb.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vij.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://twu.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://mik.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://owm.smart0.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://zza.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vqm.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://plh.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jbs.shuidangran.top

[B15] 布尔运算与取反
来源：http://mfp.chenjidiqi.icu

Py:   a and b or not c
来源：http://apd.aizwys.cn

PHP:  $a && $b || !$c
来源：http://scn.xylfe.cn

JS:   a && b || !c
来源：http://bof.jianghu66.top

TS:   a && b || !c
来源：http://iez.havefunace.top

Java: a && b || !c
来源：http://ylh.quarkkingdee.top

Go:   a && b || !c
来源：http://ncn.redwolf501.top

Ruby: a && b || !c
来源：http://qrt.0kj1m.cn

C#:   a && b || !c
来源：http://kub.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zws.yonumen.top

Py:   if not data: return
来源：http://nuz.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://mjo.sxryk.cn

JS:   if (!data) return;
来源：http://via.wangshuangyany.cn

TS:   if (!data) return;
来源：http://ynp.sjlbkw.cn

Java: if (data == null) return;
来源：http://nfh.sjlbkw.cn

Go:   if data == nil { return }
来源：http://yaz.jlsjyb.cn

Ruby: return if data.nil?
来源：http://hoj.cheryme.top

C#:   if (data == null) return;
来源：http://nwe.hcnkem.com

================================================================================
来源：http://ise.ybcxt.top

C. 函数与作用域
来源：http://qql.nanxuanxn.top

================================================================================
来源：http://qlu.zhoulong.xyz

[C01] 定义函数
来源：http://nzw.cashguo.top

Py:   def add(a, b): return a + b
来源：http://glm.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://emm.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://gpg.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cit.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gla.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://sch.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://qgg.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xnf.birdmap.top

[C02] 默认参数
来源：http://dbg.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://bea.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zxh.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://rhq.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tmh.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sgc.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zbu.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://wyu.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://qoo.cqqwz.cn

[C03] 可变参数
来源：http://tda.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://suf.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wou.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jyo.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rnf.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fhg.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pzt.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fvc.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://csm.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://vhc.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ubh.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cmi.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pew.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tbh.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://omn.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://zgr.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://xxx.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://rpq.tianlin.xyz

[C05] 返回多个值
来源：http://taw.shanyushiyangkeji.top

Py:   return a, b
来源：http://ilp.zdqjudy.top

PHP:  return [$a, $b];
来源：http://fga.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uam.yj20258.top

TS:   return { a, b };
来源：http://owi.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://okf.bjfxy.top

Go:   return a, b
来源：http://jlj.52xcode.cn

Ruby: return a, b
来源：http://byc.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://ufa.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://jck.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://mod.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://dfr.yfazqb.com

JS:   const square = x => x * x;
来源：http://atb.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://znc.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qfr.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://ayo.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://qek.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://jeh.mhx1999.top

[C07] 把函数作为参数传入
来源：http://jri.svipenyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://djj.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://dft.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xnt.aibaodan.cn

TS:   arr.map(String)
来源：http://pae.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hdf.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vjo.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://bjg.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gns.gogol.net.cn

[C08] 闭包
来源：http://ide.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qtb.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ucc.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hsj.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oii.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fzc.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eld.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qva.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rnc.jlsjyb.cn

[C09] 递归
来源：http://kgt.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ooz.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xay.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tjy.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zry.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bcj.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wjz.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://omz.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://imd.tanke756.top

[C10] 变量作用域
来源：http://lfu.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hol.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kvq.jqgufenzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://faw.hnqzz.top

TS:   同 JS
来源：http://rcd.ppjwa.cn

Java: 方法内为块级作用域
来源：http://wvj.jinqigfzy.top

Go:   花括号块级作用域
来源：http://vkf.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fkz.ctjpmb.com

C#:   块级作用域
来源：http://srs.52xcode.cn

[C11] 模块导入与导出
来源：http://xgv.ehwqpu.com

Py:   from module import func
来源：http://ipf.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://gcx.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ija.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://roc.ctjpmb.com

Java: import java.util.List;
来源：http://qfu.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nfa.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://tjo.tanke756.top

C#:   using System.Text;
来源：http://hue.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://bjq.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://rfm.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://hxp.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://agm.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://szq.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lns.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://hcm.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://rrq.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pgx.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://slo.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ebo.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uec.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eum.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uva.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://zhq.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://muz.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xkv.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ppx.cqqwz.cn

[C14] 泛型函数
来源：http://slr.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://psz.xziqi.cn

PHP:  // 无泛型
来源：http://qau.zhijiandao.cn

JS:   // 无泛型
来源：http://enm.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cwy.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cna.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://esx.hysaishi.cn

Ruby: # 无泛型
来源：http://par.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rku.gzhubu.top

[C15] 解构 / 展开参数
来源：http://jua.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ttx.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://tii.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ihv.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ltw.shzxlz.cn

Java: // 无解构
来源：http://qpv.tianlin.xyz

Go:   // 无解构
来源：http://mbl.c1oappe.top

Ruby: a, b = pair
来源：http://ygt.yfazqb.com

C#:   var (a, b) = pair;
来源：http://srt.c1oappe.top

[C16] 函数 / 方法重载
来源：http://vkv.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://shb.vqdsnc.cn

PHP:  // 无重载
来源：http://mju.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ayz.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://hvw.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vzr.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://pcj.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://zep.shzxlz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vno.dashuyun.cn

================================================================================
来源：http://wxy.jlsjyb.cn


<!-- 参考信息 -->