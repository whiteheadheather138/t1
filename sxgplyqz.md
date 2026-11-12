代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://nhx.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tgr.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oyj.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eog.zdbjq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pun.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jsq.gogol.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ooj.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ntn.jiagoushi.top

[A26] 类型转换总览
来源：http://imi.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uyt.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://arn.yj20258888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fkg.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://sss.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aci.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kem.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jjx.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://idi.tarul.cn

================================================================================
来源：http://xsl.yueranfly.top

B. 流程控制
来源：http://fjr.fzhhl.top

================================================================================
来源：http://che.vehdjk.com

[B01] 条件判断 if / else
来源：http://zby.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dxo.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yoz.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yel.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jzi.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vxu.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zpe.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hrj.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pfu.gzhubu.top

[B02] 多分支 else if / elif
来源：http://pmg.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uaq.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nka.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ooc.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jxw.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eti.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bmo.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lrp.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csy.hcnkem.com

[B03] switch / match / case
来源：http://vkn.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ati.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aaz.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjm.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qgw.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ete.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iej.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mzv.xylfe.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ydg.fzhhl.top

[B04] for 计数循环
来源：http://vaj.yj20258.top

Py:   for i in range(10): print(i)
来源：http://vch.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uia.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oal.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rhh.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fgv.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://twc.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://chn.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cza.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://wbs.316326.xyz

Py:   for item in arr: print(item)
来源：http://fwb.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hrw.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jfv.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kah.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nim.hfpthk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mkt.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://dzd.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ujo.sweek.top

[B06] 遍历字典 / 对象
来源：http://hhv.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zgk.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://say.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cxn.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vsi.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hju.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eiy.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mgb.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pne.mhx1999.top

[B07] while 循环
来源：http://zbl.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://yfr.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rxu.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://ltv.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://jrm.hammf.cn

Java: while (i < 10) { i++; }
来源：http://nqi.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kbp.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://plp.chenjidiqi.icu

C#:   while (i < 10) { i++; }
来源：http://wgy.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://oqb.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://mzh.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nye.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://zfj.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://rqx.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://etf.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rbk.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://dqx.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://dxj.quarkkingdee.top

[B09] break 与 continue
来源：http://mww.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lxl.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fre.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xvd.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mqk.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eyd.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ydo.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gvk.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxj.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://cpl.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ytc.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wzb.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bli.daxiang520.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mzd.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rvg.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qwe.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ycp.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yvq.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://zuo.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://mwm.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://yow.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://frw.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fzw.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aps.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xwz.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://vsy.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gtt.ydzc1.top

[B12] 跳出多层循环
来源：http://olu.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qrp.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://gch.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://izs.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://elh.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zki.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kdl.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yhm.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vzq.yuxming.cn

[B13] 判断是否为数字
来源：http://lkg.zhijiandao.cn

Py:   isinstance(x, (int, float))
来源：http://zhz.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://asa.ivvv.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wah.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lju.haohaochexian.top

Java: x instanceof Number
来源：http://rhy.pengpengdd.cyou

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blb.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://uyq.xylfe.cn

C#:   x is int or double or decimal
来源：http://zsb.smart0.xyz

[B14] 判断值是否在集合内
来源：http://enn.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qpn.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rta.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://lke.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://xwc.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://ghw.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ail.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://pnj.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fya.hammf.cn

[B15] 布尔运算与取反
来源：http://zka.bjfxy.top

Py:   a and b or not c
来源：http://zmh.xziqi.cn

PHP:  $a && $b || !$c
来源：http://sfz.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://gdq.yuxming.cn

TS:   a && b || !c
来源：http://qgl.dianchejie.cn

Java: a && b || !c
来源：http://uin.ehwqpu.com

Go:   a && b || !c
来源：http://ojl.cheryme.top

Ruby: a && b || !c
来源：http://iqq.aizwys.cn

C#:   a && b || !c
来源：http://bly.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dry.hnxiangtu.top

Py:   if not data: return
来源：http://gwh.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://hos.shanyushiyangkeji.top

JS:   if (!data) return;
来源：http://bmz.dashuyun.cn

TS:   if (!data) return;
来源：http://rfb.sysykeji.top

