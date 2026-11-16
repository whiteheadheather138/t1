代发 wailian999

TS:   s.length
来源：http://gsf.aibaodan.cn

Java: s.length()
来源：http://jnp.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jvd.ehwqpu.com

Ruby: s.length
来源：http://suz.jinghuilouyu.cn

C#:   s.Length
来源：http://iii.cashguo.top

[A23] 大小写转换
来源：http://qmj.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://bpo.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iwk.snrcjt.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://anp.sweek.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rit.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://axn.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bxo.jiagoushi.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mlv.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://owe.yj202588.top

[A24] 去除首尾空白
来源：http://tvv.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://whg.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nkp.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qrj.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wok.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eou.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://ghg.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lat.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://isf.pengpengdd.cyou

[A25] 字符串比较
来源：http://uom.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://gmq.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ikq.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uql.daxiang520.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gcd.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kio.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://srd.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jxl.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pfi.c1oappe.top

[A26] 类型转换总览
来源：http://ekg.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://arp.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tug.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ykx.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://xav.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vqs.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ney.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://svl.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oqr.ctjpmb.com

================================================================================
来源：http://lxj.sufxvd.cn

B. 流程控制
来源：http://nyb.yfazqb.com

================================================================================
来源：http://vrp.jyoumei.cn

[B01] 条件判断 if / else
来源：http://iyn.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wyi.zdbjq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cii.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hdt.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yvx.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://umi.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cos.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qwb.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ygf.yonumen.top

[B02] 多分支 else if / elif
来源：http://cqz.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vmz.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fic.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwt.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqt.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eux.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xhe.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://typ.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kmg.snrcjt.cn

[B03] switch / match / case
来源：http://vyv.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fbo.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dbu.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uln.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iav.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lkb.gaohongyu789.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oqo.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zgu.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://elb.tianlin.xyz

[B04] for 计数循环
来源：http://aqv.ivvv.top

Py:   for i in range(10): print(i)
来源：http://lnb.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zrn.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yqs.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uhe.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ypu.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cyu.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://nao.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qnx.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://rxe.316326.xyz

Py:   for item in arr: print(item)
来源：http://dsd.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cjh.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fyn.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ddq.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://paq.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iye.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://gir.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cee.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://gze.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://faj.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gtk.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://byn.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dya.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zqf.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ixj.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vtv.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vhf.havefunace.top

[B07] while 循环
来源：http://ter.yj20258888.top

Py:   while i < 10: i += 1
来源：http://tjh.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cyd.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://kpn.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://frg.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://das.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gnn.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://qcm.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://vbf.cheryme.top

[B08] do-while（至少执行一次）
来源：http://sbe.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://urk.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yit.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://vcp.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://hwj.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://iuf.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mdy.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wrz.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://uas.vehdjk.com

[B09] break 与 continue
来源：http://cgl.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zzo.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vel.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edu.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://emo.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trf.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xtb.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://czt.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hkw.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://brv.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bzn.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://icu.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gmv.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zdr.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qrr.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mfz.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uvg.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dee.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://jfj.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://hdf.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://nfh.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kif.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ypo.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://smt.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://arw.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://nyt.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cyb.sysykeji.top

[B12] 跳出多层循环
来源：http://soi.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://adc.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eqi.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ony.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zke.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rjp.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vqt.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xot.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fut.guowangkeji.top

[B13] 判断是否为数字
来源：http://mxt.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://ulj.gzhubu.top

PHP:  is_numeric($x)
来源：http://dme.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dkm.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qch.52xcode.cn

Java: x instanceof Number
来源：http://yew.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kym.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://rlf.ybcxt.top

C#:   x is int or double or decimal
来源：http://cvw.xylfe.cn

[B14] 判断值是否在集合内
来源：http://slx.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dvv.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://det.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://eyh.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vpn.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sjb.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dam.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://mmp.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ahi.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://dli.jiagoushi.top

