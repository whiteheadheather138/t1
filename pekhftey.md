代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bei.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oam.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ozm.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xpv.hongshengwenyu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tnl.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nbn.jianghu66.top

[A24] 去除首尾空白
来源：http://qgj.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gdl.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rgi.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zjw.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aut.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wqx.tarul.cn

Go:   strings.TrimSpace(s)
来源：http://dyc.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lkj.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cua.sufxvd.cn

[A25] 字符串比较
来源：http://kkn.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://dfq.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uww.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wbp.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zoz.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vrn.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ggs.sweek.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xvx.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rvc.guannengcc.top

[A26] 类型转换总览
来源：http://odk.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xde.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://psx.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wuk.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://doz.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pyy.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sgv.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wmz.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gra.daxiang520.top

================================================================================
来源：http://sfb.yvedp.cn

B. 流程控制
来源：http://cdo.shuidangran.top

================================================================================
来源：http://wtz.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://ckn.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dpe.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qqk.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cty.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kjx.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ciq.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nhd.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yww.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yoh.hcnkem.com

[B02] 多分支 else if / elif
来源：http://ijg.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mga.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fjy.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://maa.havefunace.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxb.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://los.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zkh.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fxe.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szb.sjlbkw.cn

[B03] switch / match / case
来源：http://gji.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://omi.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yeb.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wft.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bwh.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xrn.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vac.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ccf.dashuyun.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jwv.zycfv.cn

[B04] for 计数循环
来源：http://gsb.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://zae.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fcy.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kdd.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lrr.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lnp.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xmy.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://xkk.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bos.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://blo.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://eeh.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://idl.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://nlk.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://avl.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qyb.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://koz.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://jve.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vjq.yj202588.top

[B06] 遍历字典 / 对象
来源：http://osk.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://flm.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pja.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ipl.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eak.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oun.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://caz.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cpo.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tej.fanxiaobao.xyz

[B07] while 循环
来源：http://fgg.vehdjk.com

Py:   while i < 10: i += 1
来源：http://vyy.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://nin.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://ilc.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://ztr.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://rrk.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ekv.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://qnk.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://hup.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://jmt.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://nay.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xss.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://ycd.xylfe.cn

TS:   do { i++; } while (i < 10);
来源：http://igk.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://gvt.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ufm.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://zro.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://qai.chenlongwang.top

[B09] break 与 continue
来源：http://dpz.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ock.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vrq.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhc.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzj.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xah.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zlj.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vbr.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zta.mhx1999.top

[B10] 遍历同时拿索引
来源：http://ydc.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cdb.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sgc.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://piq.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lbc.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://crt.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dvr.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ctx.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gop.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://vxb.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://hra.yonumen.top

PHP:  range(0, 10, 2);
来源：http://qzq.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nag.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xef.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xot.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xbk.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://umh.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rtg.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://eql.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://reu.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://lim.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cai.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://etx.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mep.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kxo.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zya.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ogw.epnwcf.com

[B13] 判断是否为数字
来源：http://exf.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://uih.tian-w.cn

PHP:  is_numeric($x)
来源：http://dcy.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qmo.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://auc.shanyushiyangtech.top

Java: x instanceof Number
来源：http://gqe.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mjh.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://bas.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://fmo.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://xnw.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lgq.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xuz.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://dej.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://lpa.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ocq.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wxh.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://mmi.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rrb.guowangkeji.top

[B15] 布尔运算与取反
来源：http://wtk.jiagoushi.top

Py:   a and b or not c
来源：http://qiw.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://yyg.andypj.xyz

JS:   a && b || !c
来源：http://gdm.cqqwz.cn

TS:   a && b || !c
来源：http://sjl.dashuyun.cn

Java: a && b || !c
来源：http://czf.jqgufenzy.top

Go:   a && b || !c
来源：http://dfs.sxryk.cn

Ruby: a && b || !c
来源：http://jvq.tarul.cn

C#:   a && b || !c
来源：http://rrr.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://ycu.jinghuilouyu.cn

Py:   if not data: return
来源：http://pvq.meibo888.top

PHP:  if (!$data) { return; }
来源：http://ueb.zhongyouzk.top

JS:   if (!data) return;
来源：http://xzq.ctjpmb.com

TS:   if (!data) return;
来源：http://mjk.guannengcc.top

Java: if (data == null) return;
来源：http://yne.cqqwz.cn

Go:   if data == nil { return }
来源：http://jfr.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://hyj.dashuyun.cn

C#:   if (data == null) return;
来源：http://ooa.nanxinkj.top

================================================================================
来源：http://bwg.jinghuilouyu.cn

C. 函数与作用域
来源：http://ced.yangfankeji.com

================================================================================
来源：http://ziu.nanxinkj.top

[C01] 定义函数
来源：http://nhy.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://npv.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tea.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://mvy.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bzk.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bor.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://gbo.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://vnx.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jwf.havefunace.top

[C02] 默认参数
来源：http://eta.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://oes.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ant.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://xgk.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://ksi.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://eft.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gvz.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://pqm.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://jqb.yj202588.top

[C03] 可变参数
来源：http://ikm.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://lzb.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gom.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oii.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jiu.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dnp.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hzt.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ofc.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vty.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://cgu.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hdz.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tnt.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hlc.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hkh.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://gxw.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://ptl.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://xln.sweek.top

C#:   f(a: 1, b: 2)
来源：http://wgl.hnqzz.top

[C05] 返回多个值
来源：http://giq.svipenyu.cn

Py:   return a, b
来源：http://wji.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://hyq.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xgl.jqgufenzy.top

TS:   return { a, b };
来源：http://kdj.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cyl.vehdjk.com

Go:   return a, b
来源：http://gvc.vqdsnc.cn

Ruby: return a, b
来源：http://wgw.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://rgi.yj20258.top

[C06] 匿名函数 / lambda
来源：http://xor.xuanzx.com

Py:   square = lambda x: x * x
来源：http://wer.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://llh.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://zov.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://jom.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eit.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://cmj.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://rhw.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://bbs.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://iem.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kuo.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://rvn.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://apv.hongshengwenyu.top

TS:   arr.map(String)
来源：http://xrm.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rtc.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hyv.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://tal.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nrn.shanyushiyangtech.top

[C08] 闭包
来源：http://btd.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bhd.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iov.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://spy.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jdy.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pwc.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iwy.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://otl.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://orq.xylfe.cn

[C09] 递归
来源：http://rhh.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jvs.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eiw.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pos.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://maq.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zke.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xks.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://djo.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tyv.dashuyun.cn

[C10] 变量作用域
来源：http://rps.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ciz.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zxi.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gzl.sweek.top

TS:   同 JS
来源：http://vhd.yj202588.top

Java: 方法内为块级作用域
来源：http://bza.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://mji.vqdsnc.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oul.zdqjudy.top

C#:   块级作用域
来源：http://eri.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://aed.mhx1999.top

Py:   from module import func
来源：http://zpg.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dyo.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kkv.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vjc.smart0.xyz

Java: import java.util.List;
来源：http://ieh.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xst.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://kzu.ydzc1.top

C#:   using System.Text;
来源：http://hvn.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://fnz.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://avr.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://may.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://ain.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://vrc.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wef.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://rrh.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://kkw.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yzv.haohaochexian.top

[C13] 类型声明 / 类型注解
来源：http://hfd.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dln.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://toz.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://big.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sch.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lme.vehdjk.com

Go:   func add(a, b int) int
来源：http://yul.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xss.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://btn.dianchejie.cn


<!-- 参考信息 -->