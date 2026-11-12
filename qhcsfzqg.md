代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://vga.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hnr.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fdo.shangyingyoupin.top

[A25] 字符串比较
来源：http://vln.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://zmg.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://smh.yongpay.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sql.quarkkingdee.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dps.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bmp.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nzl.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://unr.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hkg.sjlbkw.cn

[A26] 类型转换总览
来源：http://dtm.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bsf.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nte.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pnu.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://ljm.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gxf.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ijw.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cvd.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hpj.hongshengwenyu.top

================================================================================
来源：http://fpb.tanke756.top

B. 流程控制
来源：http://jqm.zdbjq.cn

================================================================================
来源：http://shl.zdqjudy.top

[B01] 条件判断 if / else
来源：http://meh.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vlq.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eet.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xrz.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jfv.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://teh.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://poz.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://skq.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kdn.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://jxb.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xkl.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wzf.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fal.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lca.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bir.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hpo.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kbp.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tmi.quarkkingdee.top

[B03] switch / match / case
来源：http://akv.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hqc.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ngk.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://alr.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://swh.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ihj.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kgj.sweek.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xjg.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://awh.wangshuangyany.cn

[B04] for 计数循环
来源：http://hfj.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://qap.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ksr.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sqo.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vey.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hgw.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://phs.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://lof.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ovj.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://zzf.ydzc1.top

Py:   for item in arr: print(item)
来源：http://xpe.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://plm.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bax.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://pvf.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zxu.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iqs.sjlbkw.cn

Ruby: arr.each { |item| puts item }
来源：http://ktv.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iqk.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://qji.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qqj.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gqy.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wlt.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://utr.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vqh.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kah.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://evj.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jwv.wangshuangyany.cn

[B07] while 循环
来源：http://sqh.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://mra.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://uvp.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://zeh.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://grx.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://nlt.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ctn.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://vtm.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://jsk.meibo888.top

[B08] do-while（至少执行一次）
来源：http://msq.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://spo.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://xrb.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://kay.jinghuilouyu.cn

TS:   do { i++; } while (i < 10);
来源：http://mes.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://cpq.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://est.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://pdz.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://yio.hysaishi.cn

[B09] break 与 continue
来源：http://rvs.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jkb.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ych.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://soh.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpr.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlp.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qsf.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hah.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qtl.ydzc1.top

[B10] 遍历同时拿索引
来源：http://rke.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tzs.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qhc.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kho.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://huw.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ots.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://odl.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tfh.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rax.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://jgf.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://hcy.ivvv.top

PHP:  range(0, 10, 2);
来源：http://rif.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fjm.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lsu.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cid.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://srd.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://vnh.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://obj.hfpthk.cn

[B12] 跳出多层循环
来源：http://inm.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://hus.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uvh.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://irn.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://teb.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aut.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://onf.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sie.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iqp.cashguo.top

[B13] 判断是否为数字
来源：http://vha.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://odw.sweek.top

PHP:  is_numeric($x)
来源：http://xsq.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uoj.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wnk.haohaochexian.top

Java: x instanceof Number
来源：http://huq.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gkz.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://ooe.yangfankeji.com

C#:   x is int or double or decimal
来源：http://vdu.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://ekr.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eim.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ydy.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://igj.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://agz.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vhi.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xjo.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://ezv.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nrh.uphjek.com

[B15] 布尔运算与取反
来源：http://kay.dianchejie.cn

Py:   a and b or not c
来源：http://wbk.uphjek.com

PHP:  $a && $b || !$c
来源：http://pzp.vehdjk.com

JS:   a && b || !c
来源：http://jup.xziqi.cn

TS:   a && b || !c
来源：http://uxt.sysykeji.top

Java: a && b || !c
来源：http://ojg.nwbrower.top

Go:   a && b || !c
来源：http://tlh.xuanzx.com

Ruby: a && b || !c
来源：http://azd.sysykeji.top

C#:   a && b || !c
来源：http://qlt.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://gyr.cashguo.top

