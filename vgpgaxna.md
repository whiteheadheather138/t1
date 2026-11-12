代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qrm.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lbg.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qeq.52xcode.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pgg.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eyf.fzhhl.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vwu.shzxlz.cn

[A24] 去除首尾空白
来源：http://viv.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ovt.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cox.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mrm.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kzb.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rii.yongpay.top

Go:   strings.TrimSpace(s)
来源：http://mhz.yuxming.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cfz.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aka.pengpengdd.cyou

[A25] 字符串比较
来源：http://hlk.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://wyy.sjlbkw.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jur.chenjidiqi.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://syx.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://onp.yvedp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pji.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pay.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://csb.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://svb.aizwys.cn

[A26] 类型转换总览
来源：http://sdj.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pbt.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://alr.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bvm.316326.xyz

TS:   Number() String() Boolean() x as number
来源：http://icy.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ffw.dashuyun.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lyi.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bqe.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hap.dianchejie.cn

================================================================================
来源：http://umh.aizwys.cn

B. 流程控制
来源：http://wtt.zhixingplan.top

================================================================================
来源：http://qyb.jqgfzy.top

[B01] 条件判断 if / else
来源：http://gls.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lpp.9152youxi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pdn.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://amf.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://akr.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tdu.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://muz.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vxf.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rtv.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://ria.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://anc.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zya.smart0.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eoe.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgf.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukd.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://the.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kej.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iuh.pycfn.com

[B03] switch / match / case
来源：http://tho.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kjk.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pei.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lwy.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rgs.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ugy.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gjo.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wcs.zdqjudy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zfb.cdnleiting.top

[B04] for 计数循环
来源：http://fvp.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://fqx.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nev.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qvz.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cij.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bea.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ggm.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://oip.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xrt.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://zmb.aizwys.cn

Py:   for item in arr: print(item)
来源：http://ugd.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xwo.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xjd.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fgm.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kmw.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zme.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://rvy.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hvn.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://ffc.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cno.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ckl.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://guw.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://htc.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://agc.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mfi.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jzs.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hbu.fanxiaobao.xyz

[B07] while 循环
来源：http://usm.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://jvr.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://ihm.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://mxq.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://rps.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://kcc.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xyu.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://ixr.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://fim.sweek.top

[B08] do-while（至少执行一次）
来源：http://fxv.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://kjk.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://dge.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://xlz.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://rkh.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://hbo.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://din.fzhhl.top

Ruby: begin; i += 1; end while i < 10
来源：http://tcn.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://vsf.pycfn.com

[B09] break 与 continue
来源：http://uge.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ujd.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ltu.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tti.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vmm.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgv.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vrq.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vfs.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nfx.cucudq.cn

[B10] 遍历同时拿索引
来源：http://vdn.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ndm.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rou.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://euh.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ajz.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xvy.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ind.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uwj.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://unb.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://gfp.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://sot.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://yak.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjg.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ahx.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jnz.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jex.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://vxj.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dmg.xziqi.cn

[B12] 跳出多层循环
来源：http://sxh.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ucz.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tcf.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://art.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jkm.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sas.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gyu.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://spa.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wkt.hesvh.cn

[B13] 判断是否为数字
来源：http://zda.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://pcd.zhengqikj.top

PHP:  is_numeric($x)
来源：http://tqs.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nul.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hro.wangdashe.top

Java: x instanceof Number
来源：http://rcm.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://clq.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://vep.52xcode.cn

C#:   x is int or double or decimal
来源：http://zzf.yj20258.top

[B14] 判断值是否在集合内
来源：http://ayt.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gav.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nuq.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://vzq.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://tod.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dhg.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tcg.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://eum.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://whk.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://zqd.aibaodan.cn

Py:   a and b or not c
来源：http://zrz.sxryk.cn

PHP:  $a && $b || !$c
来源：http://vnn.tian-w.cn

JS:   a && b || !c
来源：http://god.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://moa.jinqigufen.top

Java: a && b || !c
来源：http://vqc.fzhhl.top

Go:   a && b || !c
来源：http://ikc.fehbvm.com

Ruby: a && b || !c
来源：http://cdq.jinqigfzy.top

C#:   a && b || !c
来源：http://lzo.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oqe.vqdsnc.cn

Py:   if not data: return
来源：http://phj.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://zww.yonumen.top

JS:   if (!data) return;
来源：http://saw.tianlin.xyz

TS:   if (!data) return;
来源：http://cya.sufxvd.cn

Java: if (data == null) return;
来源：http://scy.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://lex.cqqwz.cn

Ruby: return if data.nil?
来源：http://tpm.yfazqb.com

C#:   if (data == null) return;
来源：http://vpl.jyoumei.cn

================================================================================
来源：http://awr.chenlongwang.top

C. 函数与作用域
来源：http://ggs.ctjpmb.com

================================================================================
来源：http://avc.jlsjyb.cn

[C01] 定义函数
来源：http://gru.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://tzy.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ihi.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://rtu.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ifo.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zms.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://ebu.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://dbi.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aea.yanxiufei.cn

[C02] 默认参数
来源：http://qah.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://uvb.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://foh.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://flo.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ivx.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://dnh.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xnn.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://feb.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://wsp.jqgufenzy.top

[C03] 可变参数
来源：http://jzb.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://soe.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bxe.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zgu.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kuv.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iep.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://anz.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://rgh.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://avh.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://pdd.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://npe.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://udm.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wxr.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yhg.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://aqs.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://hbo.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://rxd.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://hpc.bjfxy.top

[C05] 返回多个值
来源：http://igw.zdqjudy.top

Py:   return a, b
来源：http://ncv.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://fzn.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dhu.sysykeji.top

TS:   return { a, b };
来源：http://swn.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://adz.haohaochexian.top

Go:   return a, b
来源：http://wrx.guowangkeji.top

Ruby: return a, b
来源：http://nae.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://for.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://dsy.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://ehe.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jxp.nwbrower.top

JS:   const square = x => x * x;
来源：http://scs.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://bmz.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://toy.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wbb.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://kue.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yyd.birdmap.top

[C07] 把函数作为参数传入
来源：http://nwi.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tnu.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://zli.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vdy.quarkkingdee.top

TS:   arr.map(String)
来源：http://vbm.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fsr.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wkl.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://ngs.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://tin.haohaochexian.top

[C08] 闭包
来源：http://bqb.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jvu.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://far.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hrr.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wrk.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gbo.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gbh.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://whj.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ssg.haohaochexian.top

[C09] 递归
来源：http://whv.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ebh.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lmb.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kbl.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lxe.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dfr.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bac.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zlh.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://buu.andypj.xyz

[C10] 变量作用域
来源：http://wtr.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://exa.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gql.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://doe.cqqwz.cn

TS:   同 JS
来源：http://tcg.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://gul.zhengqikj.top

Go:   花括号块级作用域
来源：http://jty.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tyu.nwbrower.top

C#:   块级作用域
来源：http://bam.ivvv.top

[C11] 模块导入与导出
来源：http://buw.uphjek.com

Py:   from module import func
来源：http://luh.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://nha.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sze.aibaodan.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xhx.dianchejie.cn

Java: import java.util.List;
来源：http://gty.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rgg.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://gyk.zycfv.cn

C#:   using System.Text;
来源：http://rqm.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://mue.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://adm.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://tew.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://gua.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://obi.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nkn.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://mid.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://tfk.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zii.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://gdj.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vbs.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://grr.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nro.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tpd.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://ffm.fktsv.cn

Go:   func add(a, b int) int
来源：http://btu.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wky.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ovt.shzxlz.cn


<!-- 参考信息 -->