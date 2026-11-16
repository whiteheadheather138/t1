代发 wailian999

C#:   s.Length
来源：http://bdq.gaohongyu789.top

[A23] 大小写转换
来源：http://qkj.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eth.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ilk.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://giy.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://osw.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aso.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ktn.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rzq.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gmb.quarkkingdee.top

[A24] 去除首尾空白
来源：http://cba.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://inp.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wfs.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uja.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cgn.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://imc.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://kem.ywan-chungtsiang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://obi.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lmi.chenlongwang.top

[A25] 字符串比较
来源：http://hpg.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://pgi.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://srq.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://euj.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sii.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://voq.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mgb.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rrt.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gkq.sufxvd.cn

[A26] 类型转换总览
来源：http://dkj.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zys.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pbe.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wdd.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://ovd.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qug.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cxw.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://awg.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kfn.bjfxy.top

================================================================================
来源：http://uqn.xuetiantiany.cn

B. 流程控制
来源：http://bcd.zhijiandao.cn

================================================================================
来源：http://mjh.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://zdt.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aqy.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oys.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vxp.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://poj.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yql.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mep.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ihe.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jfa.ivvv.top

[B02] 多分支 else if / elif
来源：http://gwi.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wxo.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://agz.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjx.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tfv.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lhz.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://npz.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://snm.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gcv.nanxuanxn.top

[B03] switch / match / case
来源：http://ahe.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://weg.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://egn.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rcs.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fnt.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xix.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iaa.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hrz.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jky.hnxiangtu.top

[B04] for 计数循环
来源：http://flw.tarul.cn

Py:   for i in range(10): print(i)
来源：http://plm.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zbs.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ouf.yongpay.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nnc.cdnleiting.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zdz.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gvd.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://gcr.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mul.yj202588.top

[B05] 遍历数组 / 列表
来源：http://fuu.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://zlb.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bgc.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hue.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tzc.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gto.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tkg.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://ybt.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sap.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://smb.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uiu.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lxa.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bqy.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qnv.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yem.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rxa.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cmh.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ims.fengsongda.top

[B07] while 循环
来源：http://aly.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://jpm.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://fpd.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://dkt.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://oyi.tanke756.top

Java: while (i < 10) { i++; }
来源：http://peb.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://spy.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://frf.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://eca.tanke756.top

[B08] do-while（至少执行一次）
来源：http://zzz.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://nih.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gqe.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://cur.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://vmz.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://hcn.cashguo.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kbn.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://ady.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://xvp.yfazqb.com

[B09] break 与 continue
来源：http://qyq.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ule.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://csg.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hib.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfj.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cvi.dianchejie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ecv.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lud.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://slc.ydzc1.top

[B10] 遍历同时拿索引
来源：http://byt.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wjk.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xgz.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vnc.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fqx.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aca.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oyr.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://azi.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cux.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://cnc.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://uup.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://mvn.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hmc.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gck.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://few.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qxl.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://zhi.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lbr.hysaishi.cn

[B12] 跳出多层循环
来源：http://znn.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ckf.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fta.xziqi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gvl.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ede.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://prr.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://juj.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://etc.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yfz.ppjwa.cn

[B13] 判断是否为数字
来源：http://gyj.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://rcm.yonumen.top

PHP:  is_numeric($x)
来源：http://lom.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hgg.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pzm.shangyingyoupin.top

Java: x instanceof Number
来源：http://hzf.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ncf.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://kbh.hywenlv.cn

C#:   x is int or double or decimal
来源：http://ddx.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://ksw.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vpb.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://klf.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://pty.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://scp.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xtc.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lrv.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://vtq.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zuh.yj202588.top

[B15] 布尔运算与取反
来源：http://ksg.gogol.net.cn

Py:   a and b or not c
来源：http://bci.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://pvb.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://olv.redwolf501.top

TS:   a && b || !c
来源：http://vil.ydzc1.top

