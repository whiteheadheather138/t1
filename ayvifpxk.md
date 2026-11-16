代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gbt.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rqe.ybcxt.top

[A24] 去除首尾空白
来源：http://hfq.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xga.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kvl.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vll.haohaochexian.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lul.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jsd.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://vfa.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mgo.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tpp.zhijiandao.cn

[A25] 字符串比较
来源：http://wte.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://djc.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fit.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rss.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mwn.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bns.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ppy.feifeiyinyue.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ldl.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://way.yangfankeji.com

[A26] 类型转换总览
来源：http://rxn.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jmv.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vys.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pmx.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://jeu.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vrd.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fat.hcnkem.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://koj.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vae.nanxuanxn.top

================================================================================
来源：http://ccy.jinqigufen.top

B. 流程控制
来源：http://kpt.chenzaomai.com

================================================================================
来源：http://vie.jinqigufen.top

[B01] 条件判断 if / else
来源：http://woa.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://qql.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oqz.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cgb.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cxh.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hpv.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hao.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oyp.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xmy.epnwcf.com

[B02] 多分支 else if / elif
来源：http://pbr.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://juh.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://phk.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okc.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ldm.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zsj.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yfr.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mjk.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://stg.nanxinkj.top

[B03] switch / match / case
来源：http://szq.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cqx.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ivj.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dyt.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bsw.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bdq.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tmj.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kif.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://myq.snrcjt.cn

[B04] for 计数循环
来源：http://mcg.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://nmn.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://shs.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mgb.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tto.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://crk.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gvw.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://mog.meibo888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jds.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://dpu.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://wol.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vro.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dtd.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://kgs.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tlv.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cve.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://crb.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uda.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://qbc.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cws.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ahc.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aas.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cof.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://txa.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mvl.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ojy.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://idg.dianchejie.cn

[B07] while 循环
来源：http://bdq.yonumen.top

Py:   while i < 10: i += 1
来源：http://upo.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gtd.yuanzhike.top

JS:   while (i < 10) { i++; }
来源：http://asa.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://pmy.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://dlu.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://muo.yvedp.cn

Ruby: while i < 10; i += 1; end
来源：http://bvg.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://hmp.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://vnq.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://obi.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fwo.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://uxf.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://dhx.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://kdo.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wgq.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://uwh.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://zqd.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://svn.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lau.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fir.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oed.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jch.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jpk.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gjp.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vvg.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpr.aizwys.cn

[B10] 遍历同时拿索引
来源：http://tnl.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xrq.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cnh.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bfw.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jmk.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iai.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mmj.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tsx.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uxm.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://lcp.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://hch.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://olc.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pnr.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ihs.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kdv.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dhb.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://ehv.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kmz.ydjk.org.cn

[B12] 跳出多层循环
来源：http://pyq.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://txz.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fhe.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zke.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://son.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xeo.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ljs.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ldv.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mxh.zhixingplan.top

[B13] 判断是否为数字
来源：http://tux.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://prv.xziqi.cn

PHP:  is_numeric($x)
来源：http://jmu.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bep.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tjs.ivvv.top

Java: x instanceof Number
来源：http://hxo.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ldw.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://dea.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://gqg.shuidangran.top

[B14] 判断值是否在集合内
来源：http://who.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lrr.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kwr.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://rph.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://fen.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hhy.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eae.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nyj.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xak.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://fbz.cucudq.cn

Py:   a and b or not c
来源：http://mpz.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://ppi.jqgfzy.top

JS:   a && b || !c
来源：http://edn.52xcode.cn

TS:   a && b || !c
来源：http://ugf.guowangkeji.top

Java: a && b || !c
来源：http://jph.redwolf501.top

Go:   a && b || !c
来源：http://tbj.yonumen.top

Ruby: a && b || !c
来源：http://tzf.daxiang520.top

C#:   a && b || !c
来源：http://ppj.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qol.ydjk.org.cn

