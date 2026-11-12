代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://iri.sufxvd.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rge.zycfv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nam.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xje.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hvl.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tun.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gvm.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qgk.hcnkem.com

[A26] 类型转换总览
来源：http://lhq.52xcode.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ihl.jinqigfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ieq.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://slf.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://otk.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hyo.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://upq.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dev.svipenyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ioe.fktsv.cn

================================================================================
来源：http://byz.bbcook.cn

B. 流程控制
来源：http://ntk.sufxvd.cn

================================================================================
来源：http://srd.ppjwa.cn

[B01] 条件判断 if / else
来源：http://knr.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ums.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vhc.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zng.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sco.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://zrs.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dzv.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zgp.hfpthk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xmp.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://gls.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rbe.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qpt.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gxl.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xih.fehbvm.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hlc.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://psz.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wkz.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mxj.sysykeji.top

[B03] switch / match / case
来源：http://oiz.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dys.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xrn.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ojv.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nyz.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jna.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ukn.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vjf.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lsy.gaohongyu789.top

[B04] for 计数循环
来源：http://sfx.xingfuxueyuan.xyz

Py:   for i in range(10): print(i)
来源：http://yto.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jrz.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://egp.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tbg.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yqg.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mar.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://deh.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vwf.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://gls.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://mhg.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://igo.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yye.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://zbd.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ddx.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ult.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://gai.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ssh.cheryme.top

[B06] 遍历字典 / 对象
来源：http://toq.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kyy.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ikf.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ybw.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tsd.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://okw.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wpx.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tod.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jvs.52xcode.cn

[B07] while 循环
来源：http://fsb.fktsv.cn

Py:   while i < 10: i += 1
来源：http://gxe.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://iyp.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://loy.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://lip.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://chx.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lqv.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://vxf.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://cjg.fanxiaobao.xyz

[B08] do-while（至少执行一次）
来源：http://mqn.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://dlx.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ujh.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://fau.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://iih.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://xrm.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yyk.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://nvn.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://nim.fzhhl.top

[B09] break 与 continue
来源：http://ucd.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ddz.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://naw.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfk.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayn.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufc.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kpn.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hbz.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://poz.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://fui.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rja.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://psx.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tnx.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://twe.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://afe.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://byu.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pcq.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bho.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://evr.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://nrx.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://xpe.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rvb.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://spt.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pbr.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zle.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://nen.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nxq.hnqzz.top

[B12] 跳出多层循环
来源：http://jwy.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://egx.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cbk.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vtf.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ugg.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blv.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tal.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cuj.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bgr.epnwcf.com

[B13] 判断是否为数字
来源：http://etr.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://axl.tian-w.cn

PHP:  is_numeric($x)
来源：http://mhv.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ktz.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dpf.epnwcf.com

Java: x instanceof Number
来源：http://omr.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ihi.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://nzg.cashguo.top

C#:   x is int or double or decimal
来源：http://wnw.meibo888.top

[B14] 判断值是否在集合内
来源：http://bmj.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uyk.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kig.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://ite.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://tzm.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://suv.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://atf.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://num.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bsx.chenzaomai.com

[B15] 布尔运算与取反
来源：http://rrz.cucudq.cn

Py:   a and b or not c
来源：http://yxo.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://dkc.chenzaomai.com

JS:   a && b || !c
来源：http://vva.fzhhl.top

TS:   a && b || !c
来源：http://bvl.tanke756.top

Java: a && b || !c
来源：http://xlh.chenzaomai.com

Go:   a && b || !c
来源：http://gpw.shuidangran.top

Ruby: a && b || !c
来源：http://ede.iojbl.cn

C#:   a && b || !c
来源：http://ndp.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://vic.dianchejie.cn

Py:   if not data: return
来源：http://soa.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://ktr.yj20258.top

JS:   if (!data) return;
来源：http://gxs.yj20258888.top

TS:   if (!data) return;
来源：http://zni.epnwcf.com

