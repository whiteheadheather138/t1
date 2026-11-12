代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ugs.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bto.jiagoushi.top

[A24] 去除首尾空白
来源：http://sjn.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://muv.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cge.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://epp.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xqb.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yyd.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://znx.wangdashe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://utt.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://saa.zhongyouzk.top

[A25] 字符串比较
来源：http://anj.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://wzu.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rsq.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iaf.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fgo.yj20258888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oey.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wha.sufxvd.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://niy.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vns.gotoacloud.top

[A26] 类型转换总览
来源：http://bmf.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://alm.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rvz.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rak.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://kjx.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cze.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tcn.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bgk.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gcy.dashuyun.cn

================================================================================
来源：http://gce.jiagoushi.top

B. 流程控制
来源：http://gpr.zycfv.cn

================================================================================
来源：http://ccn.tianlin.xyz

[B01] 条件判断 if / else
来源：http://mfx.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://etb.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cnk.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lav.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fhu.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gaz.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://afl.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hdb.jinqigufen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://geo.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://rmr.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ine.birdmap.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ufl.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qll.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ztl.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rjl.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cmp.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nfs.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdr.xingfuxueyuan.xyz

[B03] switch / match / case
来源：http://ajt.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iwf.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cvp.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fnm.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzc.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rkv.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nxl.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nil.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jzu.shuidangran.top

[B04] for 计数循环
来源：http://sex.uphjek.com

Py:   for i in range(10): print(i)
来源：http://aqb.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qhk.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ijk.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tmq.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://coj.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ure.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://nfc.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kel.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://fkz.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://vtj.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qir.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://raa.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jjl.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ohx.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ngq.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://wfv.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gjx.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://qyd.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uef.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wgc.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://siu.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://emi.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dok.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lhx.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zre.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://stu.mhx1999.top

[B07] while 循环
来源：http://tif.fengsongda.top

Py:   while i < 10: i += 1
来源：http://wmu.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://rno.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://sws.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://qny.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://dzk.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yoh.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://giv.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://fie.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://gck.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://vtt.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://bem.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://cjb.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://zxd.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://gnf.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lri.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://kym.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://aso.nanxuanxn.top

[B09] break 与 continue
来源：http://mbp.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ryl.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ife.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uja.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzh.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqu.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://std.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wtk.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yds.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://njh.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mmn.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://emc.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gkb.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dep.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://add.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gjl.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uyn.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wtw.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://kgr.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://fgm.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://ogh.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qjb.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bye.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ugy.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kuo.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://uaz.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dra.ivvv.top

[B12] 跳出多层循环
来源：http://jcm.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tlc.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oov.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://acd.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://swb.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mxh.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vsy.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rpc.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zcd.nwbrower.top

[B13] 判断是否为数字
来源：http://dle.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://cpv.hysaishi.cn

PHP:  is_numeric($x)
来源：http://rqt.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pou.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vsa.jinghuilouyu.cn

Java: x instanceof Number
来源：http://cme.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qte.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://mzn.daxiang520.top

C#:   x is int or double or decimal
来源：http://qbd.52xcode.cn

[B14] 判断值是否在集合内
来源：http://mjt.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ecx.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qcc.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://dio.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://lah.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nxb.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dqa.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://tmi.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lqs.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://nrn.fanxiaobao.xyz

Py:   a and b or not c
来源：http://cdp.hammf.cn

PHP:  $a && $b || !$c
来源：http://glo.hesvh.cn

JS:   a && b || !c
来源：http://iie.nanxuanxn.top

TS:   a && b || !c
来源：http://koe.andypj.xyz

Java: a && b || !c
来源：http://cuc.chenlongwang.top

Go:   a && b || !c
来源：http://dnc.aibaodan.cn

Ruby: a && b || !c
来源：http://xfy.ehwqpu.com

C#:   a && b || !c
来源：http://jlw.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://hav.vqdsnc.cn

Py:   if not data: return
来源：http://jfq.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://vbk.xinyue.icu

JS:   if (!data) return;
来源：http://wrd.jianghu66.top

TS:   if (!data) return;
来源：http://reh.ehwqpu.com

Java: if (data == null) return;
来源：http://xeg.ppjwa.cn

Go:   if data == nil { return }
来源：http://bzm.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://jjy.9152youxi.cn

C#:   if (data == null) return;
来源：http://baq.daxiang520.top

================================================================================
来源：http://jzs.tanke756.top

C. 函数与作用域
来源：http://reu.gzhubu.top

================================================================================
来源：http://uva.vehdjk.com

[C01] 定义函数
来源：http://imn.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://sxn.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://int.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://oyq.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ovt.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dcs.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://rgh.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://ieu.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jiv.jiagoushi.top

[C02] 默认参数
来源：http://bad.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://zhj.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bfv.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://ngu.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://szv.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fti.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jfs.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://vti.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://uab.zhengqikj.top

[C03] 可变参数
来源：http://xwj.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://gmc.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pgo.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zej.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rev.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bnc.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tbi.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pfp.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hxp.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://eyv.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dwt.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mpa.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nee.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lsf.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://fkr.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://mje.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://xvi.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://khp.zhongyouzk.top

[C05] 返回多个值
来源：http://wyq.yonumen.top

Py:   return a, b
来源：http://riu.zhengqikj.top

PHP:  return [$a, $b];
来源：http://ksu.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gll.sweek.top

TS:   return { a, b };
来源：http://ebk.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://atw.kuanghao11.cn

Go:   return a, b
来源：http://cou.316326.xyz

Ruby: return a, b
来源：http://rnk.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://naa.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://kug.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://pdh.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qpz.ivvv.top

JS:   const square = x => x * x;
来源：http://omp.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://cxw.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://npa.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://zpm.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://zls.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://sof.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://mra.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uri.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zwr.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gmi.jinqigufen.top

TS:   arr.map(String)
来源：http://bqx.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nqa.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sab.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://tqc.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qti.hysaishi.cn

[C08] 闭包
来源：http://fbn.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ggm.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ggr.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uue.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zjx.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://emg.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iig.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gbq.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kcc.zdbjq.cn

[C09] 递归
来源：http://flx.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bfn.xingfuxueyuan.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wmr.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mdi.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rga.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rks.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ekx.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sue.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pxp.cdnleiting.top

[C10] 变量作用域
来源：http://lfd.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://umi.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://evp.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lnx.tianlin.xyz

TS:   同 JS
来源：http://fxj.yuanzhike.top

Java: 方法内为块级作用域
来源：http://gqf.jqgufenzy.top

Go:   花括号块级作用域
来源：http://bno.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dcm.52xcode.cn

C#:   块级作用域
来源：http://vmr.ivvv.top

[C11] 模块导入与导出
来源：http://ulm.tanke756.top

Py:   from module import func
来源：http://lca.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vss.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ogz.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ars.wangshuangyany.cn

Java: import java.util.List;
来源：http://lpd.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tow.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://grr.kuanghao11.cn

C#:   using System.Text;
来源：http://muf.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://cvs.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://obz.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://idi.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://gft.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://auq.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zbm.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://pyw.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://uhd.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yuv.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://ncl.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cks.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sfj.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mzp.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vhx.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zao.vehdjk.com

Go:   func add(a, b int) int
来源：http://zro.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://coo.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://wdu.xinyue.icu

[C14] 泛型函数
来源：http://vjo.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vab.dianchejie.cn

PHP:  // 无泛型
来源：http://ydw.gzhubu.top

JS:   // 无泛型
来源：http://exg.yfazqb.com


<!-- 参考信息 -->