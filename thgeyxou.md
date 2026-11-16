代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://stu.52xcode.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zus.daxiang520.top

[A24] 去除首尾空白
来源：http://ypy.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tyc.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cze.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mhk.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqy.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zma.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://ptf.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bis.daxiang520.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nkg.redwolf501.top

[A25] 字符串比较
来源：http://yal.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://jyu.yj202588.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lkt.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kzx.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rkw.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ytn.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zfz.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iwp.tanke756.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yja.c1oappe.top

[A26] 类型转换总览
来源：http://rdx.kuanghao11.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cqp.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pai.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wah.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://lcq.zycfv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vid.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wyb.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hyb.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ukj.bbcook.cn

================================================================================
来源：http://bgr.havefunace.top

B. 流程控制
来源：http://vtn.zhaomingkeji.xyz

================================================================================
来源：http://pwu.0kj1m.cn

[B01] 条件判断 if / else
来源：http://low.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gsx.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aeg.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mrm.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mbw.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://tjb.yfazqb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://csd.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://otl.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jtr.ydzc1.top

[B02] 多分支 else if / elif
来源：http://vws.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://icd.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pwi.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bdz.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilo.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hbl.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://scr.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lij.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://and.yuxming.cn

[B03] switch / match / case
来源：http://wrm.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://frt.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://joz.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ymp.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bga.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rtc.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wqf.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ajn.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yjp.quarkkingdee.top

[B04] for 计数循环
来源：http://uoa.yj20258.top

Py:   for i in range(10): print(i)
来源：http://vjz.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dft.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wcg.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yzr.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lxz.hesvh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rgi.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://ohd.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://enp.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://xbt.yj202588.top

Py:   for item in arr: print(item)
来源：http://tlj.bjfxy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mlo.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wcz.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bin.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sim.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://irc.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://pia.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dcj.hcnkem.com

[B06] 遍历字典 / 对象
来源：http://gkc.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://guw.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dwe.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qoj.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mlj.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fyw.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fqd.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dxc.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vph.nanxinkj.top

[B07] while 循环
来源：http://lez.xuanzx.com

Py:   while i < 10: i += 1
来源：http://vgm.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://abj.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://eoc.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://vcl.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://avt.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cju.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://ajf.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://ucu.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://plo.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://ukn.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xyh.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://jtu.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://dqp.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://law.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://suy.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://sld.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://fsj.wangshuangyany.cn

[B09] break 与 continue
来源：http://mxw.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pqu.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tdx.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tec.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzs.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rit.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eju.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xgq.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyw.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://wbw.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxt.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cji.redwolf501.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://trs.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://egy.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zjl.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ykr.pycfn.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vsk.tanke756.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blg.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://que.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://bcs.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://owl.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aak.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://swt.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://frw.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rrc.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://rwx.chenlongwang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wqi.yj20258888.top

[B12] 跳出多层循环
来源：http://spg.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://nel.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cjc.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hrf.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eqw.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lle.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://meg.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bqs.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jew.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://cxo.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://skf.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://pox.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ugl.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wxp.sweek.top

Java: x instanceof Number
来源：http://rge.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qtq.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://npb.nanxinkj.top

C#:   x is int or double or decimal
来源：http://vpd.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://zps.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qhf.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ubf.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://aie.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://bug.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://qmy.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oia.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://bcz.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zrm.aizwys.cn

[B15] 布尔运算与取反
来源：http://klx.fzhhl.top

Py:   a and b or not c
来源：http://gtz.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://wej.havefunace.top

JS:   a && b || !c
来源：http://amg.vehdjk.com

TS:   a && b || !c
来源：http://lgu.zhiwuduotai.top

Java: a && b || !c
来源：http://apy.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://uvz.ybcxt.top

Ruby: a && b || !c
来源：http://khw.c1oappe.top

C#:   a && b || !c
来源：http://afx.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://nur.yj20258888.top

Py:   if not data: return
来源：http://wuz.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://ofq.kuanghao11.cn

