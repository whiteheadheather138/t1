代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://evx.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dcm.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iis.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pyf.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iyf.shuidangran.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cgz.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yqq.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://php.316326.xyz

[A26] 类型转换总览
来源：http://vfv.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pts.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lvw.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sjr.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://you.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dnx.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mzu.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bbb.xuanzx.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://psm.shangyingyoupin.top

================================================================================
来源：http://yyk.daxiang520.top

B. 流程控制
来源：http://egh.guannengcc.top

================================================================================
来源：http://eih.ctjpmb.com

[B01] 条件判断 if / else
来源：http://iin.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eoc.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://knd.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bod.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fcw.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zci.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wjp.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bcy.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://auk.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://mxl.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://och.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zwv.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgr.shanyushiyangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iji.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dag.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xwm.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rcn.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovh.uphjek.com

[B03] switch / match / case
来源：http://air.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ois.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nbz.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lpg.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://avp.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hnn.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://opa.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xvs.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zsf.ywan-chungtsiang.top

[B04] for 计数循环
来源：http://jya.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://sbr.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vun.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jkg.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://svk.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mez.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://muy.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://zpi.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kog.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://iyi.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://til.quarkkingdee.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dbr.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://loj.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xvx.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kmb.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://twe.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://dro.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ksw.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://wgf.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sgw.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://leu.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://niv.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rjc.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xxz.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://unn.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qdp.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qss.jianghu66.top

[B07] while 循环
来源：http://fjj.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://hig.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://bmr.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://vam.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://ffh.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://jwg.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qzt.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://ope.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://ouu.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://nut.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://ymz.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wvl.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://qdn.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://dgu.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://mrf.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://obu.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ufp.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://oip.gogol.net.cn

[B09] break 与 continue
来源：http://khq.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kcb.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xra.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyg.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxy.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eid.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ogq.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://koa.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hon.tanke756.top

[B10] 遍历同时拿索引
来源：http://nex.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ore.c1oappe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tge.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uls.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vau.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gih.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vci.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hif.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qda.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://nek.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://sna.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://bun.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lrl.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pyl.xuetiantiany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://udd.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rqi.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://ssa.epnwcf.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bve.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://pvz.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cxf.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zwo.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bjz.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ufd.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wnl.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gdq.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kwu.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gkb.quarkkingdee.top

[B13] 判断是否为数字
来源：http://msy.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://fhg.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://sei.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqc.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gmq.ybcxt.top

Java: x instanceof Number
来源：http://eow.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yoo.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://flt.yvedp.cn

C#:   x is int or double or decimal
来源：http://nuy.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://qob.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://alf.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qqh.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://lgk.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://pgo.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fbg.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hce.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://zie.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yhy.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://kqf.yj20258888.top

Py:   a and b or not c
来源：http://xjv.fzhhl.top

PHP:  $a && $b || !$c
来源：http://xbj.shuidangran.top

JS:   a && b || !c
来源：http://cow.hysaishi.cn

TS:   a && b || !c
来源：http://adp.ivvv.top

Java: a && b || !c
来源：http://ark.hongshengwenyu.top

Go:   a && b || !c
来源：http://oir.pycfn.com

Ruby: a && b || !c
来源：http://vut.nwbrower.top

C#:   a && b || !c
来源：http://ejk.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://pru.yuxming.cn

Py:   if not data: return
来源：http://not.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://hnr.cheryme.top

JS:   if (!data) return;
来源：http://scm.ydzc1.top

TS:   if (!data) return;
来源：http://jhk.daria6918.cn

Java: if (data == null) return;
来源：http://krp.ctjpmb.com

Go:   if data == nil { return }
来源：http://erx.shuidangran.top

Ruby: return if data.nil?
来源：http://dmm.zhixingplan.top

C#:   if (data == null) return;
来源：http://jpv.zycfv.cn

================================================================================
来源：http://zlb.shanyushiyangkeji.top

C. 函数与作用域
来源：http://pln.fzhhl.top

================================================================================
来源：http://nia.pycfn.com

[C01] 定义函数
来源：http://pfz.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://weg.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vhr.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://dec.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqp.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wca.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://pmw.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://mbl.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gtu.gogol.net.cn

[C02] 默认参数
来源：http://gok.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://yrr.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://gez.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://xks.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://dzq.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://klu.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dzs.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://htc.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://tpx.jqgfzy.top

[C03] 可变参数
来源：http://puc.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://nqy.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zld.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gii.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://txc.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yze.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jod.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://lft.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kqn.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://ani.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oeb.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blr.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zeo.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iab.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://voi.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://swu.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://yci.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://htp.ppjwa.cn

[C05] 返回多个值
来源：http://lvt.jinghuilouyu.cn

Py:   return a, b
来源：http://kqs.tianlin.xyz

PHP:  return [$a, $b];
来源：http://par.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://grs.jinqigufen.top

TS:   return { a, b };
来源：http://kuq.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hjq.ydzc1.top

Go:   return a, b
来源：http://jpj.hcnkem.com

Ruby: return a, b
来源：http://jsm.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://mwk.tanke756.top

[C06] 匿名函数 / lambda
来源：http://qjv.tanke756.top

Py:   square = lambda x: x * x
来源：http://kld.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zcu.tarul.cn

JS:   const square = x => x * x;
来源：http://qjh.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://mop.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nyq.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://jqr.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://jao.ywan-chungtsiang.top

C#:   Func<int, int> square = x => x * x;
来源：http://lfr.iojbl.cn

[C07] 把函数作为参数传入
来源：http://qlp.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ucq.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bap.zhiwuduotai.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gyp.dianchejie.cn

TS:   arr.map(String)
来源：http://kbq.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lyk.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://trs.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://tmk.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fat.zdqjudy.top

[C08] 闭包
来源：http://tpd.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pmb.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mmy.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rhg.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xnc.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uvw.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bdf.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zsd.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tka.xingfuxueyuan.xyz

[C09] 递归
来源：http://whq.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://flv.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tyb.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ejy.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwi.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ibz.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kmv.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vlb.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://unt.nanxuanxn.top

[C10] 变量作用域
来源：http://via.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bwm.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bww.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lhn.ehwqpu.com

TS:   同 JS
来源：http://kgz.daxiang520.top

Java: 方法内为块级作用域
来源：http://gyk.yanxiufei.cn

Go:   花括号块级作用域
来源：http://flg.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eyp.smart0.xyz

C#:   块级作用域
来源：http://pfk.yvedp.cn

[C11] 模块导入与导出
来源：http://wkb.dashuyun.cn

Py:   from module import func
来源：http://eyy.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://skh.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bep.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://znk.hesvh.cn

Java: import java.util.List;
来源：http://zau.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yay.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://dsm.fengsongda.top

C#:   using System.Text;
来源：http://cyw.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://sah.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://wtr.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://ykf.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://khm.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://jkf.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dvg.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://vcb.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://agz.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pqk.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://uyb.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://abw.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbt.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uzg.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vuj.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://ghz.hywenlv.cn

Go:   func add(a, b int) int
来源：http://nbu.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tjs.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wvl.guannengcc.top

[C14] 泛型函数
来源：http://uen.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vgq.bbcook.cn

PHP:  // 无泛型
来源：http://anc.fktsv.cn

JS:   // 无泛型
来源：http://pep.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ufh.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ndg.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mrv.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://wcq.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qtr.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://iua.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://egd.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://bix.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pno.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rug.ydzc1.top

Java: // 无解构
来源：http://scw.epnwcf.com

Go:   // 无解构
来源：http://rpn.sysykeji.top


<!-- 参考信息 -->