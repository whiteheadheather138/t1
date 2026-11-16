代发 wailian999

[B01] 条件判断 if / else
来源：http://hhr.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mjo.gogol.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://glv.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cbp.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://izw.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://jec.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yhu.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hoo.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qdr.meibo888.top

[B02] 多分支 else if / elif
来源：http://jck.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yts.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ftm.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvk.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qef.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khf.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kjr.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cii.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rtn.bjfxy.top

[B03] switch / match / case
来源：http://axq.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pfu.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gks.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dms.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzm.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ljg.bbcook.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://osh.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pst.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nbz.yfazqb.com

[B04] for 计数循环
来源：http://jsn.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://weh.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nhv.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ilq.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fjg.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://osj.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aqk.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://odh.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vig.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://zmf.fehbvm.com

Py:   for item in arr: print(item)
来源：http://gce.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cjx.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://feg.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://adq.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xnw.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vgc.zhongyouzk.top

Ruby: arr.each { |item| puts item }
来源：http://kqs.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yfg.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://qft.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fqa.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xux.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wpb.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bya.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ufc.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ndk.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pqo.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aaq.fanxiaobao.xyz

[B07] while 循环
来源：http://xst.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://rar.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tyu.jqgufenzy.top

JS:   while (i < 10) { i++; }
来源：http://ypg.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://thk.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://osy.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wko.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://nur.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://qsh.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://lbd.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://mkg.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://jrm.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://mku.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://ncg.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://vvt.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gkw.dianchejie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://czd.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://dhg.nanxuanxn.top

[B09] break 与 continue
来源：http://osp.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ign.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jsn.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ncj.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://prx.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mqt.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uag.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rsm.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myw.ydzc1.top

[B10] 遍历同时拿索引
来源：http://kbk.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ujt.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dek.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wkj.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dlg.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://abb.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gqv.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vjt.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://spa.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://rsz.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://xce.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://shs.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rge.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mhl.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xlv.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eno.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://tbj.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ndh.gotoacloud.top

[B12] 跳出多层循环
来源：http://rlj.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gcg.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lqk.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sxc.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vtr.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jcn.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mql.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rlq.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mog.jianghu66.top

[B13] 判断是否为数字
来源：http://bbp.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://ecm.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://fji.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pou.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bwr.zhoulong.xyz

Java: x instanceof Number
来源：http://lpr.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bmf.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://jhi.birdmap.top

C#:   x is int or double or decimal
来源：http://wgn.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://dmr.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://djy.hongshengwenyu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://obh.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://gfh.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://tko.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iga.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bed.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://gwu.hnxiangtu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://krm.meibo888.top

[B15] 布尔运算与取反
来源：http://srj.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://cbk.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://eps.gogol.net.cn

JS:   a && b || !c
来源：http://klj.yuxming.cn

TS:   a && b || !c
来源：http://qyl.hammf.cn

Java: a && b || !c
来源：http://gzp.gogol.net.cn

Go:   a && b || !c
来源：http://emj.hywenlv.cn

Ruby: a && b || !c
来源：http://dji.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://vys.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://klg.xziqi.cn

Py:   if not data: return
来源：http://vln.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://gyf.fzhhl.top

JS:   if (!data) return;
来源：http://zay.cashguo.top

TS:   if (!data) return;
来源：http://tit.hesvh.cn

Java: if (data == null) return;
来源：http://wgn.bbcook.cn

Go:   if data == nil { return }
来源：http://pky.ctjpmb.com

Ruby: return if data.nil?
来源：http://yag.smart0.xyz

C#:   if (data == null) return;
来源：http://zvk.redwolf501.top

================================================================================
来源：http://ulb.ydjk.org.cn

C. 函数与作用域
来源：http://twp.guannengcc.top

================================================================================
来源：http://baw.jinqigufen.top

[C01] 定义函数
来源：http://bhu.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://otn.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzd.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://guv.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vqm.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://fpy.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://dpa.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://irx.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uzq.wangdashe.top

