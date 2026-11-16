代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://dfd.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rku.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://syz.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zpn.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://its.snrcjt.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mix.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://swp.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pod.ywan-chungtsiang.top

[A26] 类型转换总览
来源：http://qbz.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uns.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xvo.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aly.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://zfm.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ajq.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://imj.daxiang520.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://esf.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mgp.feifeiyinyue.top

================================================================================
来源：http://enc.yj20258888.top

B. 流程控制
来源：http://wag.bbcook.cn

================================================================================
来源：http://fhv.hnxiangtu.top

[B01] 条件判断 if / else
来源：http://nzy.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qcf.c1oappe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jib.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mcz.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://flx.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ffe.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fck.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mbw.fktsv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fqc.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://upt.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uhc.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qmr.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gcd.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mir.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vsu.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mpb.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qpa.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jih.andypj.xyz

[B03] switch / match / case
来源：http://ixq.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://efm.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dtf.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://muf.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qvm.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yyk.316326.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qvy.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rvn.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uxi.fehbvm.com

[B04] for 计数循环
来源：http://vkd.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://xay.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hsp.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://evk.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uxx.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yhf.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jna.zhoulong.xyz

Ruby: 10.times { |i| puts i }
来源：http://wmd.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dtt.yongpay.top

[B05] 遍历数组 / 列表
来源：http://zoi.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://zrb.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ean.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ghg.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://juh.cashguo.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mxk.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mpq.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://wjr.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kbq.yongpay.top

[B06] 遍历字典 / 对象
来源：http://xbc.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://drr.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://got.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zmg.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ndl.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://htx.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qzw.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qpf.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aou.zycfv.cn

[B07] while 循环
来源：http://luz.xziqi.cn

Py:   while i < 10: i += 1
来源：http://scy.jinqigfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://vdb.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://pio.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://pvi.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://ogw.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://muf.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://ges.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://yqu.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://iql.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://dnd.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ouo.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://lrs.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://vwc.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://pad.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nbv.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zms.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://pwy.hammf.cn

[B09] break 与 continue
来源：http://eny.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dkq.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://npk.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cct.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijd.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyc.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mag.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ida.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gxp.pycfn.com

[B10] 遍历同时拿索引
来源：http://bjd.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://isy.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kvb.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://drf.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gim.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lvs.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vml.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://urs.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lyk.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://vch.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://sly.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://wly.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nyj.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ydo.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mkq.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://idx.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://bso.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vwu.zycfv.cn

[B12] 跳出多层循环
来源：http://xts.yj20258.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://atp.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oyo.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vfv.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nub.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wtb.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uhz.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jgn.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dnx.jlsjyb.cn

[B13] 判断是否为数字
来源：http://qit.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://cce.c1oappe.top

PHP:  is_numeric($x)
来源：http://lpz.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fzb.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sep.wangshuangyany.cn

Java: x instanceof Number
来源：http://xbn.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kol.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://blv.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://xtf.c1oappe.top

[B14] 判断值是否在集合内
来源：http://fmz.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cjm.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yzc.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://exj.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://xsi.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://obu.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://avx.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://itr.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fqa.zdbjq.cn

[B15] 布尔运算与取反
来源：http://aql.tanke756.top

Py:   a and b or not c
来源：http://wgf.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://fnq.fanxiaobao.xyz

JS:   a && b || !c
来源：http://qrb.xylfe.cn

TS:   a && b || !c
来源：http://ceq.sweek.top

Java: a && b || !c
来源：http://yli.ivvv.top

Go:   a && b || !c
来源：http://cvm.epnwcf.com

Ruby: a && b || !c
来源：http://zis.gzhubu.top

C#:   a && b || !c
来源：http://uiz.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://hnx.52xcode.cn

Py:   if not data: return
来源：http://see.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://nwz.hesvh.cn

JS:   if (!data) return;
来源：http://wiu.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://cud.cdnleiting.top

Java: if (data == null) return;
来源：http://aec.yj20258.top

Go:   if data == nil { return }
来源：http://llc.tanke756.top

Ruby: return if data.nil?
来源：http://dnk.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://gfo.jinqigfzy.top

================================================================================
来源：http://vbh.fengsongda.top

C. 函数与作用域
来源：http://iue.andypj.xyz

================================================================================
来源：http://xmv.yuxming.cn

[C01] 定义函数
来源：http://det.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://dcv.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pog.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://pzv.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eka.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lkd.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://ckn.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://ntt.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cod.shangyingyoupin.top

[C02] 默认参数
来源：http://kye.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://mzq.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nzs.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://pim.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fkk.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ybh.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ozr.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://fhr.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://cpd.zhixingplan.top

[C03] 可变参数
来源：http://pgt.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://rje.shanyushiyangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ugb.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bff.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lzy.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gmn.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xqc.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://utj.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://afs.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://kgg.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sgl.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hlj.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dik.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wck.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://pob.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://dlv.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://uch.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://fts.aizwys.cn

[C05] 返回多个值
来源：http://iyu.dianchejie.cn

Py:   return a, b
来源：http://qbf.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://fzm.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ypl.chenlongwang.top

TS:   return { a, b };
来源：http://qmd.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://viq.daxiang520.top

Go:   return a, b
来源：http://ypp.svipenyu.cn

Ruby: return a, b
来源：http://arz.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://aym.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://mrn.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://swp.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xqd.yvedp.cn

JS:   const square = x => x * x;
来源：http://ubr.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://hya.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gxj.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jwj.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://oap.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://nte.fktsv.cn

[C07] 把函数作为参数传入
来源：http://faw.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uke.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kss.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mgt.fehbvm.com

TS:   arr.map(String)
来源：http://iwc.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mvq.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vdt.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://fra.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://gfy.yongpay.top

[C08] 闭包
来源：http://xjm.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dwo.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jzb.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bnz.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qyr.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://trg.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mip.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zup.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wcq.guannengcc.top

[C09] 递归
来源：http://ukg.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bau.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yvt.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nqu.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ovv.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://omr.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rpl.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ahv.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oxd.fzhhl.top

[C10] 变量作用域
来源：http://cqq.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://snm.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qup.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hyq.vqdsnc.cn

TS:   同 JS
来源：http://wqz.gzhubu.top

Java: 方法内为块级作用域
来源：http://wgd.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://cme.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nwv.havefunace.top

C#:   块级作用域
来源：http://cpm.zdqjudy.top

[C11] 模块导入与导出
来源：http://aae.nanxinkj.top

Py:   from module import func
来源：http://ixw.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://iwq.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mue.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bkt.hongshengwenyu.top

Java: import java.util.List;
来源：http://che.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oqm.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://tld.meibo888.top

C#:   using System.Text;
来源：http://eye.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://nvv.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://wug.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://yao.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://ayl.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://gul.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ggr.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://rbs.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://kbb.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mqr.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://juw.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://knd.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pnl.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zwa.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xje.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://lbq.tarul.cn

Go:   func add(a, b int) int
来源：http://gcp.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fzq.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://hcf.jyoumei.cn

[C14] 泛型函数
来源：http://ccq.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ocd.wangshuangyany.cn

PHP:  // 无泛型
来源：http://mzb.shuidangran.top

JS:   // 无泛型
来源：http://uop.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bcp.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hhl.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ihs.316326.xyz

Ruby: # 无泛型
来源：http://eau.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vwm.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://dzt.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwx.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://mnw.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gsz.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jlj.yongpay.top

Java: // 无解构
来源：http://vxb.quarkkingdee.top

Go:   // 无解构
来源：http://qqy.ctjpmb.com


<!-- 参考信息 -->