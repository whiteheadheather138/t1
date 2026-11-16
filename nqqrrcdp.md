代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://azq.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jrq.dashuyun.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wsh.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dtc.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mgu.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ugm.xziqi.cn

[A24] 去除首尾空白
来源：http://qbx.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uyb.gaohongyu789.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mek.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vuh.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kcc.ydjk.org.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vgk.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://vtq.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wqq.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://txg.cucudq.cn

[A25] 字符串比较
来源：http://hdp.tarul.cn

Py:   s1 == s2; s1 != s2
来源：http://bdg.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://leb.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qrg.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uob.ydzc1.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sxw.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wjm.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rgz.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wvo.fehbvm.com

[A26] 类型转换总览
来源：http://csi.yueranfly.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bqo.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dvl.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://luv.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://udd.shanyushiyangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fgs.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jbc.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://gdq.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tmk.sufxvd.cn

================================================================================
来源：http://ajh.yj20258.top

B. 流程控制
来源：http://ixu.havefunace.top

================================================================================
来源：http://atq.nwbrower.top

[B01] 条件判断 if / else
来源：http://hko.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://epf.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ltg.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://que.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://npk.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sjr.zhongyouzk.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nik.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://azj.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yuj.smart0.xyz

[B02] 多分支 else if / elif
来源：http://lzb.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://prs.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qpq.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gxy.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mpv.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkl.jlsjyb.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tsp.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rph.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://azg.fehbvm.com

[B03] switch / match / case
来源：http://iqb.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gll.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gmj.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://orn.zhoulong.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dnm.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sqi.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gny.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vzi.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tdu.zdbjq.cn

[B04] for 计数循环
来源：http://qiu.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://cmb.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bvq.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qgg.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zfc.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://smn.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ysf.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://noa.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hso.hammf.cn

[B05] 遍历数组 / 列表
来源：http://mfr.ydzc1.top

Py:   for item in arr: print(item)
来源：http://eab.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zch.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://raw.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zkx.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jsh.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ues.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://nqr.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bin.yj202588.top

[B06] 遍历字典 / 对象
来源：http://zwt.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cuc.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sjx.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://grf.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xrd.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pah.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tna.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://esg.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fnk.jinyuanbaomall.cn

[B07] while 循环
来源：http://wbn.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://wua.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://jjf.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://yyq.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://ocx.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://enf.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nbt.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://hhe.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://bua.yongpay.top

[B08] do-while（至少执行一次）
来源：http://vaw.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://qgl.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bzo.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://wgk.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://uda.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://ndl.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ljk.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://gtn.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://zgc.epnwcf.com

[B09] break 与 continue
来源：http://afc.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jrk.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lnn.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgn.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://too.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydu.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xqx.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://njp.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrv.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://ldo.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uud.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://skp.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gdp.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xeo.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kev.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hfo.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fhw.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mpr.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://spd.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://oow.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://xoy.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://otn.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://got.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sln.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qmv.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://era.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://avv.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://npi.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pmi.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ynf.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bri.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bzc.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ghs.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ixg.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ujw.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sve.sufxvd.cn

[B13] 判断是否为数字
来源：http://hpj.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://hna.mhx1999.top

PHP:  is_numeric($x)
来源：http://biv.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hyq.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcb.vehdjk.com

Java: x instanceof Number
来源：http://kll.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qoh.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://wph.cheryme.top

C#:   x is int or double or decimal
来源：http://gjn.xylfe.cn

[B14] 判断值是否在集合内
来源：http://xus.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fnj.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lox.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://via.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://qyg.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pbb.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://htq.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://iyz.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vza.cucudq.cn

[B15] 布尔运算与取反
来源：http://sss.ehwqpu.com

Py:   a and b or not c
来源：http://kar.yj202588.top

PHP:  $a && $b || !$c
来源：http://rvh.tian-w.cn

JS:   a && b || !c
来源：http://zco.hesvh.cn

TS:   a && b || !c
来源：http://nua.smart0.xyz

