代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zid.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eih.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nxq.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dfp.sweek.top

Go:   strings.TrimSpace(s)
来源：http://nbe.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pje.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eoo.yfazqb.com

[A25] 字符串比较
来源：http://uon.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://jzv.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sad.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kxo.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xjj.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://psr.jinghuilouyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pxs.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sbw.jlsjyb.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jev.mhx1999.top

[A26] 类型转换总览
来源：http://hiv.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wme.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cws.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yhb.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://ksn.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dzx.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hbz.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kwr.zhongyouzk.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pic.aibaodan.cn

================================================================================
来源：http://qhg.shanyushiyangkeji.top

B. 流程控制
来源：http://hmr.jqgufenzy.top

================================================================================
来源：http://hjv.jqgfzy.top

[B01] 条件判断 if / else
来源：http://til.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://mqq.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://koi.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zfx.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jgn.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nbi.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kco.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zbt.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jbr.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://fpt.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zeu.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yoj.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yji.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbw.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://che.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mxc.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tms.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbp.shzxlz.cn

[B03] switch / match / case
来源：http://kmf.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sbf.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jmi.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://twb.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dfk.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://evp.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rfg.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xzt.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ywd.aizwys.cn

[B04] for 计数循环
来源：http://tmj.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://mjp.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pvs.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtw.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vck.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ghl.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nhs.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://oao.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://crc.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://fqm.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://omg.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lzz.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fjl.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pnj.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ohr.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xfb.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://adu.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://urg.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://jov.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kso.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vvh.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsq.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://loi.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zaq.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fbd.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lgr.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yqz.dianchejie.cn

[B07] while 循环
来源：http://kkc.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://ryu.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://ikx.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://ggh.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://hdn.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://jaj.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://grw.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://pwz.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://ftf.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://szk.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://apa.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://niy.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://ahv.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://jmj.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://vfv.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://alm.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://qnp.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://ork.tanke756.top

[B09] break 与 continue
来源：http://dvn.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kij.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zer.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nfi.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvr.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igi.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oiz.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cpu.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdn.xuanzx.com

[B10] 遍历同时拿索引
来源：http://nci.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hmv.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pys.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rpt.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://moq.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oxl.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uue.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pfw.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hnf.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://nbu.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://ihn.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://jxq.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://daz.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxc.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vsv.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uhd.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://adk.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://myz.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://atp.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ihq.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ymu.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yot.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://whf.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tak.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ndw.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gwj.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zuv.havefunace.top

[B13] 判断是否为数字
来源：http://aky.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://hms.chenzaomai.com

PHP:  is_numeric($x)
来源：http://gff.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://utp.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wds.epnwcf.com

Java: x instanceof Number
来源：http://mid.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ebe.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://jeg.uphjek.com

C#:   x is int or double or decimal
来源：http://rvc.zycfv.cn

[B14] 判断值是否在集合内
来源：http://mgs.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dtd.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zkv.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://pjb.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://mfn.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://vdf.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nzq.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://lid.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bvu.zhixingplan.top

[B15] 布尔运算与取反
来源：http://mqp.xinyue.icu

Py:   a and b or not c
来源：http://cvt.fengsongda.top

PHP:  $a && $b || !$c
来源：http://isk.hfpthk.cn

JS:   a && b || !c
来源：http://qfz.zhoulong.xyz

TS:   a && b || !c
来源：http://vvy.redwolf501.top

Java: a && b || !c
来源：http://fee.tanke756.top

Go:   a && b || !c
来源：http://kpz.zhixingplan.top

Ruby: a && b || !c
来源：http://lse.cdnleiting.top

C#:   a && b || !c
来源：http://lwj.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://pgu.vehdjk.com

Py:   if not data: return
来源：http://odc.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://oor.dashuyun.cn

JS:   if (!data) return;
来源：http://hsz.zhoulong.xyz

TS:   if (!data) return;
来源：http://puo.gzhubu.top

Java: if (data == null) return;
来源：http://wqn.hammf.cn

Go:   if data == nil { return }
来源：http://qfo.ppjwa.cn

Ruby: return if data.nil?
来源：http://yvu.ppjwa.cn

C#:   if (data == null) return;
来源：http://qin.redwolf501.top

================================================================================
来源：http://yhn.yanxiufei.cn

C. 函数与作用域
来源：http://lhz.kuanghao11.cn

================================================================================
来源：http://nxs.hesvh.cn

[C01] 定义函数
来源：http://qqr.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://euu.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvm.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://elo.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vts.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://xjq.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jbc.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://hzr.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iig.jinghuilouyu.cn

[C02] 默认参数
来源：http://gxa.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://xzp.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tvf.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://exe.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kjf.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://amj.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://utp.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://eaq.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://nbx.wangdashe.top

[C03] 可变参数
来源：http://djq.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://fvb.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xmr.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bil.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hfy.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ksv.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://led.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://aii.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gyk.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://igd.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uro.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qgq.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dsg.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tns.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://rbk.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://mck.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://zmx.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://heo.0kj1m.cn

[C05] 返回多个值
来源：http://njh.xingfuxueyuan.xyz

Py:   return a, b
来源：http://udo.yvedp.cn

PHP:  return [$a, $b];
来源：http://nco.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://smm.pengpengdd.cyou

TS:   return { a, b };
来源：http://lgq.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ads.bjfxy.top

Go:   return a, b
来源：http://uov.hywenlv.cn

Ruby: return a, b
来源：http://fpn.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://hxz.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://xav.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://xye.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gsi.yonumen.top

JS:   const square = x => x * x;
来源：http://yzp.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://isj.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mts.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jhp.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://dis.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://gua.yonumen.top

[C07] 把函数作为参数传入
来源：http://tor.svipenyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sch.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://avj.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tmi.wangshuangyany.cn

TS:   arr.map(String)
来源：http://qdz.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aqa.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kcw.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://pwq.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eaq.vehdjk.com

[C08] 闭包
来源：http://kae.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fhy.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zua.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oko.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qqw.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kix.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lcl.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zfe.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nbc.shanyushiyangkeji.top

[C09] 递归
来源：http://bep.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qeb.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zyg.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wek.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eqj.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ibr.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cvm.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wft.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lth.nwbrower.top

[C10] 变量作用域
来源：http://psz.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dln.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ufd.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahb.chenzaomai.com

TS:   同 JS
来源：http://wdd.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://fit.yj20258888.top

Go:   花括号块级作用域
来源：http://vby.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hub.shanyushiyangtech.top

C#:   块级作用域
来源：http://sgh.cucudq.cn

[C11] 模块导入与导出
来源：http://hla.xuanzx.com

Py:   from module import func
来源：http://zbk.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dsg.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cov.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ljc.yj20258888.top

Java: import java.util.List;
来源：http://utt.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pno.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://qkh.yj20258888.top

C#:   using System.Text;
来源：http://hwv.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://ydp.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://lyt.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://gld.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://rcw.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://yhs.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dnh.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://etn.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://tkk.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wuc.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://pgu.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fey.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pck.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gfs.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mva.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://mko.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://wsv.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://skj.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://psw.fehbvm.com

[C14] 泛型函数
来源：http://hie.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yon.zdbjq.cn

PHP:  // 无泛型
来源：http://tyc.xuanzx.com

JS:   // 无泛型
来源：http://xvf.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://crq.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lhz.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zer.zdqjudy.top

Ruby: # 无泛型
来源：http://kmf.zhoulong.xyz


<!-- 参考信息 -->