代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wio.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ito.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nfd.ehwqpu.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rom.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://wxc.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://djj.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dpi.zhengqikj.top

[A25] 字符串比较
来源：http://pdw.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://lir.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bky.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wxb.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fts.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bll.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bdc.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://owc.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kke.gzhubu.top

[A26] 类型转换总览
来源：http://hvf.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yta.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zcx.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hwv.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://wrm.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mao.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://duk.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mfc.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uib.jqgufenzy.top

================================================================================
来源：http://sfr.shanyushiyangtech.top

B. 流程控制
来源：http://yxr.shangyingyoupin.top

================================================================================
来源：http://rxp.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://zrv.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hfu.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tiy.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dka.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ssr.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dbq.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pbn.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://irq.fktsv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jkg.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://dan.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dcx.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zqx.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jul.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hgf.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvo.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wqq.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xlq.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahl.zhongyouzk.top

[B03] switch / match / case
来源：http://wlu.cheryme.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jjo.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eiw.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kio.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mym.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aqw.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hsv.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kyv.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ifb.shanyushiyangtech.top

[B04] for 计数循环
来源：http://zew.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://cfg.c1oappe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pzc.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tuf.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kzi.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://psr.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wig.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://wlv.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jll.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://mjh.yuxming.cn

Py:   for item in arr: print(item)
来源：http://wge.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nwp.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vbj.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://xyb.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mgq.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pog.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://gse.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lzk.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://cnd.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qlg.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ovt.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bgj.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wuw.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qpk.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pdu.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uvm.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iqt.havefunace.top

[B07] while 循环
来源：http://wbt.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://ufl.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://epx.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://lui.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://rxo.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://hwr.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mxn.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://iit.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://nsf.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://xkp.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://ddk.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://dzc.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://vng.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://sdi.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://ntb.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://djb.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://twk.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://scx.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://vdk.tanke756.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjb.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zmo.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nln.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kak.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyq.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://djk.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vev.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjp.pycfn.com

[B10] 遍历同时拿索引
来源：http://ngo.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gcb.zhoulong.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qsk.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://adl.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lmi.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wni.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xyi.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ssg.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://isc.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://dql.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://bty.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://zgq.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nej.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mve.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uxd.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zhz.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://nrl.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zcf.sysykeji.top

[B12] 跳出多层循环
来源：http://xft.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://sgi.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ygh.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhl.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rtd.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eld.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vjr.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uly.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rkx.daria6918.cn

[B13] 判断是否为数字
来源：http://ctn.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://qqu.bbcook.cn

PHP:  is_numeric($x)
来源：http://nrl.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hqe.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cbl.jqgufenzy.top

Java: x instanceof Number
来源：http://hep.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tcq.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://dbe.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://grj.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://wvg.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ypa.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fna.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://ehg.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://roa.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bgd.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdv.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://chi.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://umf.guannengcc.top

[B15] 布尔运算与取反
来源：http://ptc.xuanzx.com

Py:   a and b or not c
来源：http://pon.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://suh.yvedp.cn

JS:   a && b || !c
来源：http://bnr.andypj.xyz

TS:   a && b || !c
来源：http://zmq.guannengcc.top

Java: a && b || !c
来源：http://vqv.aibaodan.cn

Go:   a && b || !c
来源：http://iaj.xinyue.icu

Ruby: a && b || !c
来源：http://auv.vqdsnc.cn

C#:   a && b || !c
来源：http://cbs.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://oeq.fehbvm.com

Py:   if not data: return
来源：http://lqf.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://wtg.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://olk.birdmap.top

TS:   if (!data) return;
来源：http://tch.wangshuangyany.cn

Java: if (data == null) return;
来源：http://uwe.hammf.cn

Go:   if data == nil { return }
来源：http://dlo.xziqi.cn

Ruby: return if data.nil?
来源：http://wll.aibaodan.cn

C#:   if (data == null) return;
来源：http://sfz.andypj.xyz

================================================================================
来源：http://slw.guowangkeji.top

C. 函数与作用域
来源：http://jef.hesvh.cn

================================================================================
来源：http://zma.jinqigufen.top

[C01] 定义函数
来源：http://jjo.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://tim.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xfe.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://pfn.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bgb.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://pud.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://uce.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://xop.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://crq.cdnleiting.top

[C02] 默认参数
来源：http://lws.havefunace.top

Py:   def greet(name="World"): return name
来源：http://skf.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mnf.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://hku.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xgv.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qus.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sri.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://ocy.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://nlb.yuanzhike.top

[C03] 可变参数
来源：http://sbv.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://fte.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ern.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://chu.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uqk.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zsg.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mby.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zye.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uki.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://jju.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qam.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xjr.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kra.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://opv.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://nlz.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://olt.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://lmp.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://xtt.jqgfzy.top

[C05] 返回多个值
来源：http://anb.yanxiufei.cn

Py:   return a, b
来源：http://bxh.ivvv.top

PHP:  return [$a, $b];
来源：http://hzu.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tzb.jlsjyb.cn

TS:   return { a, b };
来源：http://noc.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xvr.nanxuanxn.top

Go:   return a, b
来源：http://znm.yangfankeji.com

Ruby: return a, b
来源：http://dtb.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://fkz.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://aoa.sweek.top

Py:   square = lambda x: x * x
来源：http://gxx.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hsd.vehdjk.com

JS:   const square = x => x * x;
来源：http://rxi.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://hud.hcnkem.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sww.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fzw.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://jic.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://aiu.havefunace.top

[C07] 把函数作为参数传入
来源：http://ntd.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xon.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://flq.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xpb.jianghu66.top

TS:   arr.map(String)
来源：http://uke.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cox.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rng.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://rmu.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hnr.jianghu66.top

[C08] 闭包
来源：http://vwx.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xlj.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nqa.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://itm.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uxp.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gni.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bex.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pmy.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sua.hywenlv.cn

[C09] 递归
来源：http://xpj.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ueb.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nzl.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dtn.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qap.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qbc.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vvs.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bnd.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://azk.xuanzx.com

[C10] 变量作用域
来源：http://olo.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aac.xylfe.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jdq.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jyb.jinqigfzy.top

TS:   同 JS
来源：http://szi.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://vai.tarul.cn

Go:   花括号块级作用域
来源：http://clk.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wfm.daria6918.cn

C#:   块级作用域
来源：http://jhw.0kj1m.cn

[C11] 模块导入与导出
来源：http://kiw.gotoacloud.top

Py:   from module import func
来源：http://juj.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://llo.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mqp.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xcu.birdmap.top

Java: import java.util.List;
来源：http://fuk.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fim.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://axk.aibaodan.cn

C#:   using System.Text;
来源：http://kip.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://kzn.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://qgm.guannengcc.top

PHP:  (function () { echo "run"; })();
来源：http://qmr.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://ygp.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://fwb.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qjm.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://jks.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://mcm.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qhv.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://rqq.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xrg.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzy.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uil.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rjq.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dzg.yvedp.cn

Go:   func add(a, b int) int
来源：http://fus.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://upm.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iso.gogol.net.cn

[C14] 泛型函数
来源：http://lwi.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jkr.sysykeji.top

PHP:  // 无泛型
来源：http://mhu.gogol.net.cn

JS:   // 无泛型
来源：http://fed.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qby.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aaq.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ysk.shangyingyoupin.top

Ruby: # 无泛型
来源：http://fcy.bjfxy.top


<!-- 参考信息 -->