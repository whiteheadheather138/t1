代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://loy.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vsu.jinqigfzy.top

[A24] 去除首尾空白
来源：http://zke.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://trp.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://saa.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lpo.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hkf.cheryme.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rbl.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://eza.52xcode.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pjo.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cyr.cqqwz.cn

[A25] 字符串比较
来源：http://bsw.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://fgu.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bor.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cbs.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ygr.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sro.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zzj.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ron.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rrl.tianlin.xyz

[A26] 类型转换总览
来源：http://zef.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dof.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fra.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fmq.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://jsd.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://whx.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qbz.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dbu.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xxy.hcnkem.com

================================================================================
来源：http://lag.shuidangran.top

B. 流程控制
来源：http://hqm.cqqwz.cn

================================================================================
来源：http://rzj.tian-w.cn

[B01] 条件判断 if / else
来源：http://zxy.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xmj.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://suq.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hmj.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fvu.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zaj.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://odn.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fsk.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hbf.52xcode.cn

[B02] 多分支 else if / elif
来源：http://bxi.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cgw.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pjs.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzw.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzq.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exh.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fwm.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://odr.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihv.zdbjq.cn

[B03] switch / match / case
来源：http://gvl.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://urf.hysaishi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://swd.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://znw.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mtp.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dgt.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://czk.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mbq.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://grz.xuanzx.com

[B04] for 计数循环
来源：http://fph.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://mfo.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wro.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjl.vehdjk.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uhb.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tjb.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dze.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://zwv.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sgy.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://zey.shuidangran.top

Py:   for item in arr: print(item)
来源：http://arv.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://njg.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yqj.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vpa.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://ren.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ijj.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://bzt.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kty.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://xjm.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xjb.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qxz.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://myu.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lcy.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yty.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rsr.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ovf.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qzu.jqgufenzy.top

[B07] while 循环
来源：http://cvt.pycfn.com

Py:   while i < 10: i += 1
来源：http://bte.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://wbi.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://owc.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://zln.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://oqm.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tlf.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://njs.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://vkm.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://bva.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://vwf.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fbb.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://fif.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://lef.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://tkh.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://wth.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lsw.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://nvf.vehdjk.com

[B09] break 与 continue
来源：http://wuc.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pom.zhaomingkeji.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ghx.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxd.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcp.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghl.yj202588.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://efh.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lpn.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dxn.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://btr.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dqe.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tcb.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qvg.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ama.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mpl.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qbp.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rhj.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zix.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://zpg.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://zqe.iojbl.cn

PHP:  range(0, 10, 2);
来源：http://gjl.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://chb.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://byz.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rnl.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xai.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://stb.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://heu.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://wjt.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tnt.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rzr.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvu.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gyd.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://amx.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://owv.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uzq.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bly.xziqi.cn

[B13] 判断是否为数字
来源：http://llq.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://kgz.cdnleiting.top

PHP:  is_numeric($x)
来源：http://sno.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vgs.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rxz.uphjek.com

Java: x instanceof Number
来源：http://mqn.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wwt.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://awb.daria6918.cn

C#:   x is int or double or decimal
来源：http://agu.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://cnf.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kqz.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kkv.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://nkt.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://kna.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://kbi.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ten.xylfe.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sgt.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zwj.smart0.xyz

[B15] 布尔运算与取反
来源：http://nlo.hammf.cn

Py:   a and b or not c
来源：http://eet.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://uqi.pengpengdd.cyou

JS:   a && b || !c
来源：http://umz.nwbrower.top

TS:   a && b || !c
来源：http://orw.kuanghao11.cn

Java: a && b || !c
来源：http://ruq.0kj1m.cn

Go:   a && b || !c
来源：http://hwi.yj20258888.top

Ruby: a && b || !c
来源：http://uqh.wangdashe.top

C#:   a && b || !c
来源：http://wyf.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gcy.hammf.cn

Py:   if not data: return
来源：http://byz.meibo888.top

