代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://umx.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xyp.9152youxi.cn

[A24] 去除首尾空白
来源：http://emk.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xmu.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hqg.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://szc.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nfg.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vmp.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://enx.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fud.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ouz.jianghu66.top

[A25] 字符串比较
来源：http://pxs.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://ddo.haohaochexian.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ito.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zte.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://swg.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fep.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yfi.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ffh.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ghm.birdmap.top

[A26] 类型转换总览
来源：http://jcm.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zzz.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cki.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sne.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://vor.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pyw.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sbv.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://brr.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bda.pycfn.com

================================================================================
来源：http://djd.cdnleiting.top

B. 流程控制
来源：http://xye.cucudq.cn

================================================================================
来源：http://xoc.andypj.xyz

[B01] 条件判断 if / else
来源：http://fqe.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xbj.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://whj.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uur.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pht.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sox.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dmu.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dxv.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nwq.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://sdv.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ptr.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lyt.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xrn.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gpl.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fzi.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eet.meibo888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gmx.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgp.gotoacloud.top

[B03] switch / match / case
来源：http://aok.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qmp.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dyj.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mkk.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lua.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nuq.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eqa.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://whm.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yhb.mhx1999.top

[B04] for 计数循环
来源：http://cga.yfazqb.com

Py:   for i in range(10): print(i)
来源：http://nwn.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cvm.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gjt.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xhu.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://umn.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hff.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://oid.jinqigfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jjl.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://sjr.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://goa.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uxk.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bhi.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tli.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://fmn.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jov.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://prk.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bqu.tanke756.top

[B06] 遍历字典 / 对象
来源：http://mwv.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dbp.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qfe.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blp.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agj.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://myc.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kwf.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xuy.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iqh.xinyue.icu

[B07] while 循环
来源：http://niv.cheryme.top

Py:   while i < 10: i += 1
来源：http://ypz.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://rlw.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://jry.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://vie.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://qpz.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kcr.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://ozp.jyoumei.cn

C#:   while (i < 10) { i++; }
来源：http://efc.tanke756.top

[B08] do-while（至少执行一次）
来源：http://lmx.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://wlr.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yvz.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://isp.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://dkw.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://vrr.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jar.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://zle.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://tcx.quarkkingdee.top

[B09] break 与 continue
来源：http://qbr.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zld.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://agz.redwolf501.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypp.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://geb.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcu.ehwqpu.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uef.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aan.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwz.hammf.cn

[B10] 遍历同时拿索引
来源：http://hpq.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dcv.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qol.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sdg.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xmt.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://exc.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kub.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ijz.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jfm.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://qmv.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://vhg.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://kgl.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxk.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://erk.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://axe.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uam.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://uqn.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://feh.mhx1999.top

[B12] 跳出多层循环
来源：http://elj.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bsy.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://foi.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ouy.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xri.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vko.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zoq.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://irc.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ncy.gzhubu.top

[B13] 判断是否为数字
来源：http://kgv.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://lfe.sysykeji.top

PHP:  is_numeric($x)
来源：http://xly.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wgw.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pcp.0kj1m.cn

Java: x instanceof Number
来源：http://jcq.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uxu.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://alb.jiagoushi.top

C#:   x is int or double or decimal
来源：http://njb.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://tnp.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cqf.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gqm.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://ote.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://ibv.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://roh.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wad.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xkb.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tuy.gzhubu.top

[B15] 布尔运算与取反
来源：http://rsj.uphjek.com

Py:   a and b or not c
来源：http://wre.yj20258.top

PHP:  $a && $b || !$c
来源：http://sxk.gaohongyu789.top

JS:   a && b || !c
来源：http://naa.fengsongda.top

TS:   a && b || !c
来源：http://sas.dashuyun.cn

Java: a && b || !c
来源：http://qob.hfpthk.cn

Go:   a && b || !c
来源：http://gds.ydzc1.top

Ruby: a && b || !c
来源：http://pgy.yueranfly.top

