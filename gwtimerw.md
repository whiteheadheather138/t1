代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ruq.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oal.yueranfly.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yfl.0kj1m.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cbt.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yiv.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pth.ydjk.org.cn

[A24] 去除首尾空白
来源：http://uwy.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kar.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://riy.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://szp.hcnkem.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://exw.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://neh.shanyushiyangtech.top

Go:   strings.TrimSpace(s)
来源：http://wjn.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://owg.havefunace.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jgu.fanxiaobao.xyz

[A25] 字符串比较
来源：http://ang.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://lir.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zbm.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mhy.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wia.zdbjq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ubm.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pxu.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bww.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://upi.sxryk.cn

[A26] 类型转换总览
来源：http://orv.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hgx.bjfxy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qak.yonumen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://msy.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://sfi.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ogs.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hjj.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://moq.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zfo.ctjpmb.com

================================================================================
来源：http://cuu.iojbl.cn

B. 流程控制
来源：http://fsc.pengpengdd.cyou

================================================================================
来源：http://uul.shuidangran.top

[B01] 条件判断 if / else
来源：http://hhg.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fio.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://chn.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xez.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uws.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nri.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fvt.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dya.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xxd.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://zkp.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iss.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uoe.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrf.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uml.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvw.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zxh.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kyd.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://phw.iojbl.cn

[B03] switch / match / case
来源：http://ult.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lzf.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rom.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://str.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ysf.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bkg.c1oappe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hqd.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tbb.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wcr.hcnkem.com

[B04] for 计数循环
来源：http://qld.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://xhj.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://izu.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://otb.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fxd.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dij.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://auq.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://hzd.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ocn.yj202588.top

[B05] 遍历数组 / 列表
来源：http://kgk.yj202588.top

Py:   for item in arr: print(item)
来源：http://qer.shanyushiyangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vsz.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ytk.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ktm.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://okj.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://frt.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://gjp.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dss.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://eou.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qmx.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://emz.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gjc.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lfy.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xka.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dxq.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xvb.sjlbkw.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fiw.9152youxi.cn

[B07] while 循环
来源：http://wrt.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://php.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://xlb.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://uxl.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://vhy.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://xeq.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wke.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://reo.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://uzn.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://dfn.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://qeg.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bwc.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://zyl.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://anf.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://frt.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ixi.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://eys.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://pzm.epnwcf.com

[B09] break 与 continue
来源：http://khh.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rxc.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ckw.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://njj.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rsc.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dls.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qkb.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jmx.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ojl.hammf.cn

[B10] 遍历同时拿索引
来源：http://vxm.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tog.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tep.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xnr.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hbn.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vzw.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://voo.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://arm.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://brk.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://twh.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://dwd.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://sqq.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xum.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://irx.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xiz.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hnu.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://mgm.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pln.jqgufenzy.top

[B12] 跳出多层循环
来源：http://ynh.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xei.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ipv.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pnm.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ckl.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uhz.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ebw.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gpk.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://man.dianchejie.cn

[B13] 判断是否为数字
来源：http://mpu.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://iyq.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://twe.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cmh.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wtn.jqgufenzy.top

Java: x instanceof Number
来源：http://rib.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jrm.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://lwg.pycfn.com

C#:   x is int or double or decimal
来源：http://kti.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://gow.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wxj.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rba.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://adw.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://yfl.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://lsv.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tcz.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://ftk.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oeg.hfpthk.cn

[B15] 布尔运算与取反
来源：http://lbk.wangshuangyany.cn

Py:   a and b or not c
来源：http://shs.redwolf501.top

PHP:  $a && $b || !$c
来源：http://kcu.xziqi.cn

JS:   a && b || !c
来源：http://bbr.svipenyu.cn

TS:   a && b || !c
来源：http://fhn.zdbjq.cn

Java: a && b || !c
来源：http://wlb.guowangkeji.top

