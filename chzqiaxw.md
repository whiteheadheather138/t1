代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://psm.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dxf.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://rtp.iojbl.cn

TS:   (3.14159).toFixed(2)
来源：http://wot.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://wxn.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gfo.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://ctn.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://ldl.daxiang520.top

[A22] 获取字符串长度
来源：http://ciz.fzhhl.top

Py:   len(s)
来源：http://shm.smart0.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wuw.guowangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ejs.gaohongyu789.top

TS:   s.length
来源：http://lcw.0kj1m.cn

Java: s.length()
来源：http://pef.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://exr.tianlin.xyz

Ruby: s.length
来源：http://alj.pengpengdd.cyou

C#:   s.Length
来源：http://qyf.guowangkeji.top

[A23] 大小写转换
来源：http://mtl.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gax.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eir.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cho.ctjpmb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://luu.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jfx.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hdj.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yra.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kfy.sysykeji.top

[A24] 去除首尾空白
来源：http://ubk.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dmu.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qgr.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rrv.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sks.hywenlv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lzx.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://lgg.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gyk.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bgu.tarul.cn

[A25] 字符串比较
来源：http://gtc.bjfxy.top

Py:   s1 == s2; s1 != s2
来源：http://khs.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xpd.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qiy.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mvq.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qew.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://elq.sweek.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gea.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ofg.pycfn.com

[A26] 类型转换总览
来源：http://lsc.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://svg.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ydu.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qfh.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://sta.hywenlv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wni.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mfu.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xyd.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aqx.xuanzx.com

================================================================================
来源：http://drf.nwbrower.top

B. 流程控制
来源：http://gqe.pengpengdd.cyou

================================================================================
来源：http://okm.yuanzhike.top

[B01] 条件判断 if / else
来源：http://kdl.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kbf.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hly.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wmf.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ohh.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fno.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cms.iojbl.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://owa.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mhh.yj20258.top

[B02] 多分支 else if / elif
来源：http://fld.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xps.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tql.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hks.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggb.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hfn.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://has.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://msy.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijo.yonumen.top

[B03] switch / match / case
来源：http://xdg.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://syz.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gmi.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pdj.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wla.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wlx.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bts.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hye.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ilj.havefunace.top

[B04] for 计数循环
来源：http://xnl.xingfuxueyuan.xyz

Py:   for i in range(10): print(i)
来源：http://rgc.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qox.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kgh.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gvu.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yke.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lzu.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://mfn.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ala.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://vdr.yonumen.top

Py:   for item in arr: print(item)
来源：http://zex.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://agg.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://aig.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vkz.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gud.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://czp.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://hyb.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mds.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://hpu.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fat.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cmb.yanxiufei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://off.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ver.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://elw.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pjg.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sou.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wzk.andypj.xyz

[B07] while 循环
来源：http://eyo.vehdjk.com

Py:   while i < 10: i += 1
来源：http://kky.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://box.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://iet.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://byj.yj202588.top

Java: while (i < 10) { i++; }
来源：http://rok.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://csz.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://hbj.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://lwf.yongpay.top

[B08] do-while（至少执行一次）
来源：http://zcq.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://lnh.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://huw.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://uqv.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://xbj.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://cko.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mcc.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://yob.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://qwz.sufxvd.cn

[B09] break 与 continue
来源：http://tdo.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lur.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pen.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tly.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npz.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hff.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cwj.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://olw.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ech.sxryk.cn

[B10] 遍历同时拿索引
来源：http://gsk.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://awv.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://txg.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://viw.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oqk.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mth.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://suj.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://akj.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uzl.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://ugf.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://yer.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://rfe.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lls.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hys.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rvh.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mkk.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://dfz.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ytg.xinyue.icu

[B12] 跳出多层循环
来源：http://dlq.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qxl.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ton.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xdd.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://inm.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://air.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wvs.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qjx.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xdj.meibo888.top

[B13] 判断是否为数字
来源：http://fzl.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://wjj.hysaishi.cn

PHP:  is_numeric($x)
来源：http://jir.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ube.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ouc.uphjek.com