C#:   a && b || !c
来源：http://chf.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://hgt.zdbjq.cn

Py:   if not data: return
来源：http://cnu.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://mpo.zdbjq.cn

JS:   if (!data) return;
来源：http://odn.ehwqpu.com

TS:   if (!data) return;
来源：http://zjt.jyoumei.cn

Java: if (data == null) return;
来源：http://rnx.sufxvd.cn

Go:   if data == nil { return }
来源：http://suo.jinqigufen.top

Ruby: return if data.nil?
来源：http://roh.hammf.cn

C#:   if (data == null) return;
来源：http://ebs.sysykeji.top

================================================================================
来源：http://cgt.jqgufenzy.top

C. 函数与作用域
来源：http://wtd.zhengqikj.top

================================================================================
来源：http://mkq.bjfxy.top

[C01] 定义函数
来源：http://sum.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://rsf.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pqt.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://sif.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://htr.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://odk.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ujj.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://jkn.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://stj.shanyushiyangtech.top

[C02] 默认参数
来源：http://bqb.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://blg.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://csj.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://jhx.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bdc.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vsf.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hnq.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://kxj.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://vpd.hysaishi.cn

[C03] 可变参数
来源：http://lvq.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://xpw.ydjk.org.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nja.ybcxt.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lle.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uhh.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ycs.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wgh.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://orm.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://req.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://dxh.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jdl.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rsh.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pte.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tfl.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://bjx.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://cma.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://stt.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://sab.ppjwa.cn

[C05] 返回多个值
来源：http://dxu.nanxuanxn.top

Py:   return a, b
来源：http://htn.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://wii.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qvs.hfpthk.cn

TS:   return { a, b };
来源：http://qte.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pjz.hongshengwenyu.top

Go:   return a, b
来源：http://pqx.yfazqb.com

Ruby: return a, b
来源：http://mne.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://ibf.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://cmf.tian-w.cn

Py:   square = lambda x: x * x
来源：http://kbb.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rhe.cucudq.cn

JS:   const square = x => x * x;
来源：http://srm.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://qps.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cgd.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://hnr.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://trr.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://yxm.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://rkg.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://msr.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pnt.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tzp.dashuyun.cn

TS:   arr.map(String)
来源：http://cxc.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fcv.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kim.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://yuq.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://buj.epnwcf.com

[C08] 闭包
来源：http://rzd.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cwi.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ypw.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://icm.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://let.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hoz.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://scg.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://myn.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gse.shzxlz.cn

[C09] 递归
来源：http://tod.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ldv.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://evw.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bvc.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qxg.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cvz.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ioq.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gas.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nul.zhijiandao.cn

[C10] 变量作用域
来源：http://dnn.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cmk.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://met.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tay.chenlongwang.top

TS:   同 JS
来源：http://ovf.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://rfh.chenzaomai.com

Go:   花括号块级作用域
来源：http://vlx.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qpu.zhengqikj.top

C#:   块级作用域
来源：http://lnf.iojbl.cn

[C11] 模块导入与导出
来源：http://gix.hongshengwenyu.top

Py:   from module import func
来源：http://nyf.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cfn.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xus.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://phd.birdmap.top

Java: import java.util.List;
来源：http://mlz.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bkx.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://igs.ppjwa.cn

C#:   using System.Text;
来源：http://phv.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://awt.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://rfx.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://pgd.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://vsd.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://acj.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://his.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://fxf.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://uyj.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zfk.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://zob.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vev.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sfv.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://khz.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ega.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://awf.gzhubu.top

Go:   func add(a, b int) int
来源：http://hsx.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ujc.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://ajg.zhiwuduotai.top

[C14] 泛型函数
来源：http://bqw.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ldc.yonumen.top

PHP:  // 无泛型
来源：http://lzo.jiagoushi.top

JS:   // 无泛型
来源：http://xgd.chenzaomai.com


<!-- 参考信息 -->