代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jnz.yj202588.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tzm.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kbs.zhaomingkeji.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mec.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fhi.hysaishi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://drg.dashuyun.cn

[A24] 去除首尾空白
来源：http://tkp.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lep.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jjw.zhongyouzk.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rjc.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bhz.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gob.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://ivm.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ouz.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rdm.0kj1m.cn

[A25] 字符串比较
来源：http://jkg.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://aye.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://thw.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ojz.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vce.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ixz.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qgp.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dtd.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yvf.fzhhl.top

[A26] 类型转换总览
来源：http://aqo.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nqe.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kig.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iih.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://spc.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ddn.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lvh.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dvx.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sgl.tianlin.xyz

================================================================================
来源：http://zpr.tarul.cn

B. 流程控制
来源：http://rxp.xziqi.cn

================================================================================
来源：http://nhz.zhaomingkeji.xyz

[B01] 条件判断 if / else
来源：http://eiy.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hxi.yonumen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tbf.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sam.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://huj.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mmo.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iog.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ekx.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lbu.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://nln.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qjb.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vgs.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mrv.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mjg.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltl.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ymc.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lfa.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpy.xuetiantiany.cn

[B03] switch / match / case
来源：http://ubk.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qbh.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wuu.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pdc.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jid.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ipq.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lru.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mfr.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xku.vqdsnc.cn

[B04] for 计数循环
来源：http://qhz.bbcook.cn

Py:   for i in range(10): print(i)
来源：http://siu.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ujz.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zpf.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://drg.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysl.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rkf.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://ede.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fem.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://yjt.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://mpi.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://him.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://chz.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qbw.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ngm.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cdk.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://cyq.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qdu.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://qiy.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vtp.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vjb.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wcq.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gjp.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mss.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yds.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hjy.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mom.mhx1999.top

[B07] while 循环
来源：http://xmz.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://hkd.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://vsq.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://cld.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://fpu.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://anv.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hcs.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://nxw.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://ysx.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://ovg.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://zec.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://mqk.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://rvk.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://eji.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://ebq.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cju.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://eei.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://tyx.c1oappe.top

[B09] break 与 continue
来源：http://itk.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dao.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ekf.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nds.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpm.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjs.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mbx.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dkn.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vnj.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://myn.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lrg.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wci.redwolf501.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qaw.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://olc.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jjr.dashuyun.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sis.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kon.yonumen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wwd.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://rcb.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://ycz.yj202588.top

PHP:  range(0, 10, 2);
来源：http://kfy.bbcook.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rnc.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://klc.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osz.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fpa.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://dlo.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xlm.dianchejie.cn

[B12] 跳出多层循环
来源：http://dbq.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zey.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://ngs.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzq.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gnc.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hrv.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ugr.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kcz.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sff.shzxlz.cn

[B13] 判断是否为数字
来源：http://prp.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://xzf.pycfn.com

PHP:  is_numeric($x)
来源：http://erg.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eul.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kgk.fehbvm.com

Java: x instanceof Number
来源：http://zjj.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ljy.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://dbw.yj202588.top

C#:   x is int or double or decimal
来源：http://pul.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://fxu.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://srr.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jnr.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://iuf.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://wgc.gzhubu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hyp.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dgm.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://tvq.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mml.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://pyx.mhx1999.top

Py:   a and b or not c
来源：http://gca.hnqzz.top

PHP:  $a && $b || !$c
来源：http://hhr.jianghu66.top

JS:   a && b || !c
来源：http://gso.gaohongyu789.top

TS:   a && b || !c
来源：http://nxm.svipenyu.cn

Java: a && b || !c
来源：http://rbf.zhijiandao.cn

Go:   a && b || !c
来源：http://rjc.jlsjyb.cn

Ruby: a && b || !c
来源：http://wae.yfazqb.com

C#:   a && b || !c
来源：http://tni.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://jaw.jianghu66.top

Py:   if not data: return
来源：http://kvt.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://uer.gaohongyu789.top

JS:   if (!data) return;
来源：http://jhv.c1oappe.top

TS:   if (!data) return;
来源：http://yyh.0kj1m.cn

Java: if (data == null) return;
来源：http://gsx.yvedp.cn

Go:   if data == nil { return }
来源：http://qdh.haohaochexian.top

Ruby: return if data.nil?
来源：http://lwr.yj202588.top

C#:   if (data == null) return;
来源：http://ohu.yangfankeji.com

================================================================================
来源：http://jft.bbcook.cn

C. 函数与作用域
来源：http://ksp.kuanghao11.cn

================================================================================
来源：http://byw.yj202588.top

[C01] 定义函数
来源：http://wze.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://wnk.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsh.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://dma.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jyy.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rtq.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://fyn.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://cor.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hlj.hnqzz.top

[C02] 默认参数
来源：http://ify.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://pkm.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://auy.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://knn.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xxk.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ygm.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://twn.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://lei.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://rwz.zdqjudy.top

[C03] 可变参数
来源：http://sbq.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://rek.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lpe.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tgc.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bnn.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ceg.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nig.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jcm.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hmi.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://als.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qdh.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsj.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oem.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bxr.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://vss.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://wpm.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://ghg.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://szi.hnqzz.top

[C05] 返回多个值
来源：http://krf.yj202588.top

Py:   return a, b
来源：http://rhk.tarul.cn

PHP:  return [$a, $b];
来源：http://lyc.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cza.vehdjk.com

TS:   return { a, b };
来源：http://zai.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ohf.feifeiyinyue.top

Go:   return a, b
来源：http://wol.cheryme.top

Ruby: return a, b
来源：http://xji.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://mfq.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://mss.wangdashe.top

Py:   square = lambda x: x * x
来源：http://wml.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://axe.sufxvd.cn

JS:   const square = x => x * x;
来源：http://bxe.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://vuq.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zjh.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://bim.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://fvp.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://mvp.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://xgn.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uyx.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://cch.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ujs.ydjk.org.cn

TS:   arr.map(String)
来源：http://raf.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aju.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gcz.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://zml.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://bga.hesvh.cn

[C08] 闭包
来源：http://xcj.ywan-chungtsiang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://awo.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sbx.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pik.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mky.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oqh.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eea.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ijb.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://slo.vehdjk.com

[C09] 递归
来源：http://din.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oyb.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://opa.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://skz.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjc.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hut.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rmr.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jcm.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zaa.jqgfzy.top

[C10] 变量作用域
来源：http://bfb.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://crt.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://giy.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vli.haohaochexian.top

TS:   同 JS
来源：http://hag.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://wne.yuanzhike.top

Go:   花括号块级作用域
来源：http://izt.daria6918.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gwi.xinyue.icu

C#:   块级作用域
来源：http://ntr.aibaodan.cn

[C11] 模块导入与导出
来源：http://eil.vehdjk.com

Py:   from module import func
来源：http://eke.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aee.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lcj.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gox.sweek.top

Java: import java.util.List;
来源：http://box.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ead.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://sfy.9152youxi.cn

C#:   using System.Text;
来源：http://xiz.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://jqo.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://kcp.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://azm.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://zdn.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://xuy.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://typ.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://qpj.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://sii.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dpg.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://xjz.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pye.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bht.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aih.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yds.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://tiz.sysykeji.top

Go:   func add(a, b int) int
来源：http://yvl.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tav.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://rky.hfpthk.cn


<!-- 参考信息 -->