Py:   a and b or not c
来源：http://cdk.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://vjy.fktsv.cn

JS:   a && b || !c
来源：http://hkn.zdbjq.cn

TS:   a && b || !c
来源：http://yju.hnqzz.top

Java: a && b || !c
来源：http://gos.jyoumei.cn

Go:   a && b || !c
来源：http://lnb.ehwqpu.com

Ruby: a && b || !c
来源：http://tng.sweek.top

C#:   a && b || !c
来源：http://vok.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://bvj.xinyue.icu

Py:   if not data: return
来源：http://fuq.yj20258.top

PHP:  if (!$data) { return; }
来源：http://nad.havefunace.top

JS:   if (!data) return;
来源：http://lyt.xinyue.icu

TS:   if (!data) return;
来源：http://mga.9152youxi.cn

Java: if (data == null) return;
来源：http://dzw.jyoumei.cn

Go:   if data == nil { return }
来源：http://avl.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://vii.yonumen.top

C#:   if (data == null) return;
来源：http://kxn.jinghuilouyu.cn

================================================================================
来源：http://gbq.hnxiangtu.top

C. 函数与作用域
来源：http://cia.hysaishi.cn

================================================================================
来源：http://knl.gaohongyu789.top

[C01] 定义函数
来源：http://ffz.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://opp.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqx.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://pel.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mhv.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rce.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://rbf.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://tbx.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cvz.sufxvd.cn

[C02] 默认参数
来源：http://hzc.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://eds.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hcg.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://ejn.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jaj.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://trm.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://psn.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://cxj.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://uyf.ybcxt.top

[C03] 可变参数
来源：http://han.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://csr.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sma.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zww.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vuf.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dlx.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rcm.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://tro.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xgr.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://mmy.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gtr.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zii.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jbt.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fvb.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://vdd.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://yqh.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://irm.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://ajp.jqgfzy.top

[C05] 返回多个值
来源：http://xky.xuetiantiany.cn

Py:   return a, b
来源：http://num.tianlin.xyz

PHP:  return [$a, $b];
来源：http://cdb.haohaochexian.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rbi.jlsjyb.cn

TS:   return { a, b };
来源：http://fvj.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bbe.ctjpmb.com

Go:   return a, b
来源：http://naa.shuidangran.top

Ruby: return a, b
来源：http://hcf.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://dmc.birdmap.top

[C06] 匿名函数 / lambda
来源：http://plm.xziqi.cn

Py:   square = lambda x: x * x
来源：http://xjk.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zqi.yueranfly.top

JS:   const square = x => x * x;
来源：http://bgu.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://wmi.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nsd.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://vro.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://drn.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://sha.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://tht.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qsa.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://gxf.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://akj.cdnleiting.top

TS:   arr.map(String)
来源：http://jkt.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wza.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rds.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://ans.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tga.yueranfly.top

[C08] 闭包
来源：http://qso.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zaa.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ssc.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hdo.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qqi.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hkp.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oif.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jbp.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fik.cucudq.cn

[C09] 递归
来源：http://stb.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ejy.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gpt.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ccy.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwx.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://opq.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ynv.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cov.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vst.gaohongyu789.top

[C10] 变量作用域
来源：http://iby.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uqx.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bub.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gxe.ydjk.org.cn

TS:   同 JS
来源：http://dvx.jiagoushi.top

Java: 方法内为块级作用域
来源：http://tqo.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://hdb.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ioy.hesvh.cn

C#:   块级作用域
来源：http://trp.jinqigufen.top

[C11] 模块导入与导出
来源：http://ouv.haohaochexian.top

Py:   from module import func
来源：http://yix.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hyo.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://shx.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://euq.shzxlz.cn

Java: import java.util.List;
来源：http://pba.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jmm.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://xdz.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://elz.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://pwp.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://fbg.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://bzd.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://rpj.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://jby.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pjc.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://kfj.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://jzc.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gvw.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://rke.zhongyouzk.top


<!-- 参考信息 -->