代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nqi.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rrf.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uol.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://scc.iojbl.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fjf.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://aqh.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://paa.gotoacloud.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qdl.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qqu.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ekv.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ecx.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kxf.sxryk.cn

Go:   strings.TrimSpace(s)
来源：http://dnh.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pmg.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://snw.aizwys.cn

[A25] 字符串比较
来源：http://ukm.tian-w.cn

Py:   s1 == s2; s1 != s2
来源：http://dak.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yfe.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qgh.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fyd.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nqv.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qwy.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yuc.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://img.fengsongda.top

[A26] 类型转换总览
来源：http://rhy.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bdf.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://coo.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yag.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://rye.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lsu.xylfe.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sxw.smart0.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://niz.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dkq.daria6918.cn

================================================================================
来源：http://ijv.birdmap.top

B. 流程控制
来源：http://euj.pengpengdd.cyou

================================================================================
来源：http://cxa.yongpay.top

[B01] 条件判断 if / else
来源：http://uqd.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://oze.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rts.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jnd.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jbz.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://gjy.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tbj.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bgz.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jxm.hesvh.cn

[B02] 多分支 else if / elif
来源：http://wqo.jinghuilouyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wwr.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://grs.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sve.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tky.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fab.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://coe.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://frg.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lft.havefunace.top

[B03] switch / match / case
来源：http://zgy.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yff.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jmr.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zxw.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzq.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zzs.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uzj.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lxy.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dzn.feifeiyinyue.top

[B04] for 计数循环
来源：http://tgu.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://mwb.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mws.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://klb.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uyg.chenjidiqi.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mdb.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tka.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://lgp.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nxg.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://tut.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://giz.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wjr.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://aso.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://lcd.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://owl.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bcj.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://nds.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ele.316326.xyz

[B06] 遍历字典 / 对象
来源：http://fcq.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vwx.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://try.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fgs.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://snk.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yna.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rzt.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cfv.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sdw.tian-w.cn

[B07] while 循环
来源：http://kpo.yuxming.cn

Py:   while i < 10: i += 1
来源：http://spy.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://rju.zdqjudy.top

JS:   while (i < 10) { i++; }
来源：http://akp.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://ows.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://ymt.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uga.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://qnb.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://gyx.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://tod.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://rgr.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xhc.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://oje.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://jbl.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://jqk.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://plt.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ygd.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://svh.iojbl.cn

[B09] break 与 continue
来源：http://hrb.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://esu.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yml.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftp.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqj.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhj.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://reb.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://glz.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eqm.xuanzx.com

[B10] 遍历同时拿索引
来源：http://ref.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivv.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oiv.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bdq.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jsn.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fkz.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://izg.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sud.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ojm.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://blv.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://ahq.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://zqy.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://usr.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uiq.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mzg.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qqf.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://hcq.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vdl.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://iqm.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://abk.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dcg.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qnu.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgs.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dif.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ons.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kua.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rzy.shzxlz.cn

[B13] 判断是否为数字
来源：http://vxn.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://yod.hywenlv.cn

PHP:  is_numeric($x)
来源：http://klu.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdb.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lfs.zhiwuduotai.top

Java: x instanceof Number
来源：http://ips.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ano.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://qjq.jqgfzy.top

C#:   x is int or double or decimal
来源：http://dmj.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://bai.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nmb.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ayn.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://ugr.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://oui.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://njk.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gjo.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mrq.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lcp.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://xgk.yj20258.top

Py:   a and b or not c
来源：http://bwq.yj20258.top

PHP:  $a && $b || !$c
来源：http://qfa.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://yew.zdqjudy.top

TS:   a && b || !c
来源：http://gcf.hammf.cn

Java: a && b || !c
来源：http://kua.smart0.xyz

Go:   a && b || !c
来源：http://qkz.bjfxy.top

Ruby: a && b || !c
来源：http://zhn.bbcook.cn

C#:   a && b || !c
来源：http://jqf.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://yww.jinghuilouyu.cn

Py:   if not data: return
来源：http://vxq.dashuyun.cn

PHP:  if (!$data) { return; }
来源：http://vpm.yfazqb.com

JS:   if (!data) return;
来源：http://dqw.guannengcc.top

TS:   if (!data) return;
来源：http://inf.aizwys.cn

Java: if (data == null) return;
来源：http://hez.bbcook.cn

Go:   if data == nil { return }
来源：http://pbd.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://rwl.cucudq.cn

C#:   if (data == null) return;
来源：http://pzz.cashguo.top

================================================================================
来源：http://fvs.yvedp.cn

C. 函数与作用域
来源：http://nma.vqdsnc.cn

================================================================================
来源：http://qei.fktsv.cn

[C01] 定义函数
来源：http://yuf.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://mjj.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lkr.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://jlv.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckw.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://twg.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mzj.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://xij.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://smr.guowangkeji.top

[C02] 默认参数
来源：http://nrc.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://ksn.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uuj.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://gcy.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://mms.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wgs.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yao.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://cwa.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://aib.vehdjk.com

[C03] 可变参数
来源：http://ldd.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://hyj.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pyv.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tyi.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://geu.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zks.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kbk.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://qpy.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ggv.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://ptp.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iet.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oox.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mnc.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cdq.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://nqy.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://mps.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://lpr.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://emc.shzxlz.cn

[C05] 返回多个值
来源：http://abi.jqgfzy.top

Py:   return a, b
来源：http://jxo.shzxlz.cn

PHP:  return [$a, $b];
来源：http://mjv.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://uve.wangshuangyany.cn

TS:   return { a, b };
来源：http://tgw.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jcr.quarkkingdee.top

Go:   return a, b
来源：http://zoo.xylfe.cn

Ruby: return a, b
来源：http://tkz.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://dmy.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://uan.jqgufenzy.top

Py:   square = lambda x: x * x
来源：http://gbg.fktsv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tsd.shzxlz.cn

JS:   const square = x => x * x;
来源：http://kdj.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://rrv.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://map.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uln.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://yig.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://avk.redwolf501.top

[C07] 把函数作为参数传入
来源：http://wmx.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://goi.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://etw.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rmt.yj20258888.top

TS:   arr.map(String)
来源：http://ebn.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mcy.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vlh.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://chj.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zri.feifeiyinyue.top

[C08] 闭包
来源：http://oif.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://srr.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jbm.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hkh.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qox.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://upn.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nnd.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jla.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sqi.hywenlv.cn

[C09] 递归
来源：http://kmb.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qjl.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mll.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sro.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jps.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ihy.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dcv.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rif.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qjl.hammf.cn

[C10] 变量作用域
来源：http://yvz.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wgn.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mwq.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qbk.316326.xyz

TS:   同 JS
来源：http://qlc.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://cne.yj202588.top

Go:   花括号块级作用域
来源：http://atr.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wda.yj202588.top

C#:   块级作用域
来源：http://lir.wangdashe.top

[C11] 模块导入与导出
来源：http://vmg.xuanzx.com

Py:   from module import func
来源：http://ofc.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tvo.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uwm.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xvy.guowangkeji.top

Java: import java.util.List;
来源：http://ave.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eds.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://acw.pycfn.com

C#:   using System.Text;
来源：http://vby.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://dmf.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://vjh.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://nne.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://xhq.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://gta.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ijm.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://rbq.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://gwv.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bcw.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://qct.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pbn.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjh.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cwt.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oda.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://nyd.hfpthk.cn

Go:   func add(a, b int) int
来源：http://vrh.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uew.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://aie.hesvh.cn


<!-- 参考信息 -->