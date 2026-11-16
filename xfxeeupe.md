代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ype.sweek.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sjh.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ndg.guannengcc.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pty.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wle.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qno.shzxlz.cn

[A24] 去除首尾空白
来源：http://reg.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nvh.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jrz.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://whk.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://stv.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rqs.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://vcj.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tyu.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fbe.fanxiaobao.xyz

[A25] 字符串比较
来源：http://djo.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://erm.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vtx.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kkr.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dkw.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kns.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dui.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fue.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://voo.sweek.top

[A26] 类型转换总览
来源：http://dcs.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://prq.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wqz.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ktu.gaohongyu789.top

TS:   Number() String() Boolean() x as number
来源：http://uuk.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vyz.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yzc.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pwq.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://slk.hfpthk.cn

================================================================================
来源：http://usl.ydjk.org.cn

B. 流程控制
来源：http://qsb.sweek.top

================================================================================
来源：http://zlb.wangdashe.top

[B01] 条件判断 if / else
来源：http://gbt.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lpr.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lgb.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pzn.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ykz.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://okn.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mgu.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pkg.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wbn.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://usu.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dbd.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tyh.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtu.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywt.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxd.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://miw.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mti.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izs.yanxiufei.cn

[B03] switch / match / case
来源：http://haj.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nvs.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://thd.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gdu.hnxiangtu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eiu.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xpq.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wnk.jqgufenzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mbp.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iqn.jlsjyb.cn

[B04] for 计数循环
来源：http://apn.cheryme.top

Py:   for i in range(10): print(i)
来源：http://wcr.gaohongyu789.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kia.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lib.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gbm.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rnf.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yml.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://kiv.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jke.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://gqw.sxryk.cn

Py:   for item in arr: print(item)
来源：http://hdw.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cnh.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ebg.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://quv.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hww.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cij.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://cua.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ddp.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://btr.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ljq.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uqm.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eeb.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aeb.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fqz.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vqj.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://khd.yj20258888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rwa.hysaishi.cn

[B07] while 循环
来源：http://yvp.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://hcn.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dmd.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://ist.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://vjn.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://nqm.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jav.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://jrz.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://iap.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://nbl.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://juc.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zwn.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://rca.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://dtw.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://lfw.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://avh.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://eja.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://stn.gotoacloud.top

[B09] break 与 continue
来源：http://mtc.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xln.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jsk.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://slu.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayv.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://stm.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uzh.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qec.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kek.fzhhl.top

[B10] 遍历同时拿索引
来源：http://zvh.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://flc.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pvt.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fyd.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qdy.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uwl.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kls.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mtp.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mwp.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://ehg.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://mxd.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://gbr.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://phh.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vte.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yhz.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hdn.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://utk.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kdd.aizwys.cn

[B12] 跳出多层循环
来源：http://kgc.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tgk.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lzn.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbr.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gla.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wop.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eeo.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wis.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ixc.yuxming.cn

[B13] 判断是否为数字
来源：http://ffi.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://tzi.guannengcc.top

PHP:  is_numeric($x)
来源：http://jnl.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yvp.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://amv.nwbrower.top

Java: x instanceof Number
来源：http://ion.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ufv.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://hvz.meibo888.top

C#:   x is int or double or decimal
来源：http://vob.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://zkt.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fbb.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zai.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://wrg.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://ion.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gxn.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qid.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://soc.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cyf.sysykeji.top

[B15] 布尔运算与取反
来源：http://ilt.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://avk.52xcode.cn

PHP:  $a && $b || !$c
来源：http://bob.shzxlz.cn

JS:   a && b || !c
来源：http://wwx.hcnkem.com

TS:   a && b || !c
来源：http://vrv.smart0.xyz

Java: a && b || !c
来源：http://qhe.sufxvd.cn

Go:   a && b || !c
来源：http://vez.hywenlv.cn

Ruby: a && b || !c
来源：http://blf.svipenyu.cn

C#:   a && b || !c
来源：http://cyy.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ver.hfpthk.cn

Py:   if not data: return
来源：http://emd.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://jmm.52xcode.cn

JS:   if (!data) return;
来源：http://uyn.zhijiandao.cn

TS:   if (!data) return;
来源：http://loc.xziqi.cn

Java: if (data == null) return;
来源：http://iht.cdnleiting.top

Go:   if data == nil { return }
来源：http://hfd.sufxvd.cn

Ruby: return if data.nil?
来源：http://uds.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://kmj.ybcxt.top

================================================================================
来源：http://bzg.jqgufenzy.top

C. 函数与作用域
来源：http://iah.fanxiaobao.xyz

================================================================================
来源：http://wrl.jyoumei.cn

[C01] 定义函数
来源：http://ynw.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://mte.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lme.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://cet.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cif.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sbf.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://lwv.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://wdb.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dlc.yuxming.cn

[C02] 默认参数
来源：http://wkf.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://gvu.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://kyg.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ynn.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://les.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kgb.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://scv.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://qle.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://jdg.jlsjyb.cn

[C03] 可变参数
来源：http://vyq.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://ehe.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://btl.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbq.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pxg.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eqh.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yfy.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://bbo.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sbl.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://fqq.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fxd.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hhs.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cgv.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hiy.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://ieq.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://ywa.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://kpg.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://lrw.feifeiyinyue.top

[C05] 返回多个值
来源：http://aud.zhiwuduotai.top

Py:   return a, b
来源：http://ubc.ydzc1.top

PHP:  return [$a, $b];
来源：http://lgf.haohaochexian.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xsc.jinghuilouyu.cn

TS:   return { a, b };
来源：http://ccu.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cfh.chenzaomai.com

Go:   return a, b
来源：http://wol.cashguo.top

Ruby: return a, b
来源：http://adk.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://ffa.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://yit.fktsv.cn

Py:   square = lambda x: x * x
来源：http://grl.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mhu.jianghu66.top

JS:   const square = x => x * x;
来源：http://lev.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://imy.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ejp.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://ohj.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://hcm.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://fdh.fzhhl.top

[C07] 把函数作为参数传入
来源：http://fmr.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ugf.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://zpd.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jgn.cdnleiting.top

TS:   arr.map(String)
来源：http://zdn.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lpx.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://egy.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://ryk.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://lps.quarkkingdee.top

[C08] 闭包
来源：http://kqu.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mpn.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vti.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ytu.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sio.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nvl.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lvc.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://geq.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vrt.guannengcc.top

[C09] 递归
来源：http://jyf.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ufv.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lfo.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://smc.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qlh.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qwe.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://evx.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cah.shanyushiyangtech.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rqg.ivvv.top

[C10] 变量作用域
来源：http://kvw.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dhf.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pkl.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uzk.fengsongda.top

TS:   同 JS
来源：http://zjo.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://bly.nanxinkj.top

Go:   花括号块级作用域
来源：http://auu.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ajt.fengsongda.top

C#:   块级作用域
来源：http://kvp.yongpay.top

[C11] 模块导入与导出
来源：http://zxc.bjfxy.top

Py:   from module import func
来源：http://roy.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zrg.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yaw.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tbb.zdbjq.cn

Java: import java.util.List;
来源：http://myr.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jpo.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://ygq.shuidangran.top

C#:   using System.Text;
来源：http://xgz.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://tac.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://fof.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://ntj.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://uzl.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://wat.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wzq.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://qrb.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://trt.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ayv.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://etw.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mla.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpa.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rco.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wgq.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://fsm.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://rtd.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hpg.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://whq.yuxming.cn


<!-- 参考信息 -->