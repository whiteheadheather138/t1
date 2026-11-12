代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lms.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qrx.iojbl.cn

[A24] 去除首尾空白
来源：http://rfl.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vec.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fac.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vzj.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ssc.52xcode.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://czj.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://hqr.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://civ.cucudq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hzi.zdqjudy.top

[A25] 字符串比较
来源：http://tmf.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://oyl.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wnc.yongpay.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bmm.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://udh.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zkg.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cgx.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ppk.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kuq.birdmap.top

[A26] 类型转换总览
来源：http://cac.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cyz.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://skc.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ngd.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://hjr.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ile.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lnx.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mju.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://okr.jinyuanbaomall.cn

================================================================================
来源：http://zrv.sufxvd.cn

B. 流程控制
来源：http://kiz.mhx1999.top

================================================================================
来源：http://vzk.shuidangran.top

[B01] 条件判断 if / else
来源：http://nfv.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jfn.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hgc.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://frv.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hbv.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qaz.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tdy.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yta.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://msr.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://hjn.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cjs.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fuv.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkk.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdo.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rqw.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vbf.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wnv.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvi.yj202588.top

[B03] switch / match / case
来源：http://jfc.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xwo.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tib.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ikh.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zir.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cfg.bbcook.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://foc.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rjx.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://spf.sufxvd.cn

[B04] for 计数循环
来源：http://lqk.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://ird.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://inp.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dwk.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gdu.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jcp.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yey.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://jcw.meibo888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zfr.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://grb.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://xlc.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fsw.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://qod.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://egd.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://chc.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uss.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://gmp.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vwd.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://mht.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://vjp.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xzr.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ndd.cucudq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tyf.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rmn.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oqw.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://duf.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hkf.cheryme.top

[B07] while 循环
来源：http://xqt.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://eno.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://tuj.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://zvg.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://mvo.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://xgn.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gtt.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://okl.sweek.top

C#:   while (i < 10) { i++; }
来源：http://wsp.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://pwd.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://qkc.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://vad.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://ngy.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://gyv.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://ybo.daxiang520.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pbq.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://zsa.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://omd.ydzc1.top

[B09] break 与 continue
来源：http://hfz.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://djc.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dak.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvb.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sak.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ygq.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://flq.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aho.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxs.cashguo.top

[B10] 遍历同时拿索引
来源：http://aay.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gvh.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pef.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mta.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ozi.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gqu.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qaa.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qsg.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://srn.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://kfq.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://zwn.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://qkq.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wzp.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wph.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ldi.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nuf.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://hop.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://skj.ctjpmb.com

[B12] 跳出多层循环
来源：http://sav.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ijz.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dik.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqs.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nhr.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tbj.gotoacloud.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tde.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://frt.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xgh.sjlbkw.cn

[B13] 判断是否为数字
来源：http://cif.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://tjq.havefunace.top

PHP:  is_numeric($x)
来源：http://cvl.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sot.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iay.kuanghao11.cn

Java: x instanceof Number
来源：http://gau.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mfq.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://ykb.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://uvb.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://nnt.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uki.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pbg.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://jhv.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://trv.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://ykx.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gbz.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rcp.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://npr.yuanzhike.top

[B15] 布尔运算与取反
来源：http://jfz.316326.xyz

Py:   a and b or not c
来源：http://bck.yvedp.cn

PHP:  $a && $b || !$c
来源：http://niq.tianlin.xyz

JS:   a && b || !c
来源：http://vho.cashguo.top

TS:   a && b || !c
来源：http://zrt.uphjek.com

Java: a && b || !c
来源：http://png.birdmap.top

Go:   a && b || !c
来源：http://lfw.bjfxy.top

Ruby: a && b || !c
来源：http://zxq.hammf.cn

C#:   a && b || !c
来源：http://pan.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://uqh.jyoumei.cn

Py:   if not data: return
来源：http://hln.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://tig.hysaishi.cn

JS:   if (!data) return;
来源：http://opp.hywenlv.cn

TS:   if (!data) return;
来源：http://wzb.52xcode.cn

Java: if (data == null) return;
来源：http://duq.cqqwz.cn

Go:   if data == nil { return }
来源：http://xmy.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://qhp.jianghu66.top

C#:   if (data == null) return;
来源：http://zzj.tanke756.top

================================================================================
来源：http://vmy.yuanzhike.top

C. 函数与作用域
来源：http://qtb.jinqigufen.top

================================================================================
来源：http://uis.tarul.cn

[C01] 定义函数
来源：http://fro.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://aym.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://icp.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://pef.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wwv.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ssf.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://cvi.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://ila.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://obk.zhongyouzk.top

[C02] 默认参数
来源：http://cgd.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://bif.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hgz.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://rha.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yzy.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fso.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zpb.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://zyv.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://qjv.hammf.cn

[C03] 可变参数
来源：http://uzk.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://yst.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ztn.epnwcf.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wqf.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hvc.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aro.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qyb.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oxg.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gsg.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://vhv.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lnn.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ana.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zws.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dyu.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://znv.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://hit.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://txk.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://lyg.gzhubu.top

[C05] 返回多个值
来源：http://mth.quarkkingdee.top

Py:   return a, b
来源：http://jvw.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://xpn.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://ygs.guannengcc.top

TS:   return { a, b };
来源：http://phu.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ffu.xinyue.icu

Go:   return a, b
来源：http://rqj.gaohongyu789.top

Ruby: return a, b
来源：http://xgr.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://hzs.yj20258.top

[C06] 匿名函数 / lambda
来源：http://nxu.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://zxc.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ntj.hcnkem.com

JS:   const square = x => x * x;
来源：http://oux.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://llp.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ryg.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xpq.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://pqq.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://hnm.yj20258.top

[C07] 把函数作为参数传入
来源：http://kwe.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://spr.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://yny.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hlr.hnxiangtu.top

TS:   arr.map(String)
来源：http://qem.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ekk.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gng.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://bpu.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eky.feifeiyinyue.top

[C08] 闭包
来源：http://kyy.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cjs.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jee.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ocr.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ecp.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ddc.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ssq.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtf.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nvw.hysaishi.cn

[C09] 递归
来源：http://fjy.jinqigufen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nyt.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wrn.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qpi.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tge.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hog.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ssa.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tpx.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cql.quarkkingdee.top

[C10] 变量作用域
来源：http://tyg.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iga.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://afp.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hrn.cqqwz.cn

TS:   同 JS
来源：http://ogx.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://wdo.vqdsnc.cn

Go:   花括号块级作用域
来源：http://efh.yuxming.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dfs.jinyuanbaomall.cn

C#:   块级作用域
来源：http://ajf.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://nri.cheryme.top

Py:   from module import func
来源：http://jhs.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://rkt.jianghu66.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dob.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://adg.snrcjt.cn

Java: import java.util.List;
来源：http://ubg.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ecc.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://onf.ydjk.org.cn

C#:   using System.Text;
来源：http://rvz.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://nit.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://xcj.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://elb.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://jok.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://svh.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tip.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://dct.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://bmv.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cyc.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://owr.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://exl.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://voo.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nfn.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://csi.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://dfd.52xcode.cn

Go:   func add(a, b int) int
来源：http://tqo.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fsj.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://muz.iojbl.cn

[C14] 泛型函数
来源：http://giu.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mqq.zhongyouzk.top

PHP:  // 无泛型
来源：http://zob.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://gjm.guannengcc.top


<!-- 参考信息 -->