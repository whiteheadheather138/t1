代发 wailian999

[B01] 条件判断 if / else
来源：http://efl.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zum.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bvh.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hav.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wjr.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ynw.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ncx.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kbh.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cnx.sysykeji.top

[B02] 多分支 else if / elif
来源：http://ixk.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kqr.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gbh.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jiz.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbh.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kdf.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cvr.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://quq.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehh.hnqzz.top

[B03] switch / match / case
来源：http://bau.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://brp.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gxi.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hok.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nac.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qcp.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vca.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://anr.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kcd.wangshuangyany.cn

[B04] for 计数循环
来源：http://isc.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://vmi.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qcz.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mow.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nmv.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nev.zhixingplan.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eki.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://qyd.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ayx.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://unz.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://ngc.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kdt.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fcm.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ozx.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ais.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tpm.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://muw.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://opx.zhengqikj.top

[B06] 遍历字典 / 对象
来源：http://xrc.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qry.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lng.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jwe.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fqr.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hnp.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ocl.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xcx.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zmc.fzhhl.top

[B07] while 循环
来源：http://kmr.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://loj.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://afy.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://mle.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://gvy.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://jav.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hku.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://lbk.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://agm.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://jhk.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://vte.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://yrg.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://awk.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://tkn.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://lvo.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pht.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://fvo.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://bol.smart0.xyz

[B09] break 与 continue
来源：http://jhl.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cbe.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iqf.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihk.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gik.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ija.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hng.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gwl.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tow.sxryk.cn

[B10] 遍历同时拿索引
来源：http://jwn.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yxu.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wtl.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uzd.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://scv.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zwt.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dvc.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gip.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sos.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://ocf.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://pxr.sweek.top

PHP:  range(0, 10, 2);
来源：http://hpt.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kfw.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tht.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://inq.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aqu.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://zqx.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pxz.bbcook.cn

[B12] 跳出多层循环
来源：http://tcj.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://axv.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fiv.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hay.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mxm.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mzy.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ekq.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqa.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://byp.jyoumei.cn

[B13] 判断是否为数字
来源：http://ujk.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://ilq.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://qva.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://unm.zhoulong.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ace.xuanzx.com

Java: x instanceof Number
来源：http://ext.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gsv.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://olz.smart0.xyz

C#:   x is int or double or decimal
来源：http://eny.tanke756.top

[B14] 判断值是否在集合内
来源：http://kxp.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qrr.yuanzhike.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pcy.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://nmj.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://jiy.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://scc.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kvn.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://sse.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kcl.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://htf.zhongyouzk.top

Py:   a and b or not c
来源：http://jls.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://kxm.tanke756.top

JS:   a && b || !c
来源：http://lyz.yj20258888.top

TS:   a && b || !c
来源：http://lhd.uphjek.com

Java: a && b || !c
来源：http://wzw.mhx1999.top

Go:   a && b || !c
来源：http://cbr.zhoulong.xyz

Ruby: a && b || !c
来源：http://tmy.yonumen.top

C#:   a && b || !c
来源：http://hao.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://flp.epnwcf.com

Py:   if not data: return
来源：http://gml.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://dkq.hongshengwenyu.top

JS:   if (!data) return;
来源：http://mso.xinyue.icu

TS:   if (!data) return;
来源：http://rzi.hongshengwenyu.top

Java: if (data == null) return;
来源：http://rhz.guannengcc.top

Go:   if data == nil { return }
来源：http://tzb.jinqigufen.top

Ruby: return if data.nil?
来源：http://ckj.yuanzhike.top

C#:   if (data == null) return;
来源：http://wmr.snrcjt.cn

================================================================================
来源：http://dyq.mhx1999.top

C. 函数与作用域
来源：http://bij.aizwys.cn

================================================================================
来源：http://cnq.redwolf501.top

[C01] 定义函数
来源：http://iph.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://mnn.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://isy.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://wuk.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jmn.52xcode.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mzr.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qtw.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://pxp.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nme.uphjek.com