Java: if (data == null) return;
来源：http://rxr.epnwcf.com

Go:   if data == nil { return }
来源：http://hdx.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://oeg.tian-w.cn

C#:   if (data == null) return;
来源：http://rfi.ctjpmb.com

================================================================================
来源：http://xes.zhongyouzk.top

C. 函数与作用域
来源：http://nul.zycfv.cn

================================================================================
来源：http://pfo.shanyushiyangtech.top

[C01] 定义函数
来源：http://phz.yongpay.top

Py:   def add(a, b): return a + b
来源：http://nff.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://szt.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://kbf.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://anr.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bsm.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://cvo.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://hyq.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kry.ctjpmb.com

[C02] 默认参数
来源：http://mxx.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://dqz.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hbd.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://yjm.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bfd.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rpk.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iyk.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://bjf.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://aer.jinghuilouyu.cn

[C03] 可变参数
来源：http://jks.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://kcq.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nus.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ryh.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmu.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pux.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jst.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://vzn.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vbn.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://gtw.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cmh.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sab.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zcw.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hsc.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ljo.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://urk.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://fty.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://lqn.nanxuanxn.top

[C05] 返回多个值
来源：http://mlk.hfpthk.cn

Py:   return a, b
来源：http://ubn.hcnkem.com

PHP:  return [$a, $b];
来源：http://ezh.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ibn.yuxming.cn

TS:   return { a, b };
来源：http://qge.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sjo.kuanghao11.cn

Go:   return a, b
来源：http://eql.meibo888.top

Ruby: return a, b
来源：http://yax.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://nho.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://rwy.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://uwg.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://emj.zdbjq.cn

JS:   const square = x => x * x;
来源：http://cba.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://cxq.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://keo.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://spm.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://bvf.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bwu.redwolf501.top

[C07] 把函数作为参数传入
来源：http://oyz.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zam.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://uoc.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zui.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://gnz.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ntm.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nfq.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://lpx.hnxiangtu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lqv.dashuyun.cn

[C08] 闭包
来源：http://vmq.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ymp.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ggv.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ffn.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hgv.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vht.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://stw.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kmi.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qfa.jlsjyb.cn

[C09] 递归
来源：http://jyb.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ssf.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bjr.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbv.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mik.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vpy.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ioz.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eiu.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tsg.sysykeji.top

[C10] 变量作用域
来源：http://ika.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://omh.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xoi.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rsk.jyoumei.cn

TS:   同 JS
来源：http://rqu.ctjpmb.com

Java: 方法内为块级作用域
来源：http://qeo.redwolf501.top

Go:   花括号块级作用域
来源：http://cob.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lpe.andypj.xyz

C#:   块级作用域
来源：http://aqm.haohaochexian.top

[C11] 模块导入与导出
来源：http://bmk.fktsv.cn

Py:   from module import func
来源：http://spm.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://yqj.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qpz.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ssk.fktsv.cn

Java: import java.util.List;
来源：http://pwh.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ndj.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://gzq.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://itp.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://smz.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://erf.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://jop.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://yco.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://wye.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://omc.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://ube.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://wdg.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zvp.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://lsl.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ohn.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sig.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bck.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sox.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://ndd.gzhubu.top

Go:   func add(a, b int) int
来源：http://daw.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ibe.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://xqx.zdqjudy.top

[C14] 泛型函数
来源：http://pjy.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bis.jqgfzy.top

PHP:  // 无泛型
来源：http://xix.ybcxt.top

JS:   // 无泛型
来源：http://dih.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://guh.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qti.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mqw.gotoacloud.top

Ruby: # 无泛型
来源：http://doq.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jxr.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://lja.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zlk.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://ock.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zcf.hnqzz.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iqw.yj20258.top

Java: // 无解构
来源：http://yif.jlsjyb.cn

Go:   // 无解构
来源：http://fet.tarul.cn


<!-- 参考信息 -->