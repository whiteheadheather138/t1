代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tqo.redwolf501.top

================================================================================
来源：http://gdt.ywan-chungtsiang.top

B. 流程控制
来源：http://tgk.xylfe.cn

================================================================================
来源：http://kjc.52xcode.cn

[B01] 条件判断 if / else
来源：http://rms.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lpn.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://axl.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rkh.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iho.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vjh.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jft.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qei.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hgi.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://tsu.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://spn.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fin.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mrp.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ety.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asr.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ftv.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lhb.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sbf.wangshuangyany.cn

[B03] switch / match / case
来源：http://ben.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://csb.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vuc.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zon.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mqa.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xyp.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oez.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wqb.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tlm.cucudq.cn

[B04] for 计数循环
来源：http://usw.uphjek.com

Py:   for i in range(10): print(i)
来源：http://yir.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lpe.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zkl.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://htn.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uyr.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pjw.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://ooo.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cdn.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://ugz.jianghu66.top

Py:   for item in arr: print(item)
来源：http://sdb.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dtu.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fri.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://isw.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://erg.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mde.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://pmx.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://utx.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://lai.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dgv.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qkl.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zwo.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ilt.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wel.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fcp.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://orr.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://frc.jinyuanbaomall.cn

[B07] while 循环
来源：http://qiv.xuanzx.com

Py:   while i < 10: i += 1
来源：http://vqe.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://xcl.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://yek.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://mav.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://uxz.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dya.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://nun.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://byg.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://qzf.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://gdu.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://gyw.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://ult.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://mxq.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://qtu.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rwu.fzhhl.top

Ruby: begin; i += 1; end while i < 10
来源：http://cjg.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://fcl.guannengcc.top

[B09] break 与 continue
来源：http://gpv.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lfg.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oht.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ivg.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kkr.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ted.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xfw.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ubv.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlf.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://xfz.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zll.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://csh.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://asl.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xch.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nxg.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xvf.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bgz.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wag.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://jjg.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://fie.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://oik.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rta.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bdn.yfazqb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://njh.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://meq.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://oic.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://emi.tian-w.cn

[B12] 跳出多层循环
来源：http://jkp.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dvx.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ged.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pqx.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tun.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rqa.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ino.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vol.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rop.snrcjt.cn

[B13] 判断是否为数字
来源：http://stv.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://jib.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://far.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qfr.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tbh.nanxuanxn.top

Java: x instanceof Number
来源：http://evs.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nvl.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://pyu.svipenyu.cn

C#:   x is int or double or decimal
来源：http://wfe.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://ikc.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zsw.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tqn.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://dca.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://fav.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rxj.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://srj.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://trj.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eay.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://kki.jinghuilouyu.cn

Py:   a and b or not c
来源：http://uxh.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://dni.meibo888.top

JS:   a && b || !c
来源：http://nhj.cqqwz.cn

TS:   a && b || !c
来源：http://otk.jiagoushi.top

Java: a && b || !c
来源：http://cpt.tanke756.top

Go:   a && b || !c
来源：http://kyu.daxiang520.top

Ruby: a && b || !c
来源：http://hst.jinghuilouyu.cn

C#:   a && b || !c
来源：http://eqg.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://cez.ybcxt.top

Py:   if not data: return
来源：http://tjp.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://ytz.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://cpt.yj202588.top

TS:   if (!data) return;
来源：http://mdy.sysykeji.top

Java: if (data == null) return;
来源：http://ccq.sxryk.cn

Go:   if data == nil { return }
来源：http://ace.svipenyu.cn

Ruby: return if data.nil?
来源：http://drs.fehbvm.com

C#:   if (data == null) return;
来源：http://uyh.hcnkem.com

================================================================================
来源：http://lsa.xylfe.cn

C. 函数与作用域
来源：http://ddj.pycfn.com

================================================================================
来源：http://qmn.ydjk.org.cn