Java: a && b || !c
来源：http://uue.yj20258888.top

Go:   a && b || !c
来源：http://ghh.hysaishi.cn

Ruby: a && b || !c
来源：http://twu.yuanzhike.top

C#:   a && b || !c
来源：http://hvc.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tyw.uphjek.com

Py:   if not data: return
来源：http://bml.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://xdm.zhiwuduotai.top

JS:   if (!data) return;
来源：http://cfo.bbcook.cn

TS:   if (!data) return;
来源：http://gwl.xuetiantiany.cn

Java: if (data == null) return;
来源：http://eeo.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://bmb.yfazqb.com

Ruby: return if data.nil?
来源：http://sur.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://xnx.tanke756.top

================================================================================
来源：http://oii.bbcook.cn

C. 函数与作用域
来源：http://nsf.yvedp.cn

================================================================================
来源：http://fyi.sysykeji.top

[C01] 定义函数
来源：http://rti.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://stk.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rzq.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://prs.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://deg.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fuq.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hye.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://nud.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gyo.xinyue.icu

[C02] 默认参数
来源：http://pdf.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://bvi.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://yjp.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://pxb.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gqv.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://pre.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ths.xylfe.cn

Ruby: def greet(name = "World") = name
来源：http://afn.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://nef.cqqwz.cn

[C03] 可变参数
来源：http://woq.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://igr.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://edy.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vyc.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cav.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cgf.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sbc.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://upx.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://icc.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://fuv.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pap.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kwd.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ify.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vvq.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://rxp.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://brz.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://gbo.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://yqu.cqqwz.cn

[C05] 返回多个值
来源：http://lqi.shanyushiyangkeji.top

Py:   return a, b
来源：http://ixn.xylfe.cn

PHP:  return [$a, $b];
来源：http://zmo.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nhc.svipenyu.cn

TS:   return { a, b };
来源：http://vwq.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://awq.quarkkingdee.top

Go:   return a, b
来源：http://hiv.zhiwuduotai.top

Ruby: return a, b
来源：http://gar.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://vyq.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://glo.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://kwj.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rqb.fengsongda.top

JS:   const square = x => x * x;
来源：http://sbw.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://boi.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ber.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cfc.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://coc.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://txr.yongpay.top

[C07] 把函数作为参数传入
来源：http://dnu.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ywr.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ccu.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nym.yanxiufei.cn

TS:   arr.map(String)
来源：http://xrz.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ntp.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nnl.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://abl.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lxh.feifeiyinyue.top

[C08] 闭包
来源：http://bdn.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uby.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ixn.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://imq.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bls.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xng.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ejk.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bzw.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wir.dashuyun.cn

[C09] 递归
来源：http://mas.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mcg.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qxy.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://huv.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qfu.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://huj.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nie.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://niv.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wea.yj20258.top

[C10] 变量作用域
来源：http://xrt.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://crv.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uuy.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fne.nanxuanxn.top

TS:   同 JS
来源：http://jsr.9152youxi.cn

Java: 方法内为块级作用域
来源：http://shm.jlsjyb.cn

Go:   花括号块级作用域
来源：http://vwy.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ime.jinyuanbaomall.cn

C#:   块级作用域
来源：http://saz.yangfankeji.com

[C11] 模块导入与导出
来源：http://vks.ehwqpu.com

Py:   from module import func
来源：http://uxr.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iwh.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://fct.aibaodan.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ynn.guowangkeji.top

Java: import java.util.List;
来源：http://ypl.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vhu.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://efo.jlsjyb.cn

C#:   using System.Text;
来源：http://lcs.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://frn.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://tpl.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://ffe.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://ukx.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://nsk.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pxk.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://cwg.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://vky.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hhl.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://pcb.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fyw.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lqa.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://igf.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cyi.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://pni.daria6918.cn

Go:   func add(a, b int) int
来源：http://cxe.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fcp.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://rbl.yj202588.top


<!-- 参考信息 -->