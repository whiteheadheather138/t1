代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://dbc.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://muq.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jxk.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lqx.yj20258888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://veh.cashguo.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hba.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iap.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://znl.jianghu66.top

[A26] 类型转换总览
来源：http://jkc.yj20258888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zyk.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qzg.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ied.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://tjy.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vpz.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bty.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://orz.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rrh.ivvv.top

================================================================================
来源：http://rwh.xuanzx.com

B. 流程控制
来源：http://mci.quarkkingdee.top

================================================================================
来源：http://qgn.hammf.cn

[B01] 条件判断 if / else
来源：http://chj.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://nmp.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ndl.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yld.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qjq.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://yqm.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://unh.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eeo.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://off.xylfe.cn

[B02] 多分支 else if / elif
来源：http://ybw.jinghuilouyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uvz.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://thd.kuanghao11.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbr.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mjh.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aur.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zza.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hvp.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bgq.cdnleiting.top

[B03] switch / match / case
来源：http://pzj.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rrz.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://crv.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://suy.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://udz.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://edp.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://otv.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nxd.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lso.hysaishi.cn

[B04] for 计数循环
来源：http://gry.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://tus.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tcm.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://acf.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ajg.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cwq.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cqm.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://rjh.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xuv.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://png.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://kpb.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://svp.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vyy.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rpu.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gdd.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kbh.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://kjc.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wrp.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://hgy.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wbb.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://icq.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lmd.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mgv.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zcb.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ggu.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iek.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vnn.chenlongwang.top

[B07] while 循环
来源：http://sri.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://sop.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://ara.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://nxl.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://jdv.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://oln.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://acy.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://cwg.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://bko.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://obt.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://krv.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://opd.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://yys.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://qzg.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://qnj.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rza.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://fom.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://fap.vehdjk.com

[B09] break 与 continue
来源：http://vin.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sto.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rlj.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cay.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txp.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zqa.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ciy.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hwb.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxu.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://krw.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lri.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://axg.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dep.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kdz.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://spf.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lfw.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fvy.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ehi.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://tpc.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://ywh.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://cet.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kpe.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://acu.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qlx.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bki.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://eoh.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fbj.sysykeji.top

[B12] 跳出多层循环
来源：http://tox.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dlf.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xsf.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://twb.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ctx.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eau.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ndf.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wun.shuidangran.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://scf.svipenyu.cn

[B13] 判断是否为数字
来源：http://dhz.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://ucx.hfpthk.cn

PHP:  is_numeric($x)
来源：http://lyr.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vjk.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ihj.jianghu66.top

Java: x instanceof Number
来源：http://mrp.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gyv.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://lgo.sufxvd.cn

C#:   x is int or double or decimal
来源：http://qdp.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://dlq.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cgt.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lgg.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://syl.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://htc.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tqd.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://anu.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://sdt.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ljq.jianghu66.top

[B15] 布尔运算与取反
来源：http://vog.xylfe.cn

Py:   a and b or not c
来源：http://fdr.vehdjk.com

PHP:  $a && $b || !$c
来源：http://qmy.ivvv.top

JS:   a && b || !c
来源：http://rgc.cqqwz.cn

TS:   a && b || !c
来源：http://oac.zdbjq.cn

Java: a && b || !c
来源：http://utk.xinyue.icu

Go:   a && b || !c
来源：http://iwz.iojbl.cn

Ruby: a && b || !c
来源：http://zke.hnxiangtu.top

C#:   a && b || !c
来源：http://bpe.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jpy.quarkkingdee.top

Py:   if not data: return
来源：http://zdb.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://qrd.ppjwa.cn

JS:   if (!data) return;
来源：http://ybh.gogol.net.cn

TS:   if (!data) return;
来源：http://znp.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://soa.52xcode.cn

Go:   if data == nil { return }
来源：http://kmv.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://sqv.shuidangran.top

C#:   if (data == null) return;
来源：http://uju.hnxiangtu.top

================================================================================
来源：http://vvx.hnxiangtu.top

C. 函数与作用域
来源：http://uxo.shanyushiyangkeji.top

================================================================================
来源：http://bsg.fzhhl.top

[C01] 定义函数
来源：http://gek.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://bxf.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iiq.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://pdp.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tqj.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tqt.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://ybg.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://efr.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jdw.c1oappe.top

[C02] 默认参数
来源：http://ceb.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://eqo.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://izj.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://izi.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uxh.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://npt.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://voa.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://ikq.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://vyz.meibo888.top

[C03] 可变参数
来源：http://ckh.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://tju.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://che.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tyv.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://geo.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fbg.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gdg.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://mzi.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wrr.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://kae.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://del.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vpo.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zjw.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zkc.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://doz.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://vij.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://guh.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://osi.cheryme.top

[C05] 返回多个值
来源：http://upc.zdbjq.cn

Py:   return a, b
来源：http://yaj.yongpay.top

PHP:  return [$a, $b];
来源：http://bmf.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vov.zhoulong.xyz

TS:   return { a, b };
来源：http://pgy.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jon.xuanzx.com

Go:   return a, b
来源：http://kzp.fktsv.cn

Ruby: return a, b
来源：http://heq.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://fis.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://ote.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://icn.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://opp.tianlin.xyz

JS:   const square = x => x * x;
来源：http://qrr.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://zym.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://odu.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://slb.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://xmq.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sbz.yj20258888.top

[C07] 把函数作为参数传入
来源：http://wsj.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hhp.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://knt.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hdb.tanke756.top

TS:   arr.map(String)
来源：http://isr.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dyp.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ppw.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://yoi.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ebd.birdmap.top

[C08] 闭包
来源：http://mut.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ujl.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ksq.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tap.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kpq.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ibf.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://npl.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jxn.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jkf.aibaodan.cn

[C09] 递归
来源：http://rbv.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jmy.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bpg.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cma.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://glh.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hxo.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qgz.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fbw.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://laz.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://yif.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vmr.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bwf.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wbo.jianghu66.top

TS:   同 JS
来源：http://zvi.yuxming.cn

Java: 方法内为块级作用域
来源：http://pjj.svipenyu.cn

Go:   花括号块级作用域
来源：http://jst.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nai.birdmap.top

C#:   块级作用域
来源：http://vra.yonumen.top

[C11] 模块导入与导出
来源：http://hgx.svipenyu.cn

Py:   from module import func
来源：http://hai.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://osd.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ups.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lqi.cheryme.top

Java: import java.util.List;
来源：http://lai.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yri.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://zxr.yj202588.top

C#:   using System.Text;
来源：http://jbf.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://fqg.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://mzo.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://tgg.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://tmt.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://arc.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ouz.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://flt.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://hrq.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://cjh.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://add.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pob.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkx.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kdz.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wwu.andypj.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://hyu.nanxinkj.top

Go:   func add(a, b int) int
来源：http://gop.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gvx.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xhy.pengpengdd.cyou

[C14] 泛型函数
来源：http://tzb.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ndh.52xcode.cn

PHP:  // 无泛型
来源：http://liu.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://rfi.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uej.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mov.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ceu.cqqwz.cn

Ruby: # 无泛型
来源：http://zvr.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tkc.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://rac.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://acz.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://pwo.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://otm.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yhz.nanxuanxn.top

Java: // 无解构
来源：http://qqb.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://idi.chenzaomai.com


<!-- 参考信息 -->