JS:   if (!data) return;
来源：http://brj.daxiang520.top

TS:   if (!data) return;
来源：http://ksn.epnwcf.com

Java: if (data == null) return;
来源：http://xpw.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://uee.cheryme.top

Ruby: return if data.nil?
来源：http://gdu.yangfankeji.com

C#:   if (data == null) return;
来源：http://kyo.hysaishi.cn

================================================================================
来源：http://yrj.dianchejie.cn

C. 函数与作用域
来源：http://skf.gaohongyu789.top

================================================================================
来源：http://anj.0kj1m.cn

[C01] 定义函数
来源：http://vbk.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://fpp.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zfs.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://wfq.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rgi.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xtg.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wsx.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://tcf.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uib.hysaishi.cn

[C02] 默认参数
来源：http://olk.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://out.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rpi.sufxvd.cn

JS:   function greet(name = "World") { return name; }
来源：http://cfw.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iqu.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bcz.xylfe.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lqp.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://jfc.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://rbf.fktsv.cn

[C03] 可变参数
来源：http://owo.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://duz.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lxo.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppc.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qsh.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kip.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fhn.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://qxk.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ghn.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://jjq.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qri.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wky.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oju.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bpd.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://khu.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://cct.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://sni.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://urv.zhengqikj.top

[C05] 返回多个值
来源：http://cgg.tian-w.cn

Py:   return a, b
来源：http://vfs.ctjpmb.com

PHP:  return [$a, $b];
来源：http://xxj.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ubh.gotoacloud.top

TS:   return { a, b };
来源：http://lpz.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hjt.gogol.net.cn

Go:   return a, b
来源：http://kpf.shzxlz.cn

Ruby: return a, b
来源：http://jke.jianghu66.top

C#:   return (a, b);              // ValueTuple
来源：http://fzj.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://wxq.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://jnz.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mpc.zdbjq.cn

JS:   const square = x => x * x;
来源：http://ekn.yangfankeji.com

TS:   const square = (x: number): number => x * x;
来源：http://nwl.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ldc.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://vmt.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://rhd.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://wxs.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://lhe.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fjo.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fpw.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hyr.hesvh.cn

TS:   arr.map(String)
来源：http://eav.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jht.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tgt.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://gqe.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mzt.shangyingyoupin.top

[C08] 闭包
来源：http://zvf.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wub.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pzn.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vaf.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://swa.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hkh.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kxy.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hzt.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zip.yuanzhike.top

[C09] 递归
来源：http://hdt.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gga.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://egs.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yrl.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oto.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lwz.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kan.hywenlv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vcl.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gdo.zhixingplan.top

[C10] 变量作用域
来源：http://tkm.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ymh.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eoa.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lhi.ehwqpu.com

TS:   同 JS
来源：http://cyn.svipenyu.cn

Java: 方法内为块级作用域
来源：http://bxg.zdqjudy.top

Go:   花括号块级作用域
来源：http://ves.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://krw.snrcjt.cn

C#:   块级作用域
来源：http://gpz.xziqi.cn

[C11] 模块导入与导出
来源：http://fea.hysaishi.cn

Py:   from module import func
来源：http://vbe.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yjm.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://irr.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jzm.jyoumei.cn

Java: import java.util.List;
来源：http://zck.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nlz.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://wfh.gzhubu.top

C#:   using System.Text;
来源：http://kdi.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://nfc.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://cge.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://kta.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://yhl.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://ial.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wyg.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://okt.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://bzl.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://szr.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://nzv.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zeg.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aco.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sce.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kyz.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://pzi.jinqigufen.top

Go:   func add(a, b int) int
来源：http://gff.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://axx.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://lhs.pycfn.com

[C14] 泛型函数
来源：http://wyt.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fqb.epnwcf.com

PHP:  // 无泛型
来源：http://ckg.uphjek.com

JS:   // 无泛型
来源：http://epm.jqgfzy.top


<!-- 参考信息 -->