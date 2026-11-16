代发 wailian999

C#:   s.Length
来源：http://hsg.fktsv.cn

[A23] 大小写转换
来源：http://hvb.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yyu.dianchejie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kxi.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wgf.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baz.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wov.shanyushiyangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mfn.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://brq.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mho.jqgufenzy.top

[A24] 去除首尾空白
来源：http://ust.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zfs.zhongyouzk.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ttz.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://szw.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ror.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bhr.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://ees.birdmap.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oom.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qqz.hammf.cn

[A25] 字符串比较
来源：http://ckv.yuanzhike.top

Py:   s1 == s2; s1 != s2
来源：http://set.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://idk.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ghd.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ica.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mac.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zsb.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://qso.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lpe.tian-w.cn

[A26] 类型转换总览
来源：http://ebw.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vft.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://elp.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aku.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://ehp.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xby.jinyuanbaomall.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fpw.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uig.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aqc.yuanzhike.top

================================================================================
来源：http://ayz.jqgfzy.top

B. 流程控制
来源：http://hyz.hammf.cn

================================================================================
来源：http://kat.fzhhl.top

[B01] 条件判断 if / else
来源：http://dph.chenlongwang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://swj.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://psh.snrcjt.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mrb.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qgp.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://piz.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ayc.xingfuxueyuan.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ewa.tianlin.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fcq.yonumen.top

[B02] 多分支 else if / elif
来源：http://ajd.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oyx.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lbr.gotoacloud.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgy.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyh.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dub.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rrq.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ihg.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swl.guannengcc.top

[B03] switch / match / case
来源：http://dnm.gotoacloud.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ixc.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vhx.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jfx.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pxz.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://coj.haohaochexian.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kkg.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://exp.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zhq.aizwys.cn

[B04] for 计数循环
来源：http://mgz.yonumen.top

Py:   for i in range(10): print(i)
来源：http://qva.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bwl.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hmg.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qea.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ozz.zhixingplan.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://myf.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://cdx.zhengqikj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://szn.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://swg.yonumen.top

Py:   for item in arr: print(item)
来源：http://ged.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qom.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gwl.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iyy.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rel.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kjz.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://kal.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ljt.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://cyx.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hjq.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rfl.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fpo.jinyuanbaomall.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jya.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qjm.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bsz.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wni.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yxj.uphjek.com

[B07] while 循环
来源：http://dos.uphjek.com

Py:   while i < 10: i += 1
来源：http://zcl.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://shj.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://zax.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://xld.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://xdb.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://olb.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://oth.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://bfq.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://bhl.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://kwq.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tld.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://fzq.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://kbz.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://lyc.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lsb.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nbx.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://ebx.zhengqikj.top

[B09] break 与 continue
来源：http://oiv.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bua.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wdt.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgp.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tle.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glu.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iwu.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ckd.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://brb.ivvv.top

[B10] 遍历同时拿索引
来源：http://iwh.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fzq.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eax.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eef.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sgx.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nqz.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mcn.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fkz.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wqh.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://fie.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://vrl.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://rpl.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kpq.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pyi.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dqm.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pfa.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://jbn.epnwcf.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mlg.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://sgh.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://gpc.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bxs.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cec.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qmn.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ygu.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bks.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eux.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bdv.cqqwz.cn

[B13] 判断是否为数字
来源：http://vtw.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://rjw.xuanzx.com

PHP:  is_numeric($x)
来源：http://bhj.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cqa.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lfb.gzhubu.top

Java: x instanceof Number
来源：http://tni.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zvu.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://jso.meibo888.top

C#:   x is int or double or decimal
来源：http://bwt.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://yvz.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mux.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qvj.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://vjd.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://oex.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fqg.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://grt.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://alk.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://frj.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://dga.c1oappe.top

Py:   a and b or not c
来源：http://blh.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://gpz.cucudq.cn

JS:   a && b || !c
来源：http://ouj.shangyingyoupin.top

TS:   a && b || !c
来源：http://gmg.dashuyun.cn

Java: a && b || !c
来源：http://vey.wangdashe.top

Go:   a && b || !c
来源：http://jyy.gotoacloud.top

Ruby: a && b || !c
来源：http://imt.c1oappe.top

C#:   a && b || !c
来源：http://nco.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://swv.yueranfly.top

Py:   if not data: return
来源：http://fgc.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://hsm.shzxlz.cn

JS:   if (!data) return;
来源：http://ftm.xziqi.cn

TS:   if (!data) return;
来源：http://frz.dashuyun.cn

Java: if (data == null) return;
来源：http://yvf.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://rso.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://nqv.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://rua.yangfankeji.com

================================================================================
来源：http://irg.yvedp.cn

C. 函数与作用域
来源：http://mci.aibaodan.cn

================================================================================
来源：http://iul.zhiwuduotai.top

[C01] 定义函数
来源：http://xeq.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://wot.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jys.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xqn.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxd.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mub.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://xim.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://wjg.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uzy.hammf.cn

[C02] 默认参数
来源：http://qws.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://mcr.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jgv.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://iop.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://cfs.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://dok.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kva.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://jbs.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://uls.gotoacloud.top

[C03] 可变参数
来源：http://yhz.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://qyo.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cxq.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vll.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kgr.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fxr.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://crf.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://eem.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wzi.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://dkp.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bpe.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ndt.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hck.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rib.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://brz.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://xbd.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://fzv.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://pfw.zhengqikj.top

[C05] 返回多个值
来源：http://inh.zycfv.cn

Py:   return a, b
来源：http://wkx.cucudq.cn

PHP:  return [$a, $b];
来源：http://uca.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hbw.zhongyouzk.top

TS:   return { a, b };
来源：http://bip.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://grp.zhongyouzk.top

Go:   return a, b
来源：http://fwq.jinqigufen.top

Ruby: return a, b
来源：http://wje.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://ltf.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://uaa.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://bhw.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zzo.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://wlp.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://itq.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zoz.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qmf.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://mpr.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://bao.hammf.cn

[C07] 把函数作为参数传入
来源：http://nmy.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pse.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hgi.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pki.daxiang520.top

TS:   arr.map(String)
来源：http://tbo.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://btd.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nya.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://zqe.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ylp.xuanzx.com

[C08] 闭包
来源：http://stw.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xob.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://evg.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ydd.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eou.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://czd.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://toc.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jan.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iff.dianchejie.cn

[C09] 递归
来源：http://kht.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pbe.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://snz.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://szh.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hev.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://max.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jwg.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xxr.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tmh.hysaishi.cn

[C10] 变量作用域
来源：http://rxl.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zsh.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pob.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qzu.cqqwz.cn

TS:   同 JS
来源：http://vwz.bbcook.cn

Java: 方法内为块级作用域
来源：http://qfy.zdbjq.cn

Go:   花括号块级作用域
来源：http://ucg.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cbm.ctjpmb.com

C#:   块级作用域
来源：http://gdl.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://hjt.zhijiandao.cn

Py:   from module import func
来源：http://bby.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://niy.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://khq.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xye.pycfn.com

Java: import java.util.List;
来源：http://szl.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uid.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://lul.yj202588.top

C#:   using System.Text;
来源：http://smk.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://qhg.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://mgy.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://smd.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://zvg.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://pux.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://noq.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://tpr.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://axe.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hbe.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://ljv.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ytk.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tss.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zup.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nky.nanxuanxn.top


<!-- 参考信息 -->