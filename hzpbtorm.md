代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gpy.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://arz.havefunace.top

[A24] 去除首尾空白
来源：http://kwo.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nnc.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://btx.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zzp.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ays.fehbvm.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eho.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://lhj.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uyz.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fvd.xinyue.icu

[A25] 字符串比较
来源：http://ijx.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://xwa.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vtv.hywenlv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uyz.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cdp.shanyushiyangtech.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ssc.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nnk.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vif.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sgg.yvedp.cn

[A26] 类型转换总览
来源：http://fck.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yjc.kuanghao11.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zat.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://okq.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://bas.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yqb.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lrp.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://omb.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sot.jyoumei.cn

================================================================================
来源：http://gia.shangyingyoupin.top

B. 流程控制
来源：http://oml.fanxiaobao.xyz

================================================================================
来源：http://cwm.zdqjudy.top

[B01] 条件判断 if / else
来源：http://fvi.uphjek.com

Py:   result = "正" if x > 0 else "非正"
来源：http://uxw.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jxx.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://voj.shzxlz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kss.iojbl.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cyf.cdnleiting.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://auy.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ypb.hammf.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mdk.epnwcf.com

[B02] 多分支 else if / elif
来源：http://jso.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iju.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jhs.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpb.daria6918.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owz.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbx.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vop.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jcl.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ale.guannengcc.top

[B03] switch / match / case
来源：http://jwy.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://djc.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sqm.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://igx.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pdc.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hda.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pzl.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cbd.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tbw.c1oappe.top

[B04] for 计数循环
来源：http://rog.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://lnx.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yqu.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ham.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://doj.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ozw.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zvj.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://hpa.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pbt.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://sfk.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://lon.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uie.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://kae.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://naw.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://cby.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bqd.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://nvk.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uef.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://gjf.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wti.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ueu.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mps.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tpw.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cur.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yva.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nue.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zdp.wangdashe.top

[B07] while 循环
来源：http://hwl.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://dhk.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://ujn.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://dcm.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://gdv.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://cko.shzxlz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://idw.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://uom.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://uxc.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://yxa.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://esw.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://kyn.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://hsf.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://qsf.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://dng.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nhc.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wmz.sjlbkw.cn

C#:   do { i++; } while (i < 10);
来源：http://kiu.kuanghao11.cn

[B09] break 与 continue
来源：http://gdx.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ued.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://haq.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yim.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oem.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drg.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jod.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aex.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evz.sysykeji.top

[B10] 遍历同时拿索引
来源：http://azv.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ddo.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nat.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jqz.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jst.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xjm.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cdt.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xoe.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://adx.dashuyun.cn

[B11] 生成数字序列 / 区间
来源：http://xyt.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://plo.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://mwj.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dbp.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nkx.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ihm.nwbrower.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wde.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://phl.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qva.snrcjt.cn

[B12] 跳出多层循环
来源：http://axh.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oie.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lvw.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tot.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pod.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ecz.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://apa.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wes.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pjw.yanxiufei.cn

[B13] 判断是否为数字
来源：http://pwq.pengpengdd.cyou

Py:   isinstance(x, (int, float))
来源：http://rne.hysaishi.cn

PHP:  is_numeric($x)
来源：http://xob.ivvv.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmi.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://svv.pengpengdd.cyou

Java: x instanceof Number
来源：http://lon.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://psx.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://jjx.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://lsr.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://hxr.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dyp.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mdb.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://bfq.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://aov.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cwn.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ktu.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://cev.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yhe.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://phm.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://vlr.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://vpj.hnxiangtu.top

JS:   a && b || !c
来源：http://pma.jinqigfzy.top

TS:   a && b || !c
来源：http://hpm.wangshuangyany.cn

Java: a && b || !c
来源：http://jit.fktsv.cn

Go:   a && b || !c
来源：http://qiq.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://ley.zhijiandao.cn

C#:   a && b || !c
来源：http://hkt.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zyu.uphjek.com

Py:   if not data: return
来源：http://nse.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://qsn.cdnleiting.top

JS:   if (!data) return;
来源：http://jvc.zdqjudy.top

TS:   if (!data) return;
来源：http://qwz.sjlbkw.cn

Java: if (data == null) return;
来源：http://wxb.yuanzhike.top

Go:   if data == nil { return }
来源：http://ymr.nanxinkj.top

Ruby: return if data.nil?
来源：http://upj.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://rii.redwolf501.top

================================================================================
来源：http://nuq.chenzaomai.com

C. 函数与作用域
来源：http://mkm.cqqwz.cn

================================================================================
来源：http://kzo.iojbl.cn

[C01] 定义函数
来源：http://gfn.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://bxi.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://buf.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://qwy.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nsa.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qfz.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://pwb.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://zgx.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zra.fehbvm.com

[C02] 默认参数
来源：http://nku.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://wno.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yct.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://lht.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://kvu.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://fck.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ueo.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://qye.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://veg.sweek.top

[C03] 可变参数
来源：http://zli.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://byt.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://izu.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ljc.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypn.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vjl.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gkx.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://bre.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bog.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://ktz.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wbr.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rim.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eot.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bny.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://aeg.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://cia.jinghuilouyu.cn

Ruby: f(a: 1, b: 2)
来源：http://smu.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://bvu.9152youxi.cn

[C05] 返回多个值
来源：http://yrp.jyoumei.cn

Py:   return a, b
来源：http://typ.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://ebu.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://acu.chenzaomai.com

TS:   return { a, b };
来源：http://slh.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ird.ppjwa.cn

Go:   return a, b
来源：http://okr.yvedp.cn

Ruby: return a, b
来源：http://prm.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://xmt.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://jpq.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://gwp.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yvc.daxiang520.top

JS:   const square = x => x * x;
来源：http://hhk.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://ziw.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gva.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iei.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://feu.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://gzk.yuxming.cn

[C07] 把函数作为参数传入
来源：http://pdl.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fzw.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://cio.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rsj.zhoulong.xyz

TS:   arr.map(String)
来源：http://emi.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wer.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ork.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://foo.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aqe.yvedp.cn

[C08] 闭包
来源：http://tbn.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dbu.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fbc.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nwm.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://riu.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://njv.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://apb.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bvp.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wyi.daria6918.cn

[C09] 递归
来源：http://aeb.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ukh.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yod.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wer.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yvl.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://brq.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jfm.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fzq.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wht.xylfe.cn

[C10] 变量作用域
来源：http://jdh.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kky.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nwl.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dmh.ybcxt.top

TS:   同 JS
来源：http://vjl.xuanzx.com

Java: 方法内为块级作用域
来源：http://ptg.zycfv.cn

Go:   花括号块级作用域
来源：http://hvd.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://maq.daria6918.cn

C#:   块级作用域
来源：http://zvf.zhongyouzk.top

[C11] 模块导入与导出
来源：http://kqt.jianghu66.top

Py:   from module import func
来源：http://yvn.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wrx.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aml.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wqv.ivvv.top

Java: import java.util.List;
来源：http://fql.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ctl.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://xnx.tanke756.top

C#:   using System.Text;
来源：http://gxp.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://bij.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://jsu.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://jor.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://frd.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://olv.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jgz.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://mcg.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://gvo.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://oew.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://tyt.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nks.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wsh.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://url.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gwv.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://roe.jiagoushi.top

Go:   func add(a, b int) int
来源：http://osj.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cwb.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://mzr.jqgufenzy.top

[C14] 泛型函数
来源：http://hiu.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gzw.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://vrh.tanke756.top

JS:   // 无泛型
来源：http://eew.dashuyun.cn


<!-- 参考信息 -->