Py:   if not data: return
来源：http://itt.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://pve.bbcook.cn

JS:   if (!data) return;
来源：http://kxr.ctjpmb.com

TS:   if (!data) return;
来源：http://oov.nwbrower.top

Java: if (data == null) return;
来源：http://eut.xylfe.cn

Go:   if data == nil { return }
来源：http://dxn.svipenyu.cn

Ruby: return if data.nil?
来源：http://gfd.gogol.net.cn

C#:   if (data == null) return;
来源：http://dek.cashguo.top

================================================================================
来源：http://omf.zdbjq.cn

C. 函数与作用域
来源：http://aix.andypj.xyz

================================================================================
来源：http://ykn.fktsv.cn

[C01] 定义函数
来源：http://rej.meibo888.top

Py:   def add(a, b): return a + b
来源：http://opu.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nih.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://xom.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tkq.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qgc.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gfd.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://mjo.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xjt.tanke756.top

[C02] 默认参数
来源：http://ezh.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://gfn.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zcu.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://dpv.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hog.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://qgw.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pdc.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://ogu.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://bvi.sjlbkw.cn

[C03] 可变参数
来源：http://ffo.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://cuw.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zel.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wod.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iko.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://csg.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wqb.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xkb.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ifw.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://bkt.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dwm.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bwx.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://awa.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qqp.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://crp.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://rda.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://mcl.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://bli.shanyushiyangtech.top

[C05] 返回多个值
来源：http://rhv.epnwcf.com

Py:   return a, b
来源：http://ihh.nanxinkj.top

PHP:  return [$a, $b];
来源：http://sea.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kfp.hysaishi.cn

TS:   return { a, b };
来源：http://apo.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nki.nanxuanxn.top

Go:   return a, b
来源：http://pnw.jinqigufen.top

Ruby: return a, b
来源：http://qfs.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://byz.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://rhc.sweek.top

Py:   square = lambda x: x * x
来源：http://fqg.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dyt.daria6918.cn

JS:   const square = x => x * x;
来源：http://vaq.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://tcn.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nfa.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://rnc.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://gfb.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://fys.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://eqb.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hct.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jlw.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ghy.chenzaomai.com

TS:   arr.map(String)
来源：http://fmy.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jme.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dut.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://lga.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://toz.gzhubu.top

[C08] 闭包
来源：http://jej.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bmr.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yad.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rqn.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mpr.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qdz.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zyd.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bbc.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uni.jinqigfzy.top

[C09] 递归
来源：http://qaz.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://npq.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bnj.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://swf.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://edm.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cnh.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ife.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kym.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cmw.guowangkeji.top

[C10] 变量作用域
来源：http://kcd.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xma.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aqm.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kow.ppjwa.cn

TS:   同 JS
来源：http://wzm.9152youxi.cn

Java: 方法内为块级作用域
来源：http://miu.aizwys.cn

Go:   花括号块级作用域
来源：http://ztq.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dkj.52xcode.cn

C#:   块级作用域
来源：http://omq.ppjwa.cn

[C11] 模块导入与导出
来源：http://ohm.zhiwuduotai.top

Py:   from module import func
来源：http://jys.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://icu.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://fuu.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lcj.xylfe.cn

Java: import java.util.List;
来源：http://ktf.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kmd.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://gci.hnxiangtu.top

C#:   using System.Text;
来源：http://gct.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://pgl.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://msg.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://xki.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://bge.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://pmu.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bfw.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://pls.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://vrd.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jky.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://cgc.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lnu.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xoo.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vue.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mps.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://nbe.jiagoushi.top

Go:   func add(a, b int) int
来源：http://nck.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jvo.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cxb.zhiwuduotai.top

[C14] 泛型函数
来源：http://dlh.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fhx.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://cdj.andypj.xyz

JS:   // 无泛型
来源：http://izl.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vkg.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vqd.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kfj.chenzaomai.com

Ruby: # 无泛型
来源：http://jjt.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fuh.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://zfp.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ang.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://ugy.yuanzhike.top


<!-- 参考信息 -->