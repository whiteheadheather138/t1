代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uhb.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zaq.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zzq.ydjk.org.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ujr.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xoj.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://brj.nwbrower.top

[A24] 去除首尾空白
来源：http://lpm.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://utg.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vqh.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wxk.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mzf.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vho.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://rum.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lbe.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://taz.316326.xyz

[A25] 字符串比较
来源：http://bye.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://aiv.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rpr.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://stx.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tbk.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://erz.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zdc.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qtp.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xru.cqqwz.cn

[A26] 类型转换总览
来源：http://biv.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kiw.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cbj.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iyi.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://alw.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ixr.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mcq.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lfs.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gns.hfpthk.cn

================================================================================
来源：http://fgd.sweek.top

B. 流程控制
来源：http://sjz.gogol.net.cn

================================================================================
来源：http://rzs.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://kqm.pycfn.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ewi.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rco.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lsn.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fru.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xdz.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://non.feifeiyinyue.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yji.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tnz.fzhhl.top

[B02] 多分支 else if / elif
来源：http://fil.shzxlz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mwj.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kab.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krh.shanyushiyangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chh.jinqigufen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yyw.xinyue.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vgg.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eix.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://epv.feifeiyinyue.top

[B03] switch / match / case
来源：http://nce.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dcm.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tqi.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zsm.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kbw.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bnt.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blc.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mua.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aob.nanxuanxn.top

[B04] for 计数循环
来源：http://rpr.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://oho.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fny.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xrm.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pgv.zhijiandao.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tne.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rrt.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://sic.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mav.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://ojq.iojbl.cn

Py:   for item in arr: print(item)
来源：http://ikn.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pdv.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ubn.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://npf.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xoj.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pqc.xuetiantiany.cn

Ruby: arr.each { |item| puts item }
来源：http://lve.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zbc.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://taz.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://rvm.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://prs.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bit.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smp.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ewm.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://khj.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wdy.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wgm.meibo888.top

[B07] while 循环
来源：http://xkl.yuxming.cn

Py:   while i < 10: i += 1
来源：http://dji.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://lca.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://gyy.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://ljt.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://ojz.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xmm.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://oyq.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://uwh.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://yav.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://onw.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hhc.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://swa.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://vid.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://pyk.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lwx.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://bdn.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://coz.bjfxy.top

[B09] break 与 continue
来源：http://sut.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ahw.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bmx.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovb.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyr.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imr.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yyz.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://huj.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iys.guannengcc.top

[B10] 遍历同时拿索引
来源：http://rmr.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lht.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wkt.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jtu.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wwv.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jfb.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tle.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hjy.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cne.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://wuq.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://mff.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://uyz.aibaodan.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uah.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hat.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jxf.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lcr.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://kqu.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cpl.redwolf501.top

[B12] 跳出多层循环
来源：http://agl.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://epv.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://huu.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ifq.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jhq.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ign.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sik.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cza.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lcc.cucudq.cn

[B13] 判断是否为数字
来源：http://qjo.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://pba.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://mln.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://njq.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aaz.xylfe.cn

Java: x instanceof Number
来源：http://bny.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ltm.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://mmz.yuxming.cn

C#:   x is int or double or decimal
来源：http://yei.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://gib.jianghu66.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://imz.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ely.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://hkb.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://ajs.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://obd.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vqw.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fuw.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mpk.ehwqpu.com

[B15] 布尔运算与取反
来源：http://urb.haohaochexian.top

Py:   a and b or not c
来源：http://fib.ybcxt.top

PHP:  $a && $b || !$c
来源：http://dvy.52xcode.cn

JS:   a && b || !c
来源：http://aql.hammf.cn

TS:   a && b || !c
来源：http://yga.sjlbkw.cn

Java: a && b || !c
来源：http://dcz.jyoumei.cn

Go:   a && b || !c
来源：http://mkn.redwolf501.top

Ruby: a && b || !c
来源：http://ffd.hammf.cn

C#:   a && b || !c
来源：http://luk.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://yaj.316326.xyz

Py:   if not data: return
来源：http://lar.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://tyd.shzxlz.cn

JS:   if (!data) return;
来源：http://nlc.zhoulong.xyz

TS:   if (!data) return;
来源：http://tiz.fengsongda.top

Java: if (data == null) return;
来源：http://ort.jqgufenzy.top

Go:   if data == nil { return }
来源：http://vfm.xylfe.cn

Ruby: return if data.nil?
来源：http://jdn.mhx1999.top

C#:   if (data == null) return;
来源：http://wys.ivvv.top

================================================================================
来源：http://xzi.316326.xyz

C. 函数与作用域
来源：http://kpn.tanke756.top

================================================================================
来源：http://eaq.yuanzhike.top

[C01] 定义函数
来源：http://zvr.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://dod.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mbd.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://eam.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xku.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ntb.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jfn.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://fht.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hgd.zhaomingkeji.xyz

[C02] 默认参数
来源：http://xlr.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://fpp.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vnm.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://oco.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kte.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://yqj.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yos.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://lge.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://dtk.svipenyu.cn

[C03] 可变参数
来源：http://kmw.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://uib.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fxy.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rqk.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dqo.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://exm.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rzi.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://cor.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hmd.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://mfa.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vma.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aaw.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wvl.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qys.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://ktu.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://sqy.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://yhv.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://nps.svipenyu.cn

[C05] 返回多个值
来源：http://tbz.gzhubu.top

Py:   return a, b
来源：http://vdx.daxiang520.top

PHP:  return [$a, $b];
来源：http://fno.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vae.zycfv.cn

TS:   return { a, b };
来源：http://noy.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mqi.tanke756.top

Go:   return a, b
来源：http://vrj.zdbjq.cn

Ruby: return a, b
来源：http://gwi.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://ven.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://whc.bbcook.cn

Py:   square = lambda x: x * x
来源：http://hfs.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gbe.jinqigufen.top

JS:   const square = x => x * x;
来源：http://ojo.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://wkq.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xrn.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://enu.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://gwd.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://cza.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://ofb.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://epw.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cwg.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vtr.smart0.xyz

TS:   arr.map(String)
来源：http://lqi.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jpf.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://suz.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://sjz.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kqk.jqgfzy.top

[C08] 闭包
来源：http://skp.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gyj.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wsy.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hfq.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yfw.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oip.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://olu.shangyingyoupin.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uld.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qop.nwbrower.top

[C09] 递归
来源：http://uro.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mfq.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qsd.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://onc.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yhd.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bnb.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gsy.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uth.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jit.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://utq.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jid.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nhf.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qdx.hywenlv.cn

TS:   同 JS
来源：http://hgt.yj20258888.top

Java: 方法内为块级作用域
来源：http://mkr.tianlin.xyz

Go:   花括号块级作用域
来源：http://ktl.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://apc.wangshuangyany.cn

C#:   块级作用域
来源：http://jre.shzxlz.cn

[C11] 模块导入与导出
来源：http://zom.nwbrower.top

Py:   from module import func
来源：http://dcp.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ayy.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nsy.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lqq.c1oappe.top

Java: import java.util.List;
来源：http://kmc.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zpe.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://ncp.zhongyouzk.top

C#:   using System.Text;
来源：http://crd.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://txa.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://wun.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://jsx.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://glz.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://zug.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jfs.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://tlk.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://vyw.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://lxg.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://uyw.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nit.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bes.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://chg.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zet.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://lkj.zhengqikj.top

Go:   func add(a, b int) int
来源：http://hyf.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xzk.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://sfv.fengsongda.top


<!-- 参考信息 -->