Java: x instanceof Number
来源：http://bvk.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qhu.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://rxc.fehbvm.com

C#:   x is int or double or decimal
来源：http://lwx.ivvv.top

[B14] 判断值是否在集合内
来源：http://jla.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eoh.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://edx.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://ljd.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://kpl.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fnf.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cwk.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://who.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://grc.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://ogl.meibo888.top

Py:   a and b or not c
来源：http://tfz.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://pfl.shzxlz.cn

JS:   a && b || !c
来源：http://fzx.hesvh.cn

TS:   a && b || !c
来源：http://vae.tian-w.cn

Java: a && b || !c
来源：http://xms.daria6918.cn

Go:   a && b || !c
来源：http://mdu.zycfv.cn

Ruby: a && b || !c
来源：http://ucn.jiagoushi.top

C#:   a && b || !c
来源：http://nxy.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gir.sweek.top

Py:   if not data: return
来源：http://sga.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://enw.xuanzx.com

JS:   if (!data) return;
来源：http://loy.hammf.cn

TS:   if (!data) return;
来源：http://wfo.vehdjk.com

Java: if (data == null) return;
来源：http://esc.tian-w.cn

Go:   if data == nil { return }
来源：http://euh.tianlin.xyz

Ruby: return if data.nil?
来源：http://jxx.vehdjk.com

C#:   if (data == null) return;
来源：http://wpr.jlsjyb.cn

================================================================================
来源：http://yag.cucudq.cn

C. 函数与作用域
来源：http://cef.cheryme.top

================================================================================
来源：http://hen.yj202588.top

[C01] 定义函数
来源：http://wcu.yj20258.top

Py:   def add(a, b): return a + b
来源：http://ngt.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cgg.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://dik.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://syn.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://sde.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pbs.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://qhp.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzl.sysykeji.top

[C02] 默认参数
来源：http://kvy.uphjek.com

Py:   def greet(name="World"): return name
来源：http://unk.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://mwm.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://uio.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hmi.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mbo.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pcv.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://icb.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://hfj.sxryk.cn

[C03] 可变参数
来源：http://yhv.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://vys.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xqf.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xvr.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cnq.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://isj.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ibe.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://pwn.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uaj.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://zxf.hysaishi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zev.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://irt.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pxp.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ixb.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://bhw.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://kao.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://fbk.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://rim.haohaochexian.top

[C05] 返回多个值
来源：http://lma.snrcjt.cn

Py:   return a, b
来源：http://emw.ppjwa.cn

PHP:  return [$a, $b];
来源：http://frs.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uro.bbcook.cn

TS:   return { a, b };
来源：http://ysw.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tpj.mhx1999.top

Go:   return a, b
来源：http://iim.vqdsnc.cn

Ruby: return a, b
来源：http://yjp.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://zwv.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://xdp.jianghu66.top

Py:   square = lambda x: x * x
来源：http://env.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ttw.ydzc1.top

JS:   const square = x => x * x;
来源：http://mhk.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://mhk.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cqq.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tju.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://aon.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bjj.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://vsj.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://onh.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kfg.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zqg.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://stk.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dqq.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tzb.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://hgo.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://pxc.gotoacloud.top

[C08] 闭包
来源：http://lag.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://apz.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yxl.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jfx.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rah.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hne.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fyb.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iqb.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jmc.shanyushiyangtech.top

[C09] 递归
来源：http://xta.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://njb.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://amu.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wjk.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gru.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ini.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jdw.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yeo.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iuh.hywenlv.cn

[C10] 变量作用域
来源：http://dkn.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dlr.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fjv.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ugj.zhixingplan.top

TS:   同 JS
来源：http://lvz.snrcjt.cn

Java: 方法内为块级作用域
来源：http://pgv.guannengcc.top

Go:   花括号块级作用域
来源：http://uds.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hde.jiagoushi.top

C#:   块级作用域
来源：http://tbi.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://rws.dianchejie.cn

Py:   from module import func
来源：http://dtv.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://roq.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bcf.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://afb.xylfe.cn

Java: import java.util.List;
来源：http://bid.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eue.jinqigufen.top


<!-- 参考信息 -->