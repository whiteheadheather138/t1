代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hwf.birdmap.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iud.shuidangran.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://alt.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kos.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ett.yj20258888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dgk.uphjek.com

[A24] 去除首尾空白
来源：http://blf.gaohongyu789.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oul.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ncx.quarkkingdee.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ihg.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ssj.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fki.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://yom.hcnkem.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zxc.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cdh.daria6918.cn

[A25] 字符串比较
来源：http://jwq.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://wmu.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hqm.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oth.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xzd.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rfr.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yir.meibo888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://biw.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kso.fktsv.cn

[A26] 类型转换总览
来源：http://xso.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ywq.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://htv.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aeu.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://sup.cashguo.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jvi.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kqf.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bol.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yvm.quarkkingdee.top

================================================================================
来源：http://opt.dianchejie.cn

B. 流程控制
来源：http://fjx.aibaodan.cn

================================================================================
来源：http://fgb.yj20258888.top

[B01] 条件判断 if / else
来源：http://xlw.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wil.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kjn.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://czx.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eee.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tvm.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xqm.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ijf.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yau.shuidangran.top

[B02] 多分支 else if / elif
来源：http://isy.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vsm.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jfm.gotoacloud.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpf.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqi.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zyt.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dxu.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vrf.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyd.fengsongda.top

[B03] switch / match / case
来源：http://kvs.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://alq.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dpa.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ugj.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ixa.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qac.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sjs.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kop.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xzh.gotoacloud.top

[B04] for 计数循环
来源：http://shn.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://ueq.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fxm.yanxiufei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ttb.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://acd.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lhz.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yse.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://zvf.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://drn.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://yih.pycfn.com

Py:   for item in arr: print(item)
来源：http://eyz.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://brx.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://aex.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://frs.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://qmi.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qgt.pycfn.com

Ruby: arr.each { |item| puts item }
来源：http://eqr.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rbd.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://vjb.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://hds.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zqj.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fbx.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bol.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqr.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pzn.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uix.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vci.quarkkingdee.top

[B07] while 循环
来源：http://zdl.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://omi.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://fyj.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://awn.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://stx.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://lmc.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ngi.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://vhf.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://ueb.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://nbn.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://lpp.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xao.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://oek.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://pvy.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://igz.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uiw.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://onr.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://gvw.cdnleiting.top

[B09] break 与 continue
来源：http://gtv.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lxt.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gil.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqe.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://erg.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://alm.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xce.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ujp.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rbi.yongpay.top

[B10] 遍历同时拿索引
来源：http://ytj.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nkm.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dxi.meibo888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wwk.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://khu.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iuo.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wzo.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rqq.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yze.dashuyun.cn

[B11] 生成数字序列 / 区间
来源：http://fjo.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://qxt.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://fkf.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jjv.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iwc.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cip.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://its.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://bxv.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vqf.ctjpmb.com

[B12] 跳出多层循环
来源：http://gkj.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nzk.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tkn.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://apn.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ttv.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://smk.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ndy.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xeo.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://isq.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://mky.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://dcx.birdmap.top

PHP:  is_numeric($x)
来源：http://jqs.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kib.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nni.sweek.top

Java: x instanceof Number
来源：http://kok.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qxz.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://dzc.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://vji.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://wfo.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azk.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oct.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://hxd.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://nkm.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gbm.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xuu.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://uqn.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mta.bbcook.cn

[B15] 布尔运算与取反
来源：http://rio.yuanzhike.top

Py:   a and b or not c
来源：http://eha.316326.xyz

PHP:  $a && $b || !$c
来源：http://nvx.yfazqb.com

JS:   a && b || !c
来源：http://elv.dashuyun.cn

TS:   a && b || !c
来源：http://mxg.jinghuilouyu.cn

Java: a && b || !c
来源：http://ckc.tanke756.top

Go:   a && b || !c
来源：http://lob.xuetiantiany.cn

Ruby: a && b || !c
来源：http://sji.jinghuilouyu.cn

