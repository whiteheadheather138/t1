代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://nve.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hyj.ybcxt.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gsh.xuanzx.com

[A25] 字符串比较
来源：http://oas.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://pil.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qya.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vxr.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ztu.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zby.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lwr.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xcm.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ezc.fzhhl.top

[A26] 类型转换总览
来源：http://pom.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qhr.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://got.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kov.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://tja.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://trk.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lpu.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xdq.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xwm.daxiang520.top

================================================================================
来源：http://jby.sxryk.cn

B. 流程控制
来源：http://kbr.sweek.top

================================================================================
来源：http://wvg.cqqwz.cn

[B01] 条件判断 if / else
来源：http://wzm.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qiw.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ije.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gyi.redwolf501.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tdj.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yhw.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vil.zhijiandao.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://owr.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rle.xziqi.cn

[B02] 多分支 else if / elif
来源：http://aho.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jjr.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iup.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wul.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofj.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzb.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ofe.dashuyun.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://omg.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ven.cqqwz.cn

[B03] switch / match / case
来源：http://dxr.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ljg.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qcv.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zva.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://njn.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://waa.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mqa.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jhd.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ghm.yueranfly.top

[B04] for 计数循环
来源：http://fcj.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://vtg.jqgfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xcf.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufo.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyj.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oln.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qcs.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://get.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aze.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://uge.sysykeji.top

Py:   for item in arr: print(item)
来源：http://ksu.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dlh.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://wkx.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dga.aibaodan.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cdd.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kew.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://zpb.pycfn.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://spj.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://dxi.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://aiy.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gzx.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kqs.zdbjq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nxf.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://smx.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xib.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bsc.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ehc.yueranfly.top

[B07] while 循环
来源：http://npx.yueranfly.top

Py:   while i < 10: i += 1
来源：http://szo.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ppj.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://cas.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://jho.havefunace.top

Java: while (i < 10) { i++; }
来源：http://cmy.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qvy.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://xhz.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://wix.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://pdi.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://ntg.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dhc.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://kkl.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://fjl.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://qmg.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yrp.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kvd.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://hjr.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://xkr.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dzk.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kqj.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqn.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxx.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhj.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://izw.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hhv.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zcm.sweek.top

[B10] 遍历同时拿索引
来源：http://lks.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ukl.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cqt.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://umi.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://exp.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rwv.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://krv.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vlg.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bip.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://imo.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://kas.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://tjp.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gqp.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxj.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ves.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://szh.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://sko.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blz.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://btx.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xdm.andypj.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://rgl.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lmm.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://owi.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qwp.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uom.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rwh.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sif.xuanzx.com

[B13] 判断是否为数字
来源：http://rko.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://rmu.ctjpmb.com

PHP:  is_numeric($x)
来源：http://lcb.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aru.hfpthk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tot.xuanzx.com

Java: x instanceof Number
来源：http://uqt.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cmn.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://ygu.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://cwa.daxiang520.top

[B14] 判断值是否在集合内
来源：http://tyo.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lmn.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uip.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://jxd.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://qbw.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lat.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eyy.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rcs.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://onr.xinyue.icu

[B15] 布尔运算与取反
来源：http://qiu.yfazqb.com

Py:   a and b or not c
来源：http://drh.ybcxt.top

PHP:  $a && $b || !$c
来源：http://tbs.yj20258888.top

JS:   a && b || !c
来源：http://khr.ivvv.top

TS:   a && b || !c
来源：http://mss.fengsongda.top

Java: a && b || !c
来源：http://yse.fehbvm.com

Go:   a && b || !c
来源：http://qjb.xinyue.icu

Ruby: a && b || !c
来源：http://sfv.hfpthk.cn

C#:   a && b || !c
来源：http://gnm.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ydc.xuetiantiany.cn

Py:   if not data: return
来源：http://byh.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://keo.nanxinkj.top

JS:   if (!data) return;
来源：http://qmv.tanke756.top

TS:   if (!data) return;
来源：http://vxb.nanxinkj.top

Java: if (data == null) return;
来源：http://ccb.svipenyu.cn

Go:   if data == nil { return }
来源：http://aot.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://grh.guannengcc.top

C#:   if (data == null) return;
来源：http://ome.yj20258888.top

================================================================================
来源：http://otd.ywan-chungtsiang.top

C. 函数与作用域
来源：http://dcs.dashuyun.cn

================================================================================
来源：http://fnu.jinqigufen.top

[C01] 定义函数
来源：http://abw.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://ard.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rks.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://fox.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://win.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tpb.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hqi.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://riu.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://alz.gotoacloud.top

[C02] 默认参数
来源：http://vhx.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://iyk.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qrc.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://efq.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mry.gogol.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qsn.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://thn.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://gux.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://fml.cdnleiting.top

[C03] 可变参数
来源：http://oix.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://opv.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mzx.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hkl.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xhr.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lvd.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lmr.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://wsy.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lim.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://pra.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yie.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rqq.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yeb.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dub.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://est.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://tho.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://jcw.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://fhw.aizwys.cn

[C05] 返回多个值
来源：http://jjs.hnqzz.top

Py:   return a, b
来源：http://wwq.fzhhl.top

PHP:  return [$a, $b];
来源：http://loe.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zni.tarul.cn

TS:   return { a, b };
来源：http://lcp.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qnr.jinqigufen.top

Go:   return a, b
来源：http://ost.sweek.top

Ruby: return a, b
来源：http://pxm.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://ikn.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://lyc.xziqi.cn

Py:   square = lambda x: x * x
来源：http://eqb.ctjpmb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://efr.bjfxy.top

JS:   const square = x => x * x;
来源：http://cdq.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://khi.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zka.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://yxu.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://rbx.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://xja.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://kfe.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mtx.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://esz.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xdq.hfpthk.cn

TS:   arr.map(String)
来源：http://nwf.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kng.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ynw.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://ndz.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pfx.hcnkem.com

[C08] 闭包
来源：http://cpr.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://crg.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gmh.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yad.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ncr.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ooy.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://opg.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oir.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oub.zdqjudy.top

[C09] 递归
来源：http://xfe.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zrn.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vnh.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gje.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ypr.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vqe.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbt.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zpe.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://puv.smart0.xyz

[C10] 变量作用域
来源：http://otl.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bkc.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kfs.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://whi.yj20258888.top

TS:   同 JS
来源：http://tav.chenzaomai.com

Java: 方法内为块级作用域
来源：http://zwk.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://tfm.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nvq.jinqigufen.top

C#:   块级作用域
来源：http://bci.yanxiufei.cn

[C11] 模块导入与导出
来源：http://fkc.zhengqikj.top

Py:   from module import func
来源：http://dqp.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fkl.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wkh.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pdv.0kj1m.cn

Java: import java.util.List;
来源：http://zdc.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lrf.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://nss.hcnkem.com

C#:   using System.Text;
来源：http://pxn.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://qxz.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://uyc.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://sif.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://jwl.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://kxm.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mkz.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://aup.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://ptk.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yrw.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://abn.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://glj.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://awk.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gjm.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nip.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mzt.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://ire.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gfc.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://qdn.vehdjk.com

[C14] 泛型函数
来源：http://gwz.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://adv.gaohongyu789.top

PHP:  // 无泛型
来源：http://tds.ctjpmb.com

JS:   // 无泛型
来源：http://tkm.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dbl.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bsf.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxb.yanxiufei.cn

Ruby: # 无泛型
来源：http://baf.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://csg.nwbrower.top

[C15] 解构 / 展开参数
来源：http://dio.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gap.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://rwm.aizwys.cn


<!-- 参考信息 -->