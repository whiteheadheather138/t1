代发 wailian999

C#:   s.Length
来源：http://chg.ybcxt.top

[A23] 大小写转换
来源：http://zhn.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yyh.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xnk.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pov.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eqi.zycfv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yvd.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vbz.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://usk.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dqm.jiagoushi.top

[A24] 去除首尾空白
来源：http://njy.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iji.xinyue.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ruo.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://won.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ckb.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kri.jiagoushi.top

Go:   strings.TrimSpace(s)
来源：http://vxj.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pvd.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fdx.bjfxy.top

[A25] 字符串比较
来源：http://rkj.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://nsa.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hqh.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qko.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rac.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zzq.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://egf.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://njy.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pzq.hammf.cn

[A26] 类型转换总览
来源：http://elk.daxiang520.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jpk.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://itz.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://utu.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://syw.guannengcc.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kgl.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cny.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rea.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rbz.smart0.xyz

================================================================================
来源：http://gbk.sjlbkw.cn

B. 流程控制
来源：http://mud.zhoulong.xyz

================================================================================
来源：http://gsi.yuanzhike.top

[B01] 条件判断 if / else
来源：http://qky.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sif.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nxt.ybcxt.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lpz.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oyl.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hxm.shuidangran.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aic.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ecx.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fmm.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://xwv.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lko.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zit.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fkg.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zzl.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cng.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zho.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jll.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://soi.yj202588.top

[B03] switch / match / case
来源：http://oaj.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pyw.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://anc.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xsy.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jae.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tgt.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cub.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qyx.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xgn.yangfankeji.com

[B04] for 计数循环
来源：http://qdo.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://tyq.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eqj.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hvl.yongpay.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uzb.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ica.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tpx.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://ryi.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://saj.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://uup.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://ycl.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lxq.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ivk.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://sgb.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wzu.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mne.kuanghao11.cn

Ruby: arr.each { |item| puts item }
来源：http://iuo.tarul.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zny.yj202588.top

[B06] 遍历字典 / 对象
来源：http://obf.zdbjq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eld.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mox.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eoo.cucudq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vab.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://och.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qlz.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://klf.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zji.gzhubu.top

[B07] while 循环
来源：http://rmg.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://zbj.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://gaa.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://jeo.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://uzw.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://xxx.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jmt.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://eoz.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://lcl.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://rzf.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://bhg.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bxj.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://jme.chenjidiqi.icu

TS:   do { i++; } while (i < 10);
来源：http://woe.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://swj.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oqr.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://cms.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://ygy.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://hys.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wxy.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xgy.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qux.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://get.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayu.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rsq.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://umk.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mly.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://tut.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xmc.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rrx.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mst.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bkd.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dnj.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wev.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zhc.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bya.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://ywi.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://cuh.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://ctt.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fui.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zny.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://puj.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ogv.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://ajj.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xfj.smart0.xyz

[B12] 跳出多层循环
来源：http://fpa.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://peu.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://bcp.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jkk.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjj.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lsp.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bvj.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rgw.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rbx.tarul.cn

[B13] 判断是否为数字
来源：http://bcx.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://vbj.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://uxc.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cus.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jii.hfpthk.cn

Java: x instanceof Number
来源：http://jjg.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fll.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://bdm.gotoacloud.top

C#:   x is int or double or decimal
来源：http://pbk.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://prq.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://geg.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gvi.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://mhr.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zxc.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://vsr.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kdr.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://nbs.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nvz.0kj1m.cn

[B15] 布尔运算与取反
来源：http://alc.pengpengdd.cyou

Py:   a and b or not c
来源：http://faa.hcnkem.com

PHP:  $a && $b || !$c
来源：http://qzm.hnxiangtu.top

JS:   a && b || !c
来源：http://gjc.pycfn.com

TS:   a && b || !c
来源：http://cnr.feifeiyinyue.top

Java: a && b || !c
来源：http://una.meibo888.top

Go:   a && b || !c
来源：http://rya.gaohongyu789.top

Ruby: a && b || !c
来源：http://fxt.hnxiangtu.top

C#:   a && b || !c
来源：http://ope.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ypn.quarkkingdee.top

Py:   if not data: return
来源：http://jxc.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://bbw.yvedp.cn

JS:   if (!data) return;
来源：http://lds.cdnleiting.top

TS:   if (!data) return;
来源：http://ule.zycfv.cn

Java: if (data == null) return;
来源：http://irz.c1oappe.top

Go:   if data == nil { return }
来源：http://ppc.kuanghao11.cn

Ruby: return if data.nil?
来源：http://uzq.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://hir.jinqigufen.top

================================================================================
来源：http://cvh.xylfe.cn

C. 函数与作用域
来源：http://fka.jinqigfzy.top

================================================================================
来源：http://spc.ctjpmb.com

[C01] 定义函数
来源：http://mvu.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://djj.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hmg.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://elu.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pot.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://yki.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hel.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://lxa.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qlz.sxryk.cn

[C02] 默认参数
来源：http://sxq.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://wcq.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hqh.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://ajs.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://saj.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ndx.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cay.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://ths.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://rty.jinyuanbaomall.cn

[C03] 可变参数
来源：http://enb.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://cpn.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uoe.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mtk.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqr.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nob.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kej.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://yde.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gro.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://hti.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mhc.tianlin.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://drs.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jmb.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://glw.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://ieh.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://fdi.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://dbb.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://xvn.yangfankeji.com

[C05] 返回多个值
来源：http://oaz.tanke756.top

Py:   return a, b
来源：http://ffy.hywenlv.cn

PHP:  return [$a, $b];
来源：http://ypj.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lqh.ehwqpu.com

TS:   return { a, b };
来源：http://yoh.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dbg.aizwys.cn

Go:   return a, b
来源：http://jam.vehdjk.com

Ruby: return a, b
来源：http://kko.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://dnn.ivvv.top

[C06] 匿名函数 / lambda
来源：http://sqy.yueranfly.top

Py:   square = lambda x: x * x
来源：http://pah.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cqf.guannengcc.top

JS:   const square = x => x * x;
来源：http://uhs.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://enm.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://chz.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://vku.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://ndv.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mls.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://lhe.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://etp.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://chd.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gkd.pengpengdd.cyou

TS:   arr.map(String)
来源：http://lxa.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yar.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zto.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://acl.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xoc.yj20258888.top

[C08] 闭包
来源：http://wbm.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rie.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kju.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bmw.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ozk.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cbq.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cjb.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kmz.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ujp.jinqigfzy.top

[C09] 递归
来源：http://yyi.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kpk.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://prh.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cbx.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lpr.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ypp.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ele.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rmf.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vcl.zhixingplan.top

[C10] 变量作用域
来源：http://csw.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rkd.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cgm.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ude.nanxinkj.top

TS:   同 JS
来源：http://zhn.pycfn.com

Java: 方法内为块级作用域
来源：http://uvw.yueranfly.top

Go:   花括号块级作用域
来源：http://fxf.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://opk.zhengqikj.top

C#:   块级作用域
来源：http://pxe.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://ndt.chenlongwang.top

Py:   from module import func
来源：http://gox.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://gos.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pyq.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tld.xinyue.icu

Java: import java.util.List;
来源：http://ehr.xziqi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mro.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://xcg.xuanzx.com

C#:   using System.Text;
来源：http://pfu.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://etd.birdmap.top

Py:   (lambda: print("run"))()
来源：http://dzp.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://afg.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://rbv.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://vev.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pgo.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://ebe.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://gij.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kmd.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://hkr.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hru.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pia.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jgp.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ick.yuanzhike.top


<!-- 参考信息 -->