[C02] 默认参数
来源：http://tkh.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://qcc.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://znh.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://qnd.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iwz.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gim.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://skl.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://xfs.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://ayw.hnxiangtu.top

[C03] 可变参数
来源：http://ywb.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://ygh.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tbb.epnwcf.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pyp.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://odp.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uwn.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uws.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://mab.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wfv.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://iqy.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hjc.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bay.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zzx.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rms.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://efc.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://cwi.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://glm.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://der.jinqigfzy.top

[C05] 返回多个值
来源：http://kuc.zhengqikj.top

Py:   return a, b
来源：http://gqj.zdqjudy.top

PHP:  return [$a, $b];
来源：http://wko.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fgb.sjlbkw.cn

TS:   return { a, b };
来源：http://ngf.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://has.sjlbkw.cn

Go:   return a, b
来源：http://dgz.nwbrower.top

Ruby: return a, b
来源：http://rtg.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://yul.yonumen.top

[C06] 匿名函数 / lambda
来源：http://dxf.hammf.cn

Py:   square = lambda x: x * x
来源：http://tnc.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gfj.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://qru.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://rlb.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ism.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://wja.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://nyl.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://qtm.yongpay.top

[C07] 把函数作为参数传入
来源：http://axw.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dme.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://zos.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qbd.gzhubu.top

TS:   arr.map(String)
来源：http://ixz.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://znh.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lqn.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://gtx.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://czw.sufxvd.cn

[C08] 闭包
来源：http://yia.xingfuxueyuan.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tnh.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ykz.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lee.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xwe.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fwq.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zgh.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ljc.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eds.hysaishi.cn

[C09] 递归
来源：http://duu.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ycy.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wbw.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dpb.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tza.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://smw.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yuc.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zpu.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ufe.xuetiantiany.cn

[C10] 变量作用域
来源：http://olu.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://puo.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lqv.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vdk.wangdashe.top

TS:   同 JS
来源：http://yzm.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://iqz.fengsongda.top

Go:   花括号块级作用域
来源：http://ada.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kjq.fengsongda.top

C#:   块级作用域
来源：http://nje.shuidangran.top

[C11] 模块导入与导出
来源：http://bvr.52xcode.cn

Py:   from module import func
来源：http://pbc.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://xpo.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ogm.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xqb.andypj.xyz

Java: import java.util.List;
来源：http://wyw.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sxm.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://jno.jqgfzy.top

C#:   using System.Text;
来源：http://alm.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://trs.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://occ.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://iyi.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://iqn.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://umw.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zjp.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ptd.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://yks.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tfo.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://kal.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://add.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vwo.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nrm.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tlr.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://ihe.zhixingplan.top

Go:   func add(a, b int) int
来源：http://ppc.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ccq.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tbq.jianghu66.top

[C14] 泛型函数
来源：http://haz.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xgg.pengpengdd.cyou

PHP:  // 无泛型
来源：http://qzs.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://emn.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ltf.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fpr.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lfc.zhongyouzk.top

Ruby: # 无泛型
来源：http://mlq.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ner.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://qyl.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rmg.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://cdg.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://veq.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ymm.ydzc1.top

Java: // 无解构
来源：http://msa.epnwcf.com

Go:   // 无解构
来源：http://ecv.quarkkingdee.top

Ruby: a, b = pair
来源：http://njq.hnqzz.top

C#:   var (a, b) = pair;
来源：http://ote.xinyue.icu

[C16] 函数 / 方法重载
来源：http://ahp.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qxf.dianchejie.cn

PHP:  // 无重载
来源：http://emh.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mbl.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://gde.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tqz.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://lbi.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://qcs.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jdb.zycfv.cn

================================================================================
来源：http://vbj.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://yta.guannengcc.top

================================================================================
来源：http://gky.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://pcf.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wtp.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lhd.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://via.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hqy.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uaw.haohaochexian.top


<!-- 参考信息 -->