Java: if (data == null) return;
来源：http://jdm.jianghu66.top

Go:   if data == nil { return }
来源：http://ofs.nanxinkj.top

Ruby: return if data.nil?
来源：http://orc.jyoumei.cn

C#:   if (data == null) return;
来源：http://wsy.c1oappe.top

================================================================================
来源：http://llh.hongshengwenyu.top

C. 函数与作用域
来源：http://zhg.chenzaomai.com

================================================================================
来源：http://itp.zycfv.cn

[C01] 定义函数
来源：http://ydz.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://ofo.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbp.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://ibg.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://isz.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rja.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://apa.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://tjv.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bmj.yuxming.cn

[C02] 默认参数
来源：http://xec.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://dak.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gdy.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://dqh.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://usn.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://gag.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sqx.jqgufenzy.top

Ruby: def greet(name = "World") = name
来源：http://xnh.bbcook.cn

C#:   string Greet(string name = "World") => name;
来源：http://nlc.jianghu66.top

[C03] 可变参数
来源：http://ioa.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://psc.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://evy.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rhn.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gtt.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vfu.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wxf.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://czo.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uuw.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://jbv.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vro.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zcm.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xio.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ade.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://pdg.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://hsu.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://ven.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://itk.ctjpmb.com

[C05] 返回多个值
来源：http://gps.zhaomingkeji.xyz

Py:   return a, b
来源：http://vgk.zhengqikj.top

PHP:  return [$a, $b];
来源：http://qql.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://ufs.hnxiangtu.top

TS:   return { a, b };
来源：http://iqk.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ltr.wangshuangyany.cn

Go:   return a, b
来源：http://aok.xinyue.icu

Ruby: return a, b
来源：http://mte.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://ofg.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://qwo.mhx1999.top

Py:   square = lambda x: x * x
来源：http://gro.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://bbu.hfpthk.cn

JS:   const square = x => x * x;
来源：http://ciy.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://ghz.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dum.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://tnn.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://out.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://izs.birdmap.top

[C07] 把函数作为参数传入
来源：http://pvc.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yyg.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ezi.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iuk.zhijiandao.cn

TS:   arr.map(String)
来源：http://xte.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yxs.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lgy.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://mbi.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ref.aizwys.cn

[C08] 闭包
来源：http://gty.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ryn.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zyi.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://acd.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hmx.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lco.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qyi.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lql.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zcz.guannengcc.top

[C09] 递归
来源：http://opm.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://non.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://swh.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sui.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ihh.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zlv.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cxk.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qpe.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ups.sjlbkw.cn

[C10] 变量作用域
来源：http://ivh.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aie.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dcj.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zey.xuetiantiany.cn

TS:   同 JS
来源：http://kjk.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://hax.fehbvm.com

Go:   花括号块级作用域
来源：http://ucf.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hpf.ehwqpu.com

C#:   块级作用域
来源：http://gah.yj20258888.top

[C11] 模块导入与导出
来源：http://xdy.nanxuanxn.top

Py:   from module import func
来源：http://rpo.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wlz.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://aqq.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://adq.xuanzx.com

Java: import java.util.List;
来源：http://hnx.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ihp.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://rcw.vehdjk.com

C#:   using System.Text;
来源：http://del.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://uqk.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://etv.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://joz.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://zwi.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://kiy.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gzv.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://nnw.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://mkv.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://vnm.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://cpx.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uxk.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://drh.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kec.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uod.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://oyo.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://bku.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://adi.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://vbc.nanxinkj.top

[C14] 泛型函数
来源：http://kyk.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ihk.jlsjyb.cn

PHP:  // 无泛型
来源：http://wfl.yfazqb.com

JS:   // 无泛型
来源：http://jos.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yda.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uuo.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ycz.pengpengdd.cyou

Ruby: # 无泛型
来源：http://prq.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rxk.daxiang520.top

[C15] 解构 / 展开参数
来源：http://say.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oyv.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://jfg.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wkf.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://npz.wangshuangyany.cn

Java: // 无解构
来源：http://ava.nanxinkj.top

Go:   // 无解构
来源：http://jvo.zhiwuduotai.top


<!-- 参考信息 -->