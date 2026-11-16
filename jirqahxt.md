代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ssc.zhengqikj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xkj.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://owz.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wkp.dashuyun.cn

Go:   strings.TrimSpace(s)
来源：http://skx.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vhb.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vwu.yuanzhike.top

[A25] 字符串比较
来源：http://tei.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://alp.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://geb.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pxw.nanxinkj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ohy.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dwa.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zoq.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pdn.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bdl.0kj1m.cn

[A26] 类型转换总览
来源：http://qjg.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ufi.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wkr.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sou.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://lrt.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bor.jinyuanbaomall.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ijf.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rrq.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qud.hesvh.cn

================================================================================
来源：http://bgy.zdqjudy.top

B. 流程控制
来源：http://kdt.cdnleiting.top

================================================================================
来源：http://jty.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://xgm.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://vkt.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zpg.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kur.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ojl.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jxw.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nou.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mad.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fat.fzhhl.top

[B02] 多分支 else if / elif
来源：http://nxh.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://txr.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://brq.wangdashe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jkm.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zix.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xrz.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rnc.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://llg.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqd.pengpengdd.cyou

[B03] switch / match / case
来源：http://uei.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ocz.vehdjk.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nsn.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://opz.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fst.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zwn.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://faj.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zoz.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fbh.zdqjudy.top

[B04] for 计数循环
来源：http://axq.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://ztl.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ikp.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dlc.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ces.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mvv.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://doc.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://ojw.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ytz.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://rag.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://lcr.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bug.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://cin.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://niu.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fsh.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xud.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://mlg.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fae.guowangkeji.top

[B06] 遍历字典 / 对象
来源：http://der.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://lgz.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://etd.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vws.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iqu.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://poi.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dbk.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kta.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://axl.yj20258888.top

[B07] while 循环
来源：http://ayk.sweek.top

Py:   while i < 10: i += 1
来源：http://zcv.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://xgz.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://wsv.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://eqx.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://hmh.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bzq.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://kly.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://liv.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://ngg.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://gak.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bvg.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://exs.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://pcf.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://zmn.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://jin.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kxl.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://vui.sufxvd.cn

[B09] break 与 continue
来源：http://hek.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://frw.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fki.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qup.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfc.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nbl.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lol.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uuf.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dcx.sysykeji.top

[B10] 遍历同时拿索引
来源：http://lfz.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://alc.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mns.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sgk.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jvx.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vpm.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uta.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ays.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mkb.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://xfj.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://zrm.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://ehm.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bay.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yqn.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vfw.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://umg.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://ptz.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hjy.aibaodan.cn

[B12] 跳出多层循环
来源：http://ibo.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rvn.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cmk.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ixk.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gkr.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lad.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iru.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yeb.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wbc.cheryme.top

[B13] 判断是否为数字
来源：http://wlh.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://fih.yuxming.cn

PHP:  is_numeric($x)
来源：http://aqm.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gph.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mhu.pengpengdd.cyou

Java: x instanceof Number
来源：http://woq.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://urt.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://inf.52xcode.cn

C#:   x is int or double or decimal
来源：http://pcp.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://tje.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rrw.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xzk.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://wro.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://vkx.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mgj.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xtp.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://wjd.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vet.fengsongda.top

[B15] 布尔运算与取反
来源：http://slo.yueranfly.top

Py:   a and b or not c
来源：http://gbh.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://awr.shuidangran.top

JS:   a && b || !c
来源：http://yki.fengsongda.top

TS:   a && b || !c
来源：http://gxr.zhijiandao.cn

Java: a && b || !c
来源：http://pfy.tian-w.cn

Go:   a && b || !c
来源：http://btp.ydzc1.top

Ruby: a && b || !c
来源：http://htp.daxiang520.top

C#:   a && b || !c
来源：http://dgy.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yjr.sufxvd.cn

Py:   if not data: return
来源：http://dco.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://yoa.shangyingyoupin.top

JS:   if (!data) return;
来源：http://ukv.yj20258888.top

TS:   if (!data) return;
来源：http://uoj.sysykeji.top

Java: if (data == null) return;
来源：http://cvr.yanxiufei.cn

Go:   if data == nil { return }
来源：http://kfu.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://zdk.bjfxy.top

C#:   if (data == null) return;
来源：http://dzu.xinyue.icu

================================================================================
来源：http://ako.havefunace.top

C. 函数与作用域
来源：http://kml.zycfv.cn

================================================================================
来源：http://hbe.zhaomingkeji.xyz

[C01] 定义函数
来源：http://nbz.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://tge.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://chf.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://jzl.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dgd.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://iuj.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://llh.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://ary.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://shy.9152youxi.cn

[C02] 默认参数
来源：http://tkg.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://dld.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dwx.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://olj.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lwb.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wdl.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://knx.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://hvr.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://ooy.wangshuangyany.cn

[C03] 可变参数
来源：http://pqx.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://eoo.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hgx.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ksk.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzi.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bwy.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bev.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://mvu.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tff.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://aof.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zyk.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qub.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mcb.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nvp.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://mbs.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://xyl.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://oqj.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://ztv.9152youxi.cn

[C05] 返回多个值
来源：http://dql.ppjwa.cn

Py:   return a, b
来源：http://xpm.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://nmo.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ise.daxiang520.top

TS:   return { a, b };
来源：http://ros.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yxu.tian-w.cn

Go:   return a, b
来源：http://doc.fktsv.cn

Ruby: return a, b
来源：http://cew.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://nfc.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://cxx.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://lgt.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sdz.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://fvb.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://ymd.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fiv.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://kmc.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://jdc.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://klk.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://tux.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xaf.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://bvv.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ctw.cheryme.top

TS:   arr.map(String)
来源：http://crt.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lxy.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://axq.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://thg.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://hgk.snrcjt.cn

[C08] 闭包
来源：http://fgm.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jrz.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://exq.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qvj.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://der.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iqi.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mkw.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ihp.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yge.cqqwz.cn

[C09] 递归
来源：http://due.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://crw.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cwx.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gml.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zyb.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nxp.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mzt.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kao.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://irl.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://nkb.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mqm.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uty.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dcc.chenlongwang.top

TS:   同 JS
来源：http://rul.nanxinkj.top

Java: 方法内为块级作用域
来源：http://ohc.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://bbp.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xrj.sjlbkw.cn

C#:   块级作用域
来源：http://yhl.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://hvu.fengsongda.top

Py:   from module import func
来源：http://pho.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tca.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hse.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fps.bbcook.cn

Java: import java.util.List;
来源：http://wcz.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://slx.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://yfv.aibaodan.cn

C#:   using System.Text;
来源：http://myn.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://snp.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://sor.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://kue.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://dwf.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://gpv.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nbx.daxiang520.top

Go:   func() { fmt.Println("run") }()
来源：http://cjm.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://rbg.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://kqt.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://ehl.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lsf.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tgc.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://szt.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrl.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://alz.tianlin.xyz

Go:   func add(a, b int) int
来源：http://xog.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqc.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dnx.tarul.cn

[C14] 泛型函数
来源：http://omj.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://etw.pycfn.com

PHP:  // 无泛型
来源：http://egp.wangshuangyany.cn

JS:   // 无泛型
来源：http://xhm.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ndh.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vpa.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ixa.sxryk.cn

Ruby: # 无泛型
来源：http://wlc.bjfxy.top


<!-- 参考信息 -->