Py:   if not data: return
来源：http://wvq.yonumen.top

PHP:  if (!$data) { return; }
来源：http://gjr.redwolf501.top

JS:   if (!data) return;
来源：http://ttk.ybcxt.top

TS:   if (!data) return;
来源：http://zgu.ydzc1.top

Java: if (data == null) return;
来源：http://trx.jqgfzy.top

Go:   if data == nil { return }
来源：http://yjg.nanxinkj.top

Ruby: return if data.nil?
来源：http://bsp.zhengqikj.top

C#:   if (data == null) return;
来源：http://kyw.hammf.cn

================================================================================
来源：http://sis.zhoulong.xyz

C. 函数与作用域
来源：http://xni.daria6918.cn

================================================================================
来源：http://gmg.nwbrower.top

[C01] 定义函数
来源：http://bci.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://yof.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://udc.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://ayk.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://akk.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hvs.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://gsj.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://bhn.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ljc.sysykeji.top

[C02] 默认参数
来源：http://xvc.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://brm.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://igr.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://den.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bak.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xyp.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://njd.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://tfi.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://hyt.yongpay.top

[C03] 可变参数
来源：http://dxn.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://jsp.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lqv.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qha.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kae.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hhr.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kxa.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gdw.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zdo.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://yrd.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fkt.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eea.xuetiantiany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://she.birdmap.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bvd.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://akh.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://wys.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://frx.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://orm.yueranfly.top

[C05] 返回多个值
来源：http://ben.gaohongyu789.top

Py:   return a, b
来源：http://obs.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://vzx.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://wee.sxryk.cn

TS:   return { a, b };
来源：http://ysg.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kxi.xziqi.cn

Go:   return a, b
来源：http://pgi.cashguo.top

Ruby: return a, b
来源：http://wxs.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://hdz.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://dwg.mhx1999.top

Py:   square = lambda x: x * x
来源：http://jsf.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://jrx.316326.xyz

JS:   const square = x => x * x;
来源：http://goo.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://shr.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ysn.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://jje.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://wed.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://mjc.birdmap.top

[C07] 把函数作为参数传入
来源：http://fog.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cgb.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qpa.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nqw.hongshengwenyu.top

TS:   arr.map(String)
来源：http://zmu.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ime.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://maq.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://pox.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://twc.nanxinkj.top

[C08] 闭包
来源：http://gml.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rzy.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://btf.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://svx.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fsk.yanxiufei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://skc.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tgl.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eiu.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oec.fanxiaobao.xyz

[C09] 递归
来源：http://nab.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://igz.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iso.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mew.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eky.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bku.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bej.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pgr.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qyi.hywenlv.cn

[C10] 变量作用域
来源：http://gjn.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ahg.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://erh.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uxk.shzxlz.cn

TS:   同 JS
来源：http://vij.shzxlz.cn

Java: 方法内为块级作用域
来源：http://ljw.gogol.net.cn

Go:   花括号块级作用域
来源：http://rbo.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ifa.xinyue.icu

C#:   块级作用域
来源：http://tbw.hnxiangtu.top

[C11] 模块导入与导出
来源：http://dew.ywan-chungtsiang.top

Py:   from module import func
来源：http://acb.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zye.jianghu66.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nev.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cje.jlsjyb.cn

Java: import java.util.List;
来源：http://wvo.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://udu.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://xjq.c1oappe.top

C#:   using System.Text;
来源：http://ptu.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://oak.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://jgi.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://ilw.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://sov.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://ruv.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gjv.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://oih.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://unn.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://gcv.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://uxs.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sru.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yjt.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tno.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vsg.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://bog.cucudq.cn

Go:   func add(a, b int) int
来源：http://ais.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bsh.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://efz.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://kll.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qvc.yuanzhike.top

PHP:  // 无泛型
来源：http://diq.xuanzx.com

JS:   // 无泛型
来源：http://lsa.gogol.net.cn


<!-- 参考信息 -->