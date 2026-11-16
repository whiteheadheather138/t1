代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gxj.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dlg.hfpthk.cn

[A24] 去除首尾空白
来源：http://agq.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cav.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aro.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://snm.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://geo.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vbm.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://zrx.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ijs.hysaishi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://epn.redwolf501.top

[A25] 字符串比较
来源：http://fbf.zdqjudy.top

Py:   s1 == s2; s1 != s2
来源：http://gpq.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://alc.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://slb.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qod.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pzg.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qxn.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ban.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ljb.cqqwz.cn

[A26] 类型转换总览
来源：http://yyp.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ksj.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://raz.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ynt.cqqwz.cn

TS:   Number() String() Boolean() x as number
来源：http://dpn.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bxj.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://suu.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://jcp.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ngz.chenlongwang.top

================================================================================
来源：http://gdf.feifeiyinyue.top

B. 流程控制
来源：http://oyc.jlsjyb.cn

================================================================================
来源：http://rqm.jyoumei.cn

[B01] 条件判断 if / else
来源：http://qjw.pycfn.com

Py:   result = "正" if x > 0 else "非正"
来源：http://kbw.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hug.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gnu.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kow.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vcu.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ili.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zbj.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rdz.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://seo.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qyy.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tnj.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyu.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqw.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pik.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://elz.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ano.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jsy.epnwcf.com

[B03] switch / match / case
来源：http://qso.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sic.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vye.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yrq.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ugv.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://skl.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bvz.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qdb.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yzu.yfazqb.com

[B04] for 计数循环
来源：http://lbe.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://qnv.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ayy.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fke.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xap.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jll.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ujk.sweek.top

Ruby: 10.times { |i| puts i }
来源：http://opk.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kfr.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://ldu.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://qst.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pjj.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ihf.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://yhi.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vlz.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://idx.nanxuanxn.top

Ruby: arr.each { |item| puts item }
来源：http://rmo.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eji.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://dvo.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yuu.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kdh.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ebr.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wmv.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wyv.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hek.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://odb.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iib.ehwqpu.com

[B07] while 循环
来源：http://wam.iojbl.cn

Py:   while i < 10: i += 1
来源：http://kso.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://xfh.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://pjl.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://qdw.yj20258.top

Java: while (i < 10) { i++; }
来源：http://ihi.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gxt.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://oxm.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://bbb.yj20258.top

[B08] do-while（至少执行一次）
来源：http://pbd.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://mtb.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lng.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://hom.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://tbj.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://pdw.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://smd.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://cqv.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://qen.shanyushiyangtech.top

[B09] break 与 continue
来源：http://yqs.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tdg.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bjm.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqd.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hnr.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzx.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bjy.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pqd.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jia.yfazqb.com

[B10] 遍历同时拿索引
来源：http://kdq.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wgl.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fke.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fqy.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rfi.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iba.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ldz.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fus.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://woi.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://edo.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://pux.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://swv.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ldl.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bhp.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ezc.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vdq.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://izn.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bvq.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://xqx.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://exx.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xil.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzg.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ioc.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rol.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xrb.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nlh.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sxn.9152youxi.cn

[B13] 判断是否为数字
来源：http://szt.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://bju.9152youxi.cn

PHP:  is_numeric($x)
来源：http://rbl.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://teu.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tkj.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://ivc.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cgi.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://lqt.daria6918.cn

C#:   x is int or double or decimal
来源：http://bhz.yj202588.top

[B14] 判断值是否在集合内
来源：http://wyj.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mmi.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yzc.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://jsl.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://lno.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kcz.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dzj.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ymo.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xvc.epnwcf.com

[B15] 布尔运算与取反
来源：http://kwo.hammf.cn

Py:   a and b or not c
来源：http://vor.iojbl.cn

PHP:  $a && $b || !$c
来源：http://vdw.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://boe.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://nxd.fengsongda.top

Java: a && b || !c
来源：http://afh.wangshuangyany.cn

Go:   a && b || !c
来源：http://ilt.dashuyun.cn

