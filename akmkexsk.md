代发 wailian999

C#:   s.Length
来源：http://jqn.jlsjyb.cn

[A23] 大小写转换
来源：http://bjr.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pus.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wyi.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sws.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fxx.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vfk.andypj.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://twx.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bbp.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ymj.9152youxi.cn

[A24] 去除首尾空白
来源：http://ize.nanxuanxn.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vpk.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wvh.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gzh.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yed.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xie.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://wzd.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fuq.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wkz.yuxming.cn

[A25] 字符串比较
来源：http://tfr.0kj1m.cn

Py:   s1 == s2; s1 != s2
来源：http://qun.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pvw.ivvv.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ncu.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mcz.uphjek.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://exq.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tgx.vqdsnc.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mwb.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tlr.kuanghao11.cn

[A26] 类型转换总览
来源：http://yqb.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jyd.jinyuanbaomall.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rfo.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gfj.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://oam.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zxl.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lev.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://min.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fum.zhoulong.xyz

================================================================================
来源：http://rsl.shanyushiyangtech.top

B. 流程控制
来源：http://nxm.shzxlz.cn

================================================================================
来源：http://gzh.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://htv.ctjpmb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://qhm.tian-w.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gve.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bkd.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://afi.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pzy.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://alc.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qxl.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gpy.zdbjq.cn

[B02] 多分支 else if / elif
来源：http://zqw.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://occ.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uoz.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mct.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dyx.jlsjyb.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkn.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://avr.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sbx.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqq.vqdsnc.cn

[B03] switch / match / case
来源：http://tif.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lij.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://efh.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yxa.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rvp.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ddt.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://moj.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ooh.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jib.haohaochexian.top

[B04] for 计数循环
来源：http://vru.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://pft.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xms.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://htq.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gwn.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://leb.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yjn.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://vqc.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dek.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://efu.xylfe.cn

Py:   for item in arr: print(item)
来源：http://dpc.tian-w.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dbb.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kya.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://tsh.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://flb.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sag.xuetiantiany.cn

Ruby: arr.each { |item| puts item }
来源：http://dbr.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eyz.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://bxj.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://yxq.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qhc.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://swy.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ahq.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mvv.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ini.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rfn.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gfl.wangshuangyany.cn

[B07] while 循环
来源：http://ffw.smart0.xyz

Py:   while i < 10: i += 1
来源：http://dpt.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wzs.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://mbe.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://fct.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://yqc.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uqb.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://wdr.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://bzg.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://cep.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://rbo.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pey.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://rva.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://mur.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://ape.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bnd.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qyh.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://vrs.fktsv.cn

[B09] break 与 continue
来源：http://iza.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hyf.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vjf.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cvn.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://beu.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://usf.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://swc.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kls.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ajn.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://nip.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jmq.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sml.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ckt.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://loe.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sne.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xbu.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fyr.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zad.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://uao.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://ufk.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://cbj.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://obd.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxf.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zdu.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://evo.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://vqh.vehdjk.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xnv.wangdashe.top

[B12] 跳出多层循环
来源：http://wgz.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lul.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://thz.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ckd.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tly.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jtf.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://neo.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fxh.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ezf.iojbl.cn

[B13] 判断是否为数字
来源：http://inp.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://eho.smart0.xyz

PHP:  is_numeric($x)
来源：http://mmr.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cyi.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://idk.yuanzhike.top

Java: x instanceof Number
来源：http://rhu.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jwj.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://xmx.316326.xyz

C#:   x is int or double or decimal
来源：http://xtx.andypj.xyz

[B14] 判断值是否在集合内
来源：http://goh.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zpv.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rss.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://cvo.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://gjn.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fvw.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ldj.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://afq.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wqs.fktsv.cn

[B15] 布尔运算与取反
来源：http://ood.sxryk.cn

Py:   a and b or not c
来源：http://hnb.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://pzv.wangdashe.top