Java: a && b || !c
来源：http://vkx.uphjek.com

Go:   a && b || !c
来源：http://bxs.yj20258.top

Ruby: a && b || !c
来源：http://bds.bbcook.cn

C#:   a && b || !c
来源：http://vis.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://dej.zdbjq.cn

Py:   if not data: return
来源：http://cgk.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://prc.haohaochexian.top

JS:   if (!data) return;
来源：http://wri.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://jdh.pengpengdd.cyou

Java: if (data == null) return;
来源：http://ygy.0kj1m.cn

Go:   if data == nil { return }
来源：http://kpv.aizwys.cn

Ruby: return if data.nil?
来源：http://kxa.zhengqikj.top

C#:   if (data == null) return;
来源：http://xsr.meibo888.top

================================================================================
来源：http://zrv.jinghuilouyu.cn

C. 函数与作用域
来源：http://rxr.nanxinkj.top

================================================================================
来源：http://svq.nanxuanxn.top

[C01] 定义函数
来源：http://sst.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://vtu.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxt.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://tjm.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aan.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qvc.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nkp.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://iun.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://stn.jinghuilouyu.cn

[C02] 默认参数
来源：http://wdm.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://ubr.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vzz.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://igo.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wrk.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ipk.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qki.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://hrk.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://otk.fanxiaobao.xyz

[C03] 可变参数
来源：http://ebd.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://fmh.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uim.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uok.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zoh.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nzc.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vce.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bhc.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xeb.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://gqb.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lnl.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rln.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hrl.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wbg.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://gun.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://xth.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://owd.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://rnr.hcnkem.com

[C05] 返回多个值
来源：http://byx.nanxinkj.top

Py:   return a, b
来源：http://chh.fehbvm.com

PHP:  return [$a, $b];
来源：http://yci.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://nhm.jqgufenzy.top

TS:   return { a, b };
来源：http://cmg.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qvv.ctjpmb.com

Go:   return a, b
来源：http://srv.yj20258888.top

Ruby: return a, b
来源：http://pqt.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://qid.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://eeq.mhx1999.top

Py:   square = lambda x: x * x
来源：http://crk.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cch.cashguo.top

JS:   const square = x => x * x;
来源：http://shp.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://jva.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://njf.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://uvn.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://gve.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fzc.daria6918.cn

[C07] 把函数作为参数传入
来源：http://vjz.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zfe.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://dfk.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dgw.hnxiangtu.top

TS:   arr.map(String)
来源：http://scq.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hcv.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zmb.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://zgv.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ocq.yj202588.top

[C08] 闭包
来源：http://phw.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ydk.316326.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wws.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kyp.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rsm.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ubb.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://met.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uao.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mrz.shangyingyoupin.top

[C09] 递归
来源：http://lee.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vyt.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wtm.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ecg.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aaj.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fld.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://akf.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lss.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://svf.hywenlv.cn

[C10] 变量作用域
来源：http://omf.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uox.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aqb.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dsr.yj20258888.top

TS:   同 JS
来源：http://zlu.aizwys.cn

Java: 方法内为块级作用域
来源：http://kmt.vqdsnc.cn

Go:   花括号块级作用域
来源：http://ofj.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jsm.shangyingyoupin.top

C#:   块级作用域
来源：http://apy.ehwqpu.com

[C11] 模块导入与导出
来源：http://yam.yongpay.top

Py:   from module import func
来源：http://kpm.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lxe.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yth.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cew.c1oappe.top

Java: import java.util.List;
来源：http://vsb.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ozu.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://pau.dianchejie.cn

C#:   using System.Text;
来源：http://jui.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://bvk.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://rgl.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://tyt.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://wdr.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://sci.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lps.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://uia.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://fni.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ypa.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://vvf.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hdg.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqj.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vyv.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fgu.redwolf501.top


<!-- 参考信息 -->