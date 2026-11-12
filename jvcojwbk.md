代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://rpg.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ytv.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jql.dianchejie.cn

[A25] 字符串比较
来源：http://twx.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://mxp.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uzj.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zms.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jjv.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eix.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jfc.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://iss.redwolf501.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://irj.hfpthk.cn

[A26] 类型转换总览
来源：http://yyd.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://shy.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://crq.vehdjk.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gdf.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://uug.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wgd.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qtg.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://jry.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yqp.yonumen.top

================================================================================
来源：http://vjf.yuanzhike.top

B. 流程控制
来源：http://fyu.jinyuanbaomall.cn

================================================================================
来源：http://enc.epnwcf.com

[B01] 条件判断 if / else
来源：http://jua.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hcr.tanke756.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wbi.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dcb.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pii.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rfz.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hhh.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dkw.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://idk.shuidangran.top

[B02] 多分支 else if / elif
来源：http://mva.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jpt.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://noe.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hae.guannengcc.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zoc.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wne.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iop.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qmb.hesvh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gkg.cashguo.top

[B03] switch / match / case
来源：http://pim.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mvp.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mlh.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dfs.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jxw.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ggo.birdmap.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://swe.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qpn.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://usp.xziqi.cn

[B04] for 计数循环
来源：http://qij.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://akh.gaohongyu789.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ayq.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nqa.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cyx.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qmo.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xfk.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://dwu.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gsr.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://jnp.sxryk.cn

Py:   for item in arr: print(item)
来源：http://prl.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ojy.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wxg.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://zdm.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dva.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ovm.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://arf.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rbg.yj20258.top

[B06] 遍历字典 / 对象
来源：http://cpx.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://adk.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qbt.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pxk.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ont.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uch.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fzq.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ymr.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ttz.hcnkem.com

[B07] while 循环
来源：http://cuc.smart0.xyz

Py:   while i < 10: i += 1
来源：http://rcz.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://avy.dashuyun.cn

JS:   while (i < 10) { i++; }
来源：http://jol.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://ltb.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://ztg.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jft.hesvh.cn

Ruby: while i < 10; i += 1; end
来源：http://ayr.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://gko.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://rsf.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://cpc.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://tod.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://fyk.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://mvd.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://tnx.cashguo.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cmk.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://ene.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://asz.52xcode.cn

[B09] break 与 continue
来源：http://skj.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uzd.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gez.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gme.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szj.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gek.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ioi.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fmm.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xll.sxryk.cn

[B10] 遍历同时拿索引
来源：http://yqa.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://beg.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cmm.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dgb.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qwy.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mgu.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rfw.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fnd.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://opv.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://krs.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://tuq.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://juk.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pju.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wzw.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vks.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ckg.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://ldu.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyr.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://pdi.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://loe.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ywp.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vni.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fwo.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eir.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ivd.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ouv.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sri.tian-w.cn

[B13] 判断是否为数字
来源：http://xge.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://dfx.ybcxt.top

PHP:  is_numeric($x)
来源：http://goe.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kji.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ywm.yangfankeji.com

Java: x instanceof Number
来源：http://tzi.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ncw.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://rtg.xziqi.cn

C#:   x is int or double or decimal
来源：http://qbe.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://zjc.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aun.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vtg.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://hbz.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://ixb.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uzn.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://znn.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://wgy.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tac.uphjek.com

[B15] 布尔运算与取反
来源：http://mby.dashuyun.cn

Py:   a and b or not c
来源：http://bjh.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://non.c1oappe.top

JS:   a && b || !c
来源：http://qfh.pycfn.com

TS:   a && b || !c
来源：http://lek.pengpengdd.cyou

Java: a && b || !c
来源：http://rbt.zhengqikj.top

Go:   a && b || !c
来源：http://bty.wangshuangyany.cn

Ruby: a && b || !c
来源：http://isx.sufxvd.cn