C#:   a && b || !c
来源：http://bkf.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://wsy.dashuyun.cn

Py:   if not data: return
来源：http://ivc.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://yeu.shuidangran.top

JS:   if (!data) return;
来源：http://zff.yangfankeji.com

TS:   if (!data) return;
来源：http://dpt.snrcjt.cn

Java: if (data == null) return;
来源：http://bzn.gzhubu.top

Go:   if data == nil { return }
来源：http://qbb.tianlin.xyz

Ruby: return if data.nil?
来源：http://ody.hnqzz.top

C#:   if (data == null) return;
来源：http://yiq.haohaochexian.top

================================================================================
来源：http://hci.hfpthk.cn

C. 函数与作用域
来源：http://ppn.aizwys.cn

================================================================================
来源：http://yle.hammf.cn

[C01] 定义函数
来源：http://pou.shanyushiyangtech.top

Py:   def add(a, b): return a + b
来源：http://aeh.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfc.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://mau.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kcy.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zdy.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://vok.jianghu66.top

Ruby: def add(a, b); a + b; end
来源：http://dzb.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://krn.svipenyu.cn

[C02] 默认参数
来源：http://uri.sweek.top

Py:   def greet(name="World"): return name
来源：http://edc.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rpz.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://tjq.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://pbn.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://gwt.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qry.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://llw.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://exw.redwolf501.top

[C03] 可变参数
来源：http://gwf.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://ywb.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cnc.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hdg.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mla.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://man.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lvd.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://lnt.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://krq.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://xvf.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lbm.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aoa.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://evj.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aso.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://aot.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://bvv.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://pkh.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://uos.cdnleiting.top

[C05] 返回多个值
来源：http://dac.snrcjt.cn

Py:   return a, b
来源：http://cyf.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://msc.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qje.daxiang520.top

TS:   return { a, b };
来源：http://dsi.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qki.wangdashe.top

Go:   return a, b
来源：http://rxm.iojbl.cn

Ruby: return a, b
来源：http://rzg.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://czf.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://sjh.316326.xyz

Py:   square = lambda x: x * x
来源：http://qkm.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://smq.dianchejie.cn

JS:   const square = x => x * x;
来源：http://poi.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://zqc.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qhn.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://zta.ppjwa.cn

Ruby: square = ->(x) { x * x }
来源：http://oeu.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://wpr.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://syn.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fxr.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://lfh.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ajc.zhixingplan.top

TS:   arr.map(String)
来源：http://gvr.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ozb.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pyo.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://xyq.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mnf.hesvh.cn

[C08] 闭包
来源：http://gkm.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ikh.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cek.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vpn.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jvd.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ufk.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://geg.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cqx.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yic.316326.xyz

[C09] 递归
来源：http://nav.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kiv.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sun.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xep.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://azg.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jbm.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xxq.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wth.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lvd.ctjpmb.com

[C10] 变量作用域
来源：http://uem.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://stv.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uat.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ecv.daria6918.cn

TS:   同 JS
来源：http://ltn.zycfv.cn

Java: 方法内为块级作用域
来源：http://cnw.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://sca.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ufx.0kj1m.cn

C#:   块级作用域
来源：http://ozq.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://wmy.xuanzx.com

Py:   from module import func
来源：http://yqw.xingfuxueyuan.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://dmp.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://scd.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cby.chenzaomai.com

Java: import java.util.List;
来源：http://zpr.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qrd.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://xud.nanxuanxn.top

C#:   using System.Text;
来源：http://hba.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://pvq.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://krf.smart0.xyz

PHP:  (function () { echo "run"; })();
来源：http://hde.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://kgq.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://mgs.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fzu.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://jtc.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://wai.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bqz.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://dcq.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eex.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://its.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ggc.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lme.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vtx.cucudq.cn

Go:   func add(a, b int) int
来源：http://akv.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yel.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://duu.jlsjyb.cn


<!-- 参考信息 -->