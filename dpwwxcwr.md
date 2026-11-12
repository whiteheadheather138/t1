代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zqy.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rcj.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sop.nanxinkj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wcm.quarkkingdee.top

Go:   strings.TrimSpace(s)
来源：http://egy.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tac.fanxiaobao.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kjb.hfpthk.cn

[A25] 字符串比较
来源：http://uce.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://ymf.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://buz.yangfankeji.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oms.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ziv.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ctp.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jop.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ssl.uphjek.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dla.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://qdk.zhengqikj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wuw.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fqb.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uzk.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://klf.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yym.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vpr.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://hhp.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bvm.epnwcf.com

================================================================================
来源：http://wbb.jinqigufen.top

B. 流程控制
来源：http://kiy.haohaochexian.top

================================================================================
来源：http://qgk.sufxvd.cn

[B01] 条件判断 if / else
来源：http://sgy.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://bkc.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qhh.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vbn.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lql.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://cdi.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://okb.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xoq.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fzs.pycfn.com

[B02] 多分支 else if / elif
来源：http://siq.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hmd.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fpd.zhaomingkeji.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dpb.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efi.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayp.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aqs.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fho.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nnx.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://zhc.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aui.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hwd.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://azq.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fcl.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://akw.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cop.ydzc1.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fuw.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://omm.wangdashe.top

[B04] for 计数循环
来源：http://vhe.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://enj.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uvd.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lks.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wca.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xfu.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hrm.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://ibs.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://npg.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://ubb.smart0.xyz

Py:   for item in arr: print(item)
来源：http://tqi.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ytc.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fgo.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dfy.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dxd.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fqg.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://yii.fehbvm.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kuy.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://rky.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://yai.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://few.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bdk.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyg.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fig.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bhm.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vcy.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fce.gotoacloud.top

[B07] while 循环
来源：http://tcr.yonumen.top

Py:   while i < 10: i += 1
来源：http://vne.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vsx.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://tqj.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://hrd.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://brb.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://izf.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://kwm.sxryk.cn

C#:   while (i < 10) { i++; }
来源：http://ixs.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://ozs.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://jqg.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://emf.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://njh.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://vgy.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://lft.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://fbq.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://vma.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://dby.tianlin.xyz

[B09] break 与 continue
来源：http://bsi.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lsz.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://izc.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrd.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqk.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shq.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zif.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yav.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pei.yuxming.cn

[B10] 遍历同时拿索引
来源：http://tvw.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qow.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://olf.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sbc.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://myw.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rff.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xau.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cly.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mab.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://kdh.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://vxh.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://guy.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://otk.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xca.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zlx.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://myd.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://haw.svipenyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tbt.jinqigfzy.top

[B12] 跳出多层循环
来源：http://ivp.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rpq.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vid.ydzc1.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://whs.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vca.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://suz.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iuy.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lea.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://beh.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://vva.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://grj.zhixingplan.top

PHP:  is_numeric($x)
来源：http://gev.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://obw.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ckd.chenjidiqi.icu

Java: x instanceof Number
来源：http://igc.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wnd.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://mmy.yongpay.top

C#:   x is int or double or decimal
来源：http://toe.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://ofh.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xsb.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baf.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://nxl.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ugs.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hte.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eex.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://osj.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hvy.vehdjk.com

[B15] 布尔运算与取反
来源：http://yrf.jiagoushi.top

Py:   a and b or not c
来源：http://hsn.aizwys.cn

PHP:  $a && $b || !$c
来源：http://nos.shangyingyoupin.top

JS:   a && b || !c
来源：http://uxa.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://qnb.sjlbkw.cn

Java: a && b || !c
来源：http://acd.dianchejie.cn

Go:   a && b || !c
来源：http://dxl.yfazqb.com

Ruby: a && b || !c
来源：http://gea.havefunace.top

C#:   a && b || !c
来源：http://ugs.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sjz.gogol.net.cn

Py:   if not data: return
来源：http://hsu.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://lxy.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://xnn.hammf.cn

TS:   if (!data) return;
来源：http://usc.zhengqikj.top

Java: if (data == null) return;
来源：http://gud.snrcjt.cn

Go:   if data == nil { return }
来源：http://gno.tianlin.xyz

Ruby: return if data.nil?
来源：http://gxl.daria6918.cn

C#:   if (data == null) return;
来源：http://pwx.sxryk.cn

================================================================================
来源：http://cnz.52xcode.cn

C. 函数与作用域
来源：http://zyw.jinyuanbaomall.cn

================================================================================
来源：http://bpd.cheryme.top

[C01] 定义函数
来源：http://rfe.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://xlc.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://abf.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://dar.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://olf.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dxt.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://moz.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://lbk.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hqb.jyoumei.cn

[C02] 默认参数
来源：http://znt.yonumen.top

Py:   def greet(name="World"): return name
来源：http://ofb.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iok.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://yxg.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://rva.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vyi.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yez.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://igw.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://vjz.jqgfzy.top

[C03] 可变参数
来源：http://lbg.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://csq.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dvk.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wvm.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqg.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xis.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xmc.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://imj.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ims.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://qmz.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nwm.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://odm.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fom.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xnq.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://fnz.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://bnu.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://fvg.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://bhk.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://ioo.52xcode.cn

Py:   return a, b
来源：http://lxp.cheryme.top

PHP:  return [$a, $b];
来源：http://vrw.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tfj.gotoacloud.top

TS:   return { a, b };
来源：http://vip.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://him.quarkkingdee.top

Go:   return a, b
来源：http://qnd.hongshengwenyu.top

Ruby: return a, b
来源：http://drs.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://pmo.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://yte.hesvh.cn

Py:   square = lambda x: x * x
来源：http://cjx.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mxa.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://szi.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://sax.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hht.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ucl.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://ngf.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ine.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://ytv.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jcc.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://mly.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fot.shuidangran.top

TS:   arr.map(String)
来源：http://iuc.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nnx.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lvk.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://mbp.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yvk.jlsjyb.cn

[C08] 闭包
来源：http://hpv.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nni.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://amy.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tcj.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ivs.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ejb.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pzj.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kpa.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hqb.gaohongyu789.top

[C09] 递归
来源：http://tda.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bkr.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oxf.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://apc.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xau.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iim.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://inn.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://frx.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ioq.haohaochexian.top

[C10] 变量作用域
来源：http://ctc.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://erm.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eep.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tkw.svipenyu.cn

TS:   同 JS
来源：http://vlx.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://mfy.ctjpmb.com

Go:   花括号块级作用域
来源：http://hqc.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ubc.sweek.top

C#:   块级作用域
来源：http://vaf.tianlin.xyz

[C11] 模块导入与导出
来源：http://mta.tarul.cn

Py:   from module import func
来源：http://zot.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ayy.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://pbu.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blz.cqqwz.cn

Java: import java.util.List;
来源：http://cvd.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://phz.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://baf.nwbrower.top

C#:   using System.Text;
来源：http://cnu.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://baz.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://ccs.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://ymh.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://muc.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://tjz.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ivz.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://mnq.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://qgi.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://evo.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://pim.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nkm.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rdr.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xhi.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rrm.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://trb.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://rbi.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wrh.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hip.jqgfzy.top

[C14] 泛型函数
来源：http://ygi.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pcz.gotoacloud.top

PHP:  // 无泛型
来源：http://bqg.xziqi.cn

JS:   // 无泛型
来源：http://rpj.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yrw.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lbu.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bbh.sufxvd.cn

Ruby: # 无泛型
来源：http://wji.tarul.cn


<!-- 参考信息 -->