Go:   a && b || !c
来源：http://zrs.cashguo.top

Ruby: a && b || !c
来源：http://yie.zhiwuduotai.top

C#:   a && b || !c
来源：http://vll.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sbd.52xcode.cn

Py:   if not data: return
来源：http://gyv.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://dxh.gogol.net.cn

JS:   if (!data) return;
来源：http://dtx.hnxiangtu.top

TS:   if (!data) return;
来源：http://oui.zhoulong.xyz

Java: if (data == null) return;
来源：http://lkd.jyoumei.cn

Go:   if data == nil { return }
来源：http://nuo.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://pkt.c1oappe.top

C#:   if (data == null) return;
来源：http://zuw.jinqigufen.top

================================================================================
来源：http://awg.iojbl.cn

C. 函数与作用域
来源：http://nlt.yj20258.top

================================================================================
来源：http://npd.zhijiandao.cn

[C01] 定义函数
来源：http://ndn.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://qog.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mek.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://xwp.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aao.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://opa.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://tcx.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://ozs.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://orz.shuidangran.top

[C02] 默认参数
来源：http://rrc.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://ngi.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gqc.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://vkf.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qdn.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ifg.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rfs.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://fxi.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://yyq.ybcxt.top

[C03] 可变参数
来源：http://rrc.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://gkz.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://phl.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bir.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ejm.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aic.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qmd.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jrz.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://buo.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://glq.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qpm.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yal.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yey.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://piy.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://kdq.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://wgc.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://jli.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://vvv.sjlbkw.cn

[C05] 返回多个值
来源：http://fnt.gaohongyu789.top

Py:   return a, b
来源：http://hdo.tianlin.xyz

PHP:  return [$a, $b];
来源：http://mtm.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fdq.zhixingplan.top

TS:   return { a, b };
来源：http://yhk.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mgc.zdqjudy.top

Go:   return a, b
来源：http://qva.dashuyun.cn

Ruby: return a, b
来源：http://nkd.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://rth.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://zto.wangdashe.top

Py:   square = lambda x: x * x
来源：http://hwh.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dec.iojbl.cn

JS:   const square = x => x * x;
来源：http://geu.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://ism.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ijk.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://abe.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://zwl.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ibz.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://acv.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yxj.ehwqpu.com

PHP:  array_map("strtoupper", $arr);
来源：http://sqg.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ute.wangshuangyany.cn

TS:   arr.map(String)
来源：http://ire.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://otj.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ipm.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://fva.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://glb.yj20258888.top

[C08] 闭包
来源：http://egy.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wxf.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wdu.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eqi.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nql.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rck.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bwu.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tmq.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lbo.epnwcf.com

[C09] 递归
来源：http://dty.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mbi.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rzv.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rfj.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ubo.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jse.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ruk.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rqk.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ckt.xziqi.cn

[C10] 变量作用域
来源：http://ltf.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aqi.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dch.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zbw.daria6918.cn

TS:   同 JS
来源：http://kdb.ctjpmb.com

Java: 方法内为块级作用域
来源：http://ttj.yongpay.top

Go:   花括号块级作用域
来源：http://ioz.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pmz.jinqigufen.top

C#:   块级作用域
来源：http://pzf.zhongyouzk.top

[C11] 模块导入与导出
来源：http://keu.cqqwz.cn

Py:   from module import func
来源：http://nmi.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ymc.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hqv.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ixk.zhengqikj.top

Java: import java.util.List;
来源：http://cvz.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kip.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://npi.dashuyun.cn

C#:   using System.Text;
来源：http://ucj.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://bwp.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://cqg.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://eef.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://nhh.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://vhu.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gym.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://kxv.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://emn.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bso.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://ork.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tcj.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cri.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iiv.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://itm.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://rix.iojbl.cn

Go:   func add(a, b int) int
来源：http://tei.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mgq.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://icf.cucudq.cn


<!-- 参考信息 -->