Ruby: a && b || !c
来源：http://bjj.svipenyu.cn

C#:   a && b || !c
来源：http://kam.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://jez.hcnkem.com

Py:   if not data: return
来源：http://xrc.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://ejn.yuxming.cn

JS:   if (!data) return;
来源：http://skw.cheryme.top

TS:   if (!data) return;
来源：http://ocg.sysykeji.top

Java: if (data == null) return;
来源：http://zte.jinqigfzy.top

Go:   if data == nil { return }
来源：http://twc.meibo888.top

Ruby: return if data.nil?
来源：http://bld.wangdashe.top

C#:   if (data == null) return;
来源：http://cmy.hywenlv.cn

================================================================================
来源：http://tjo.chenlongwang.top

C. 函数与作用域
来源：http://oqo.ywan-chungtsiang.top

================================================================================
来源：http://hvp.tarul.cn

[C01] 定义函数
来源：http://ajr.shanyushiyangtech.top

Py:   def add(a, b): return a + b
来源：http://vix.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iiu.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://drn.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cpp.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wbs.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://pxh.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://oyu.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ovz.tianlin.xyz

[C02] 默认参数
来源：http://fje.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://baq.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://csh.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://kks.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oeb.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://nop.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ycj.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://ycc.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://nck.gaohongyu789.top

[C03] 可变参数
来源：http://gin.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://rph.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gfb.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xld.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://owa.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ifu.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qnx.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://ray.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lwg.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://kbd.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://awl.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bbt.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tpw.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hzg.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://tdp.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://mqw.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://nos.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://huc.ybcxt.top

[C05] 返回多个值
来源：http://qwz.ydjk.org.cn

Py:   return a, b
来源：http://lyr.daxiang520.top

PHP:  return [$a, $b];
来源：http://veg.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hic.yangfankeji.com

TS:   return { a, b };
来源：http://wsg.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mqi.zhaomingkeji.xyz

Go:   return a, b
来源：http://qwd.yongpay.top

Ruby: return a, b
来源：http://ahf.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://zoi.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://axl.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://dtq.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://knc.jqgfzy.top

JS:   const square = x => x * x;
来源：http://zjw.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://zah.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://deg.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://emi.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://qap.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dye.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://wcp.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jok.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://zqb.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zdf.gaohongyu789.top

TS:   arr.map(String)
来源：http://ojo.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sud.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://erq.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://aze.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://odj.pengpengdd.cyou

[C08] 闭包
来源：http://czm.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pej.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cer.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lea.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nis.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dxo.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fmu.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qww.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aoh.316326.xyz

[C09] 递归
来源：http://ouf.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xov.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wvf.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sci.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wzl.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uem.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oms.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iox.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yeh.guowangkeji.top

[C10] 变量作用域
来源：http://gnw.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zhm.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://czy.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uec.9152youxi.cn

TS:   同 JS
来源：http://vmw.zdqjudy.top

Java: 方法内为块级作用域
来源：http://ukd.bjfxy.top

Go:   花括号块级作用域
来源：http://yyh.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ghm.sysykeji.top

C#:   块级作用域
来源：http://gtu.c1oappe.top

[C11] 模块导入与导出
来源：http://zjh.hfpthk.cn

Py:   from module import func
来源：http://leo.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hjc.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uiv.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tzo.chenjidiqi.icu

Java: import java.util.List;
来源：http://xda.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iiv.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://auk.yongpay.top

C#:   using System.Text;
来源：http://nds.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://yqq.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://qxi.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://nur.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://ret.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://yll.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://odh.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://baa.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://whn.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xmd.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://zdx.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rsp.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uvj.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://emk.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kgw.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://rzf.aizwys.cn

Go:   func add(a, b int) int
来源：http://sxa.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gyc.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://miz.pycfn.com

[C14] 泛型函数
来源：http://zaz.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mvx.hesvh.cn

PHP:  // 无泛型
来源：http://urv.yj202588.top

JS:   // 无泛型
来源：http://lkr.yj202588.top


<!-- 参考信息 -->