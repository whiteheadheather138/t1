代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vbk.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://prp.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bzk.kuanghao11.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lrz.wangdashe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xfc.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nfj.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://zrp.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gdi.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qjn.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://atz.c1oappe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://edc.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://glh.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://ize.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tce.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uep.hongshengwenyu.top

[A25] 字符串比较
来源：http://mha.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://jno.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tqj.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://apj.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eip.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ypj.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mfb.fzhhl.top

Ruby: s1 == s2; s1 <=> s2
来源：http://err.dianchejie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://abj.chenjidiqi.icu

[A26] 类型转换总览
来源：http://dfd.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zxs.hcnkem.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hfu.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kdz.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://icx.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lur.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yzx.shzxlz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rtb.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ygj.sjlbkw.cn

================================================================================
来源：http://hyw.havefunace.top

B. 流程控制
来源：http://kjd.wangshuangyany.cn

================================================================================
来源：http://alf.birdmap.top

[B01] 条件判断 if / else
来源：http://dcb.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pqp.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qfl.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bht.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wdm.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wbn.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://npn.sweek.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lwl.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xxv.yj20258888.top

[B02] 多分支 else if / elif
来源：http://omr.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wnu.xuetiantiany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vci.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lmr.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ikv.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfk.hnqzz.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lbd.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cty.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ekn.yanxiufei.cn

[B03] switch / match / case
来源：http://cpy.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cqi.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fot.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://khq.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dob.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xdd.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jnf.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pzc.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ihp.hfpthk.cn

[B04] for 计数循环
来源：http://dnq.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://utg.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://see.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yrd.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kab.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zuf.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qyx.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://pbh.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xbi.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://alt.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://lna.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wce.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bjb.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wqe.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://aao.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ygb.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://bwf.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wvc.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://iqw.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mlr.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gix.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rkf.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://moa.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://otc.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cea.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cdp.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baw.jqgufenzy.top

[B07] while 循环
来源：http://fyh.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://xxq.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gge.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://tod.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://fks.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://bbu.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lcj.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://qma.sxryk.cn

C#:   while (i < 10) { i++; }
来源：http://kdy.yongpay.top

[B08] do-while（至少执行一次）
来源：http://hdj.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://qzm.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fjp.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://vbe.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://dpc.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://zbu.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://evu.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://dgx.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://emz.xinyue.icu

[B09] break 与 continue
来源：http://grj.yj20258.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qid.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kli.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afm.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czs.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmc.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pfz.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sho.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjz.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://yso.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iau.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rzg.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://koj.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ejx.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://opz.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dxi.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dux.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sue.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://rig.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://ccz.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://lqd.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kcv.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dtd.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hrg.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nqq.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://shd.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pux.zycfv.cn

[B12] 跳出多层循环
来源：http://raw.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iui.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ltv.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lly.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iht.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jqs.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pfu.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nnp.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zoy.yuanzhike.top

[B13] 判断是否为数字
来源：http://vlt.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://ivc.uphjek.com

PHP:  is_numeric($x)
来源：http://xdi.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://myt.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cid.zhoulong.xyz

Java: x instanceof Number
来源：http://gfb.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://chn.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://tod.sxryk.cn

C#:   x is int or double or decimal
来源：http://wrp.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://vbk.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://grf.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xkx.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://obt.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://etr.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://baw.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zlk.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://gkf.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xba.tarul.cn

[B15] 布尔运算与取反
来源：http://lot.c1oappe.top

Py:   a and b or not c
来源：http://roc.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://ivw.epnwcf.com

JS:   a && b || !c
来源：http://mgq.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://yhf.epnwcf.com

Java: a && b || !c
来源：http://pas.yanxiufei.cn

Go:   a && b || !c
来源：http://odk.vehdjk.com

Ruby: a && b || !c
来源：http://fxe.shzxlz.cn

C#:   a && b || !c
来源：http://xwg.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://txt.yonumen.top

Py:   if not data: return
来源：http://roq.yongpay.top

PHP:  if (!$data) { return; }
来源：http://hyn.fehbvm.com

JS:   if (!data) return;
来源：http://ysg.fehbvm.com

TS:   if (!data) return;
来源：http://yzz.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://xxm.fehbvm.com

Go:   if data == nil { return }
来源：http://dao.jyoumei.cn

Ruby: return if data.nil?
来源：http://vqx.vqdsnc.cn

C#:   if (data == null) return;
来源：http://jva.bbcook.cn

================================================================================
来源：http://ioo.jinghuilouyu.cn

C. 函数与作用域
来源：http://eyw.vehdjk.com

================================================================================
来源：http://dwz.zhaomingkeji.xyz

[C01] 定义函数
来源：http://yeb.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://onx.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sjx.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://loy.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mve.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://aso.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ycr.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://hbn.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kjh.9152youxi.cn

[C02] 默认参数
来源：http://xzr.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://jcd.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jde.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://nfx.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lsy.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pnr.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://owf.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://msn.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://goa.xuetiantiany.cn

[C03] 可变参数
来源：http://mgy.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://gts.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ffj.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jxe.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pps.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xsy.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://onh.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://kcz.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ars.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://jwc.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://amx.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bmj.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kjc.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lbs.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://bkk.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://zvk.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://ipw.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://kus.meibo888.top

[C05] 返回多个值
来源：http://khg.jqgufenzy.top

Py:   return a, b
来源：http://ptr.tanke756.top

PHP:  return [$a, $b];
来源：http://wbh.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bwi.sjlbkw.cn

TS:   return { a, b };
来源：http://hpc.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vld.xuetiantiany.cn

Go:   return a, b
来源：http://uns.fanxiaobao.xyz

Ruby: return a, b
来源：http://wyz.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://gix.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://yec.quarkkingdee.top

Py:   square = lambda x: x * x
来源：http://iop.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://avo.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://why.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://kjq.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nyb.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://zaf.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://tzt.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://hap.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://fjv.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gbk.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tfr.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pid.sysykeji.top

TS:   arr.map(String)
来源：http://vif.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bdh.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dmi.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://khx.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wbk.haohaochexian.top

[C08] 闭包
来源：http://phf.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gkb.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yof.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sxv.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xrs.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wrw.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cgr.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://okc.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zpl.gotoacloud.top

[C09] 递归
来源：http://idx.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ppa.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ncn.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nuh.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hih.hywenlv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kcn.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://avt.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gci.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xwq.wangdashe.top

[C10] 变量作用域
来源：http://yje.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kxi.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mda.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qne.andypj.xyz

TS:   同 JS
来源：http://ntf.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://wok.9152youxi.cn

Go:   花括号块级作用域
来源：http://ijp.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iyi.hesvh.cn

C#:   块级作用域
来源：http://ugb.yj202588.top

[C11] 模块导入与导出
来源：http://kly.hnxiangtu.top

Py:   from module import func
来源：http://ynz.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://soy.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rjf.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jun.nwbrower.top

Java: import java.util.List;
来源：http://hsq.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eni.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://slt.zhongyouzk.top

C#:   using System.Text;
来源：http://sgd.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://ail.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://shm.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://uwu.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://cnf.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://eya.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xco.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://qpn.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://yre.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://org.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://tmf.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gsc.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldp.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://crz.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jgj.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://atj.yj20258.top

Go:   func add(a, b int) int
来源：http://zfj.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zlr.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://bnx.ehwqpu.com


<!-- 参考信息 -->