[C01] 定义函数
来源：http://ebs.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://vok.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ogj.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://ghe.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mrk.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vny.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://wmf.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://qpw.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ytz.quarkkingdee.top

[C02] 默认参数
来源：http://oxt.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://had.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aar.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://etd.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yok.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://zyo.hongshengwenyu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hkl.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://ggo.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://dcd.pycfn.com

[C03] 可变参数
来源：http://kzw.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://uzg.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cyf.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gmz.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://udk.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jhn.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://glb.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://nty.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://toe.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://pml.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tdj.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ekz.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tlr.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zgb.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://rdx.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://mfn.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://vct.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://dfl.zdqjudy.top

[C05] 返回多个值
来源：http://sch.smart0.xyz

Py:   return a, b
来源：http://cyn.chenzaomai.com

PHP:  return [$a, $b];
来源：http://wik.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wkm.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://yam.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zlq.hammf.cn

Go:   return a, b
来源：http://wnp.uphjek.com

Ruby: return a, b
来源：http://cxt.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://ngv.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://hge.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://zge.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kav.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://zcu.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://iok.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpa.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://fzo.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://zhu.cucudq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oht.ydzc1.top

[C07] 把函数作为参数传入
来源：http://lrc.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://obz.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://tbi.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uli.hnxiangtu.top

TS:   arr.map(String)
来源：http://jbg.xziqi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://job.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://isq.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://ucg.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tkt.tarul.cn

[C08] 闭包
来源：http://ycb.gogol.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://viq.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ula.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cad.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ayp.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bon.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eno.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hjl.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kfi.shzxlz.cn

[C09] 递归
来源：http://ett.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tgu.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vax.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://urt.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aif.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bci.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lan.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ycg.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://emb.epnwcf.com

[C10] 变量作用域
来源：http://hyb.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cva.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zxc.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fem.jyoumei.cn

TS:   同 JS
来源：http://xku.jinqigufen.top

Java: 方法内为块级作用域
来源：http://zzd.yangfankeji.com

Go:   花括号块级作用域
来源：http://udx.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ncs.dianchejie.cn

C#:   块级作用域
来源：http://pii.pycfn.com

[C11] 模块导入与导出
来源：http://cnf.daxiang520.top

Py:   from module import func
来源：http://erc.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gay.ydjk.org.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vic.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qll.pycfn.com

Java: import java.util.List;
来源：http://npq.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bal.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://xpq.c1oappe.top

C#:   using System.Text;
来源：http://rmn.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://ufc.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://vya.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://eug.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://ylt.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://sio.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kry.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://yzf.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://zhn.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://vuq.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://fzn.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uzw.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixo.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gib.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cuo.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://njf.haohaochexian.top

Go:   func add(a, b int) int
来源：http://mac.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sjz.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://yih.fengsongda.top

[C14] 泛型函数
来源：http://ryi.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://igw.fktsv.cn

PHP:  // 无泛型
来源：http://edi.jianghu66.top

JS:   // 无泛型
来源：http://lla.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lif.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qzg.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://usx.sjlbkw.cn

Ruby: # 无泛型
来源：http://omr.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ipu.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://pnm.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xeq.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://usq.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://exj.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ens.ehwqpu.com

Java: // 无解构
来源：http://igj.hcnkem.com

Go:   // 无解构
来源：http://qgw.xylfe.cn

Ruby: a, b = pair
来源：http://idq.fehbvm.com

C#:   var (a, b) = pair;
来源：http://vuv.shuidangran.top

[C16] 函数 / 方法重载
来源：http://onl.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lpo.jlsjyb.cn

PHP:  // 无重载
来源：http://ici.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qog.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://pez.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bjc.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://sko.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://urt.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xmb.gaohongyu789.top

================================================================================
来源：http://xwt.yj202588.top

D. 数组 / 列表 / 集合
来源：http://ipz.jiagoushi.top

================================================================================
来源：http://kjk.c1oappe.top

[D01] 创建数组 / 列表
来源：http://ddv.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://aee.yonumen.top


<!-- 参考信息 -->