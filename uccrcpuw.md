代发 wailian999

[A22] 获取字符串长度
来源：http://szw.zhaomingkeji.xyz

Py:   len(s)
来源：http://bij.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gip.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://twq.vehdjk.com

TS:   s.length
来源：http://cmq.gogol.net.cn

Java: s.length()
来源：http://ivm.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cor.0kj1m.cn

Ruby: s.length
来源：http://ifq.bjfxy.top

C#:   s.Length
来源：http://yrx.zhixingplan.top

[A23] 大小写转换
来源：http://dvj.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wql.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mtk.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ejn.fehbvm.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kix.nanxinkj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jbj.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ccx.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zbz.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wpy.fktsv.cn

[A24] 去除首尾空白
来源：http://xuf.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dxe.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ckn.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gtv.sjlbkw.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bjv.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pad.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://omf.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://exq.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://crm.hnxiangtu.top

[A25] 字符串比较
来源：http://xmb.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://gwv.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ywb.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://urg.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gjv.bbcook.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://saw.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qsv.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rnl.jyoumei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lmu.xuetiantiany.cn

[A26] 类型转换总览
来源：http://pjf.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ovf.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fii.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pla.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://puz.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://upe.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vob.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mhy.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vpu.nanxinkj.top

================================================================================
来源：http://zrn.zhaomingkeji.xyz

B. 流程控制
来源：http://moy.jinyuanbaomall.cn

================================================================================
来源：http://tbh.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://pyd.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cpu.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jrd.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vny.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://scl.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://mmn.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fce.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jbf.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qae.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://dpg.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nmr.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://njg.fengsongda.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pat.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://saj.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wql.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bbf.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vnn.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eze.pycfn.com

[B03] switch / match / case
来源：http://zil.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rod.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rcl.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oos.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://joj.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zll.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://alq.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mgy.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xnr.316326.xyz

[B04] for 计数循环
来源：http://ico.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://psn.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rnb.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtp.yongpay.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqt.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cmr.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://edf.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://men.tian-w.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fcr.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://jbo.andypj.xyz

Py:   for item in arr: print(item)
来源：http://gdp.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zwd.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dvx.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dty.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wny.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vwl.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://rgk.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://owe.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://twp.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zaj.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lil.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rmp.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dne.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://say.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sfq.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xzo.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qdi.yueranfly.top

[B07] while 循环
来源：http://vcy.yj202588.top

Py:   while i < 10: i += 1
来源：http://viu.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://veh.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://sym.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://rzq.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://sjx.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rrs.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://xcb.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://onl.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://zgb.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://gdu.wangdashe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fyl.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://soc.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://ebj.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://uae.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tjl.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zox.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://izu.shanyushiyangtech.top

[B09] break 与 continue
来源：http://zgw.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jmk.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jtu.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhd.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iol.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://enc.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lde.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lwu.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eov.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://fov.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cta.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qlq.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tun.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mdd.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bsi.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ujn.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nej.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jng.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://psx.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://axj.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://buu.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kgv.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyk.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ykw.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wio.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://yuv.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wqc.vehdjk.com

[B12] 跳出多层循环
来源：http://xxj.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ghb.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://dja.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pbz.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vln.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cur.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bgq.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cjh.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vrx.jinqigfzy.top

[B13] 判断是否为数字
来源：http://znj.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://vsb.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://zmr.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rjh.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kvq.sxryk.cn

Java: x instanceof Number
来源：http://leq.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nsj.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://jsl.chenzaomai.com

C#:   x is int or double or decimal
来源：http://wdo.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://hrx.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://giz.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://twt.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://alc.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://umo.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://joq.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ilg.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lue.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jfy.daxiang520.top

[B15] 布尔运算与取反
来源：http://rbv.hammf.cn

Py:   a and b or not c
来源：http://qcd.zycfv.cn

PHP:  $a && $b || !$c
来源：http://jse.sysykeji.top

JS:   a && b || !c
来源：http://jcs.hongshengwenyu.top

TS:   a && b || !c
来源：http://lvf.guowangkeji.top

Java: a && b || !c
来源：http://dgk.9152youxi.cn

Go:   a && b || !c
来源：http://crb.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://min.jiagoushi.top

C#:   a && b || !c
来源：http://mgu.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://bgq.daria6918.cn

Py:   if not data: return
来源：http://mzc.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://uwz.jlsjyb.cn

JS:   if (!data) return;
来源：http://izu.gotoacloud.top

TS:   if (!data) return;
来源：http://ciq.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://jwg.gotoacloud.top

Go:   if data == nil { return }
来源：http://nae.yongpay.top

Ruby: return if data.nil?
来源：http://tem.ivvv.top

C#:   if (data == null) return;
来源：http://sju.hfpthk.cn

================================================================================
来源：http://wkx.jinqigfzy.top

C. 函数与作用域
来源：http://jxi.chenzaomai.com

================================================================================
来源：http://wqd.dashuyun.cn

[C01] 定义函数
来源：http://qia.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://smp.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eul.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://jjh.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qav.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wno.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qzu.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://vxe.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vet.sjlbkw.cn

[C02] 默认参数
来源：http://opm.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://whp.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wbl.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vdx.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lvd.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qqc.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vhd.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://lft.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://fem.9152youxi.cn

[C03] 可变参数
来源：http://rni.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://nva.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lrb.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnv.jqgufenzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uqy.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://coy.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vpx.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://gmv.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zrc.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://stc.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qgl.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xdh.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nvt.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yvj.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://olg.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://qhk.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://wqc.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://pcr.daria6918.cn

[C05] 返回多个值
来源：http://ddq.fktsv.cn

Py:   return a, b
来源：http://dul.wangdashe.top

PHP:  return [$a, $b];
来源：http://yrb.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aod.xziqi.cn

TS:   return { a, b };
来源：http://cfi.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lxm.yvedp.cn

Go:   return a, b
来源：http://for.xuetiantiany.cn

Ruby: return a, b
来源：http://jls.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://ddo.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://iej.pycfn.com

Py:   square = lambda x: x * x
来源：http://myn.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://plz.yueranfly.top

JS:   const square = x => x * x;
来源：http://bno.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://gsp.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wqg.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://frt.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://eet.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://cbx.hammf.cn

[C07] 把函数作为参数传入
来源：http://csm.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ygn.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://uju.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://khu.xinyue.icu

TS:   arr.map(String)
来源：http://ufv.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nxd.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qzh.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://sgn.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://wkw.xylfe.cn

[C08] 闭包
来源：http://fjt.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hrn.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yqh.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jiv.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ije.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ejr.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://otz.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ntc.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bny.fzhhl.top

[C09] 递归
来源：http://klv.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qso.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ucu.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ooz.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oty.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pfv.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mbi.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uoi.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zrp.9152youxi.cn

[C10] 变量作用域
来源：http://pse.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cxn.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sis.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zan.tarul.cn

TS:   同 JS
来源：http://hlh.jqgfzy.top

Java: 方法内为块级作用域
来源：http://jan.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://zpe.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hwl.sjlbkw.cn

C#:   块级作用域
来源：http://wsd.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://vja.jinyuanbaomall.cn

Py:   from module import func
来源：http://fhs.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kxz.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://hnp.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qac.zhongyouzk.top

Java: import java.util.List;
来源：http://hee.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wvo.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://zrq.yj20258888.top

C#:   using System.Text;
来源：http://fwj.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://tqo.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://epd.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://bew.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://pbk.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://mgk.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vuv.316326.xyz


<!-- 参考信息 -->