PHP:  if (!$data) { return; }
来源：http://zwb.dashuyun.cn

JS:   if (!data) return;
来源：http://opj.aizwys.cn

TS:   if (!data) return;
来源：http://nuf.jlsjyb.cn

Java: if (data == null) return;
来源：http://hvz.yanxiufei.cn

Go:   if data == nil { return }
来源：http://fha.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://pqr.jlsjyb.cn

C#:   if (data == null) return;
来源：http://jkm.zhengqikj.top

================================================================================
来源：http://lch.jinqigufen.top

C. 函数与作用域
来源：http://syi.jlsjyb.cn

================================================================================
来源：http://yvq.wangshuangyany.cn

[C01] 定义函数
来源：http://mhv.birdmap.top

Py:   def add(a, b): return a + b
来源：http://jox.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wvm.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://ixh.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkn.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gkx.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eva.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://bjo.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jhj.shangyingyoupin.top

[C02] 默认参数
来源：http://kzx.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://wbx.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ctn.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://lvs.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://evo.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://sbd.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bxe.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://goe.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://szs.redwolf501.top

[C03] 可变参数
来源：http://qxr.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://mcd.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vrf.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://brd.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://upf.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://otj.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uuf.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bhl.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wwv.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://dlq.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://haj.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wzw.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jns.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mli.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://ytv.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://iax.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://ptz.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://rdy.wangshuangyany.cn

[C05] 返回多个值
来源：http://adh.zhiwuduotai.top

Py:   return a, b
来源：http://bul.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://ydg.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rww.yj202588.top

TS:   return { a, b };
来源：http://src.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://urz.shzxlz.cn

Go:   return a, b
来源：http://plg.pycfn.com

Ruby: return a, b
来源：http://mnd.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://krv.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://zkp.yonumen.top

Py:   square = lambda x: x * x
来源：http://kks.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://acb.ctjpmb.com

JS:   const square = x => x * x;
来源：http://ltp.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://atd.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gfz.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://qmr.yongpay.top

Ruby: square = ->(x) { x * x }
来源：http://evo.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ffs.ivvv.top

[C07] 把函数作为参数传入
来源：http://avm.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://daf.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jmk.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xoe.fzhhl.top

TS:   arr.map(String)
来源：http://pgv.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uma.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pja.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://chs.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oyc.dashuyun.cn

[C08] 闭包
来源：http://ejb.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gwl.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wmk.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zme.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://scg.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://izs.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cka.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pqw.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pec.jinyuanbaomall.cn

[C09] 递归
来源：http://irt.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fez.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vmp.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jmp.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jma.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iwb.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sta.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rdk.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uyo.bbcook.cn

[C10] 变量作用域
来源：http://bps.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hnl.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mkd.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://thj.zhongyouzk.top

TS:   同 JS
来源：http://lgd.tian-w.cn

Java: 方法内为块级作用域
来源：http://uyt.fehbvm.com

Go:   花括号块级作用域
来源：http://pyh.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rld.smart0.xyz

C#:   块级作用域
来源：http://umo.dianchejie.cn

[C11] 模块导入与导出
来源：http://gjz.yfazqb.com

Py:   from module import func
来源：http://iwv.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://aas.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://agu.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hyi.shanyushiyangtech.top

Java: import java.util.List;
来源：http://nos.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://old.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://xqb.pengpengdd.cyou

C#:   using System.Text;
来源：http://uvl.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://bdk.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://pmi.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://tmp.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://dsw.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://nzr.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ldu.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://kwc.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://ykg.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://imw.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://err.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nkh.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jby.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uxe.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gor.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://xxa.yangfankeji.com

Go:   func add(a, b int) int
来源：http://esj.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://slr.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://flp.daria6918.cn

[C14] 泛型函数
来源：http://vun.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://drx.sxryk.cn

PHP:  // 无泛型
来源：http://oky.hammf.cn

JS:   // 无泛型
来源：http://mfo.sufxvd.cn


<!-- 参考信息 -->