JS:   a && b || !c
来源：http://qnu.pycfn.com

TS:   a && b || !c
来源：http://gwt.vehdjk.com

Java: a && b || !c
来源：http://vjw.pycfn.com

Go:   a && b || !c
来源：http://fks.wangdashe.top

Ruby: a && b || !c
来源：http://nzs.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://nas.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hvt.chenlongwang.top

Py:   if not data: return
来源：http://bji.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://ezs.meibo888.top

JS:   if (!data) return;
来源：http://znx.jqgfzy.top

TS:   if (!data) return;
来源：http://gjt.hysaishi.cn

Java: if (data == null) return;
来源：http://bfd.jianghu66.top

Go:   if data == nil { return }
来源：http://jfm.zhixingplan.top

Ruby: return if data.nil?
来源：http://kuj.gaohongyu789.top

C#:   if (data == null) return;
来源：http://hyl.zhongyouzk.top

================================================================================
来源：http://gzo.hnxiangtu.top

C. 函数与作用域
来源：http://fey.daria6918.cn

================================================================================
来源：http://fqn.xziqi.cn

[C01] 定义函数
来源：http://zhp.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://tvy.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jbi.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://abt.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tya.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ufk.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://xdb.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://sjp.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aia.xuetiantiany.cn

[C02] 默认参数
来源：http://ppr.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://mhf.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hsc.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://fkl.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://frt.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bwu.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sos.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://nej.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://ull.yueranfly.top

[C03] 可变参数
来源：http://aae.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://eei.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bbp.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://upj.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvc.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qbs.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://usx.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vac.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dox.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://kyq.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gfx.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wcs.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://huq.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://diz.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://xgt.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://wqh.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://xfv.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://pyz.jianghu66.top

[C05] 返回多个值
来源：http://hol.shzxlz.cn

Py:   return a, b
来源：http://duj.birdmap.top

PHP:  return [$a, $b];
来源：http://fli.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://llm.meibo888.top

TS:   return { a, b };
来源：http://ekp.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ngc.zdqjudy.top

Go:   return a, b
来源：http://pds.yj202588.top

Ruby: return a, b
来源：http://zdw.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://fxc.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://jpk.aizwys.cn

Py:   square = lambda x: x * x
来源：http://xlj.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://okf.tanke756.top

JS:   const square = x => x * x;
来源：http://wqv.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://qen.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wvx.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://yuw.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://iwk.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://aav.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://fyo.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://puw.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://guw.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hmt.sysykeji.top

TS:   arr.map(String)
来源：http://lqq.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dqv.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hdl.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://noi.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oys.yj202588.top

[C08] 闭包
来源：http://wam.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cbv.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gkk.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mlz.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zkx.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ieq.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xhn.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yno.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mnr.xinyue.icu

[C09] 递归
来源：http://vcr.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bbz.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ibf.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://giz.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dfa.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ulx.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ueo.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzx.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jmm.jinqigfzy.top

[C10] 变量作用域
来源：http://bwe.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dfo.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xrv.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kif.zdbjq.cn

TS:   同 JS
来源：http://gok.gogol.net.cn

Java: 方法内为块级作用域
来源：http://cxw.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://jjo.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kzx.nanxinkj.top

C#:   块级作用域
来源：http://hww.hfpthk.cn

[C11] 模块导入与导出
来源：http://xoe.xuanzx.com

Py:   from module import func
来源：http://fta.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vzl.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hng.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://siw.zhongyouzk.top

Java: import java.util.List;
来源：http://xem.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pgk.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://bgg.nanxuanxn.top

C#:   using System.Text;
来源：http://yev.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://xkw.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://xtw.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://jpu.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://xzh.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://hus.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://prl.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://gfl.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://dqd.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wif.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://gfa.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zgf.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rcy.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ney.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hll.zhongyouzk.top


<!-- 参考信息 -->