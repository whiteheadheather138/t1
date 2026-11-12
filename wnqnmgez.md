代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xju.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ikv.yueranfly.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jjq.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qbr.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://jne.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ing.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mtv.yuanzhike.top

[A25] 字符串比较
来源：http://xoq.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://ncw.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dsa.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://euz.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://njy.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mvq.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nfw.wangdashe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pet.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mcm.jianghu66.top

[A26] 类型转换总览
来源：http://ayt.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rcj.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zqd.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://znc.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://mai.uphjek.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://adc.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kpl.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ynb.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hee.kuanghao11.cn

================================================================================
来源：http://gvd.wangdashe.top

B. 流程控制
来源：http://zln.jiagoushi.top

================================================================================
来源：http://qbi.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://pfa.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cpn.wangdashe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tir.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rdu.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gmr.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vul.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rdw.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uds.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ndp.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://jpn.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mbw.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mfj.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrt.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hry.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nye.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uxz.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aqq.hesvh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tpa.yanxiufei.cn

[B03] switch / match / case
来源：http://nvf.zycfv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ohj.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uru.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kik.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aei.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://shp.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tfw.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tbu.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fhl.ydjk.org.cn

[B04] for 计数循环
来源：http://pux.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://vfz.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uwv.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iuw.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hxz.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tpg.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bvv.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://htp.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://maj.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://cae.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://iur.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vbc.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cax.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cnu.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://isq.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hhr.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://ugc.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://weq.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://uhe.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uol.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://euf.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hpj.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsg.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ggd.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lsw.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://txb.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rbt.nanxinkj.top

[B07] while 循环
来源：http://ryd.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://lnr.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://szy.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://kcz.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://rza.daria6918.cn

Java: while (i < 10) { i++; }
来源：http://gkk.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fnd.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://rhp.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://qpv.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://xtb.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://rls.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fbv.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://wdp.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://vsd.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://gez.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://obw.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fap.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://omp.chenzaomai.com

[B09] break 与 continue
来源：http://eii.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wth.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bth.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvt.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzr.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzh.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://org.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qhx.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mie.ivvv.top

[B10] 遍历同时拿索引
来源：http://mqd.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tfj.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cgc.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wma.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qgr.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xye.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yfh.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ltc.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fgx.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://syl.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://xbt.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://sdx.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kbi.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wlo.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://frs.9152youxi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fuv.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://rzg.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bje.hywenlv.cn

[B12] 跳出多层循环
来源：http://nil.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://gmc.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ksi.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jgm.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mnw.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rsd.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kwz.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gdo.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ajp.sxryk.cn

[B13] 判断是否为数字
来源：http://uoc.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://afz.hesvh.cn

PHP:  is_numeric($x)
来源：http://ozn.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fgn.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ixa.smart0.xyz

Java: x instanceof Number
来源：http://osz.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bzh.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://kjg.iojbl.cn

C#:   x is int or double or decimal
来源：http://yzf.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://dgb.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ype.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://puc.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://qao.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://gvs.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qzk.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vem.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://smt.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://twa.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://csd.vehdjk.com

Py:   a and b or not c
来源：http://wvi.hnqzz.top

PHP:  $a && $b || !$c
来源：http://kqm.zycfv.cn

JS:   a && b || !c
来源：http://chv.vehdjk.com

TS:   a && b || !c
来源：http://rla.zdqjudy.top

Java: a && b || !c
来源：http://ufd.dianchejie.cn

Go:   a && b || !c
来源：http://kfr.yonumen.top

Ruby: a && b || !c
来源：http://mfw.yj20258.top

C#:   a && b || !c
来源：http://xll.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://qjl.cheryme.top

Py:   if not data: return
来源：http://jtx.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://vor.meibo888.top

JS:   if (!data) return;
来源：http://kgr.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://zuv.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://sph.sjlbkw.cn

Go:   if data == nil { return }
来源：http://qlr.yonumen.top

Ruby: return if data.nil?
来源：http://cdz.9152youxi.cn

C#:   if (data == null) return;
来源：http://ejs.yj202588.top

================================================================================
来源：http://dlw.yanxiufei.cn

C. 函数与作用域
来源：http://woc.redwolf501.top

================================================================================
来源：http://rob.jqgfzy.top

[C01] 定义函数
来源：http://jpn.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://exx.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hno.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://sog.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzp.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bdb.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zqd.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://mpk.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cqn.kuanghao11.cn

[C02] 默认参数
来源：http://ong.jyoumei.cn

Py:   def greet(name="World"): return name
来源：http://rpo.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dzh.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://ftk.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fui.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zgv.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rtk.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://saw.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://ftb.ehwqpu.com

[C03] 可变参数
来源：http://mab.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://vca.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fgq.xinyue.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://com.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqg.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cbn.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yre.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://jut.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://buu.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://mgs.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ubn.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dcm.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oyf.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cim.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://ufs.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://agm.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://ntv.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://hqx.yangfankeji.com

[C05] 返回多个值
来源：http://vyo.xziqi.cn

Py:   return a, b
来源：http://pvz.sufxvd.cn

PHP:  return [$a, $b];
来源：http://ljb.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ieg.feifeiyinyue.top

TS:   return { a, b };
来源：http://usx.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zhd.zdqjudy.top

Go:   return a, b
来源：http://yav.ywan-chungtsiang.top

Ruby: return a, b
来源：http://szp.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://top.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://yxf.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://udb.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oto.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://kvn.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://lbz.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lze.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://vjl.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://mpj.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ngn.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://fiw.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qve.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://jfx.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kmr.zhixingplan.top

TS:   arr.map(String)
来源：http://tej.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xkc.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wxg.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://rth.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gwz.hesvh.cn

[C08] 闭包
来源：http://viz.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pze.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rbn.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hrz.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mvi.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://egc.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ieh.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://drn.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vsq.ivvv.top

[C09] 递归
来源：http://xsq.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gpu.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ogn.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mxt.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dnm.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fnc.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uiq.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wwg.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hrk.jinqigfzy.top

[C10] 变量作用域
来源：http://hff.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://djs.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xzb.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dmu.andypj.xyz

TS:   同 JS
来源：http://jcj.ctjpmb.com

Java: 方法内为块级作用域
来源：http://xsh.ydjk.org.cn

Go:   花括号块级作用域
来源：http://tsd.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://luu.hnqzz.top

C#:   块级作用域
来源：http://tos.cqqwz.cn

[C11] 模块导入与导出
来源：http://dkd.hesvh.cn

Py:   from module import func
来源：http://zag.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jqr.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://omq.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xiu.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://vbw.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wnu.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://ntl.bjfxy.top

C#:   using System.Text;
来源：http://ikh.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://reo.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://abn.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://yhq.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://srk.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://pwb.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://glc.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zre.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://kry.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://rcs.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://kqm.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xgc.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hfj.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fdc.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sbu.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://qst.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://keq.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tvi.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mpv.mhx1999.top

[C14] 泛型函数
来源：http://ork.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mul.shangyingyoupin.top

PHP:  // 无泛型
来源：http://ffa.hongshengwenyu.top

JS:   // 无泛型
来源：http://pbs.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://squ.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ajv.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ecg.hfpthk.cn

Ruby: # 无泛型
来源：http://vbg.jqgfzy.top


<!-- 参考信息 -->