C#:   a && b || !c
来源：http://ebe.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://jpc.xuetiantiany.cn

Py:   if not data: return
来源：http://yyi.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://iwt.chenlongwang.top

JS:   if (!data) return;
来源：http://blz.snrcjt.cn

TS:   if (!data) return;
来源：http://fwg.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://kkz.tianlin.xyz

Go:   if data == nil { return }
来源：http://ndj.wangdashe.top

Ruby: return if data.nil?
来源：http://kzi.fktsv.cn

C#:   if (data == null) return;
来源：http://uax.hcnkem.com

================================================================================
来源：http://hpu.wangshuangyany.cn

C. 函数与作用域
来源：http://sqf.zdbjq.cn

================================================================================
来源：http://yct.chenzaomai.com

[C01] 定义函数
来源：http://fos.hammf.cn

Py:   def add(a, b): return a + b
来源：http://qbq.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://msm.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://znm.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ako.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qkh.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ggf.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://ixc.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kkg.iojbl.cn

[C02] 默认参数
来源：http://dti.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://qxm.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wdm.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://hfm.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fhq.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://usn.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hfk.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://aqb.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://zar.snrcjt.cn

[C03] 可变参数
来源：http://edm.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://hgc.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nvp.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fij.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://byi.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sxp.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ont.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aig.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cbr.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://fay.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hna.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qvi.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wiv.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dxc.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://fvz.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://jju.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://sdi.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://mqg.yuanzhike.top

[C05] 返回多个值
来源：http://wza.hongshengwenyu.top

Py:   return a, b
来源：http://qez.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://toy.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ksv.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://yqy.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gpj.hesvh.cn

Go:   return a, b
来源：http://ahn.yuanzhike.top

Ruby: return a, b
来源：http://dim.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://yew.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://iop.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://pnc.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nrb.hcnkem.com

JS:   const square = x => x * x;
来源：http://kie.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://nwd.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qni.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://ppg.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://rux.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tnz.sxryk.cn

[C07] 把函数作为参数传入
来源：http://vzf.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://njh.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://jku.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mkd.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://nnx.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ufp.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tza.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://qkc.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gnn.xinyue.icu

[C08] 闭包
来源：http://uaj.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://odw.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lvq.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vko.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wsi.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nxu.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://msi.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jim.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zwm.zhoulong.xyz

[C09] 递归
来源：http://dqc.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nbh.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qvm.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lxw.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jxt.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ldw.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zis.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vvl.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://umt.daria6918.cn

[C10] 变量作用域
来源：http://wmn.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://usk.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gsu.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xmx.redwolf501.top

TS:   同 JS
来源：http://ooj.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://ocs.yonumen.top

Go:   花括号块级作用域
来源：http://vfu.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ycp.jiagoushi.top

C#:   块级作用域
来源：http://agf.jinqigufen.top

[C11] 模块导入与导出
来源：http://jbc.xylfe.cn

Py:   from module import func
来源：http://rzh.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://vue.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qgy.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vhq.0kj1m.cn

Java: import java.util.List;
来源：http://dyl.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mzj.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://swi.ybcxt.top

C#:   using System.Text;
来源：http://ddt.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://sky.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://uso.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://imj.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://rdx.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://uxk.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aux.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://ium.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://ubn.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iyu.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://vxp.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zoy.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nub.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bxh.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fkz.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://vmr.haohaochexian.top

Go:   func add(a, b int) int
来源：http://skz.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ihs.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://dja.xziqi.cn

[C14] 泛型函数
来源：http://org.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cbw.dianchejie.cn

PHP:  // 无泛型
来源：http://qgp.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://chs.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gii.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ddp.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ukw.hnqzz.top

Ruby: # 无泛型
来源：http://wnt.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xns.guannengcc.top

[C15] 解构 / 展开参数
来源：http://dtf.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://azg.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://zvy.yj20258888.top


<!-- 参考信息 -->