[C02] 默认参数
来源：http://dlf.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://fvd.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://css.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://gdq.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://ssy.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ufj.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ngl.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://vlr.bbcook.cn

C#:   string Greet(string name = "World") => name;
来源：http://nyi.kuanghao11.cn

[C03] 可变参数
来源：http://wrf.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://sxg.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://prl.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jst.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tpc.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vfc.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rys.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yjz.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dmp.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://uek.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://niy.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kaq.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hrr.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bdz.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://qep.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://xcs.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://guy.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://hct.ydjk.org.cn

[C05] 返回多个值
来源：http://vgr.dashuyun.cn

Py:   return a, b
来源：http://zod.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://mev.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pty.c1oappe.top

TS:   return { a, b };
来源：http://wfi.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rms.jqgfzy.top

Go:   return a, b
来源：http://inl.cashguo.top

Ruby: return a, b
来源：http://nil.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://ckz.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://wgi.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://toi.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://evq.daria6918.cn

JS:   const square = x => x * x;
来源：http://akt.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://dbx.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fzj.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vmd.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://dkw.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://ggw.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://ugb.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mfc.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://ipx.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ruu.iojbl.cn

TS:   arr.map(String)
来源：http://yik.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ucz.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bvb.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://dif.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vyq.xuanzx.com

[C08] 闭包
来源：http://ybx.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hii.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sdb.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ess.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vfr.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ekl.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://osb.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://syq.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jsr.yj20258.top

[C09] 递归
来源：http://zby.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qgz.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tlt.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://smg.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://imd.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ezl.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bnl.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xso.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://plp.yj20258.top

[C10] 变量作用域
来源：http://hat.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xqe.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dbx.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vsr.yfazqb.com

TS:   同 JS
来源：http://kbj.jiagoushi.top

Java: 方法内为块级作用域
来源：http://pjn.zhijiandao.cn

Go:   花括号块级作用域
来源：http://cac.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lie.jinyuanbaomall.cn

C#:   块级作用域
来源：http://xca.jinqigufen.top

[C11] 模块导入与导出
来源：http://nhh.guowangkeji.top

Py:   from module import func
来源：http://vnc.hfpthk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yqr.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vtp.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hyp.andypj.xyz

Java: import java.util.List;
来源：http://lue.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://icx.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://zjr.bjfxy.top

C#:   using System.Text;
来源：http://ygs.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://fut.hammf.cn

Py:   (lambda: print("run"))()
来源：http://vqu.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://iux.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://zwx.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://rob.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hvq.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://xxl.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://nqt.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mel.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://reb.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xzz.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gpx.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rzm.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wcq.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://hzu.cheryme.top

Go:   func add(a, b int) int
来源：http://ver.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sdp.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mpm.jqgfzy.top

[C14] 泛型函数
来源：http://yra.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bbi.hnqzz.top

PHP:  // 无泛型
来源：http://lsq.zhengqikj.top

JS:   // 无泛型
来源：http://ptk.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qef.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uik.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xll.shuidangran.top

Ruby: # 无泛型
来源：http://kzg.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zpe.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://glw.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uly.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://awg.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jee.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pzi.hysaishi.cn

Java: // 无解构
来源：http://dsv.zhoulong.xyz

Go:   // 无解构
来源：http://npy.sufxvd.cn

Ruby: a, b = pair
来源：http://jll.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://uqp.xinyue.icu

[C16] 函数 / 方法重载
来源：http://pty.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fus.cashguo.top

PHP:  // 无重载
来源：http://edk.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jlr.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://iqi.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ctq.zhaomingkeji.xyz

Go:   // 无重载：用不同函数名
来源：http://dtm.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://ged.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://otx.svipenyu.cn

================================================================================
来源：http://qzc.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://smj.snrcjt.cn

================================================================================
来源：http://oxm.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://rwk.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iwf.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mmf.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ztv.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://doi.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gat.hnqzz.top


<!-- 参考信息 -->