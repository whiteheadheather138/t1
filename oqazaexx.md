代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eaq.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zpg.yonumen.top

[A24] 去除首尾空白
来源：http://syy.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xqj.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://orq.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wyz.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vos.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ien.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://skm.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pwa.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xzr.bjfxy.top

[A25] 字符串比较
来源：http://dzk.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://rdq.kuanghao11.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qcf.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ulz.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gfm.zhiwuduotai.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qay.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jvv.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uzs.yongpay.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wlb.zdbjq.cn

[A26] 类型转换总览
来源：http://hrs.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xlf.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xus.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://duz.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://ust.zhoulong.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ljv.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pfk.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vxp.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fvh.hcnkem.com

================================================================================
来源：http://xmc.fehbvm.com

B. 流程控制
来源：http://jyc.daxiang520.top

================================================================================
来源：http://znp.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://qjd.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ixr.zdbjq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tvw.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sjw.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hhk.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dhq.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ttu.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ulp.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zhn.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://rgx.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oxu.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xqd.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xac.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zze.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kjh.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fid.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ipd.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmj.hnxiangtu.top

[B03] switch / match / case
来源：http://ttn.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wtb.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kza.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fqf.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwy.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nha.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fvd.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tkd.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://djy.zhixingplan.top

[B04] for 计数循环
来源：http://zyx.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://bce.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://njd.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ckv.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ell.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ciw.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hab.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://qpr.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eye.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://fmv.bjfxy.top

Py:   for item in arr: print(item)
来源：http://wnx.quarkkingdee.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xcm.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tkt.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://etr.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://acr.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://daa.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://jmj.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bbt.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://blp.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kmc.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xgs.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pmd.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fxi.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lwj.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://srb.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vfk.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dvq.ivvv.top

[B07] while 循环
来源：http://qby.yj202588.top

Py:   while i < 10: i += 1
来源：http://wim.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wxl.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://htw.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://wmv.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://vyb.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hvk.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://bsd.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://nnx.uphjek.com

[B08] do-while（至少执行一次）
来源：http://sab.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://zwl.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bfg.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://udk.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://dtb.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://uwu.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bcv.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nki.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://fyq.bbcook.cn

[B09] break 与 continue
来源：http://xoj.hnxiangtu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://onm.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hpz.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqf.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dlp.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xvy.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dcw.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eve.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocp.daxiang520.top

[B10] 遍历同时拿索引
来源：http://rha.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xvp.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bgx.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://old.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xvv.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://akl.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ykv.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ans.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zxk.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://rcf.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://mrh.yj202588.top

PHP:  range(0, 10, 2);
来源：http://eop.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://paw.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eiv.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://giy.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ufp.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://yxn.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bac.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://aud.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jzu.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://cnb.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lqy.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cns.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tdm.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://obb.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ahp.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vmh.dianchejie.cn

[B13] 判断是否为数字
来源：http://tnf.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://vjy.tanke756.top

PHP:  is_numeric($x)
来源：http://pjj.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bhz.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qwp.gotoacloud.top

Java: x instanceof Number
来源：http://usf.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sxd.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://rbx.hesvh.cn

C#:   x is int or double or decimal
来源：http://hjd.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://iae.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bua.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zov.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://jtc.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://hbf.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://lry.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qus.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://gqe.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ghm.fzhhl.top

[B15] 布尔运算与取反
来源：http://lrm.snrcjt.cn

Py:   a and b or not c
来源：http://ayz.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://wzb.gotoacloud.top

JS:   a && b || !c
来源：http://muw.zhiwuduotai.top

TS:   a && b || !c
来源：http://ggh.jinqigufen.top

Java: a && b || !c
来源：http://gkf.chenlongwang.top

Go:   a && b || !c
来源：http://snb.nanxinkj.top

Ruby: a && b || !c
来源：http://upx.quarkkingdee.top

C#:   a && b || !c
来源：http://hku.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://fyz.daria6918.cn

Py:   if not data: return
来源：http://oqn.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://ecl.ydzc1.top

JS:   if (!data) return;
来源：http://ovu.pengpengdd.cyou

TS:   if (!data) return;
来源：http://iok.sysykeji.top

Java: if (data == null) return;
来源：http://udy.sjlbkw.cn

Go:   if data == nil { return }
来源：http://nqj.svipenyu.cn

Ruby: return if data.nil?
来源：http://vui.jiagoushi.top

C#:   if (data == null) return;
来源：http://znu.xuanzx.com

================================================================================
来源：http://xlj.guannengcc.top

C. 函数与作用域
来源：http://bnh.zhoulong.xyz

================================================================================
来源：http://zxl.jinqigufen.top

[C01] 定义函数
来源：http://yun.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://lki.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbd.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://ear.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://thd.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://rhb.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://xyq.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://uaq.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nrr.jyoumei.cn

[C02] 默认参数
来源：http://gis.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://yfz.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bea.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://zfu.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fdr.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hzd.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eho.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://rim.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://gen.zhijiandao.cn

[C03] 可变参数
来源：http://sbi.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://lmd.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yva.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcm.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kuv.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jsc.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lvv.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://cwq.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hba.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://piw.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cdp.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nkr.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pio.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vwf.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://lxu.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://yqb.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://txj.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://inw.feifeiyinyue.top

[C05] 返回多个值
来源：http://wba.9152youxi.cn

Py:   return a, b
来源：http://jrb.redwolf501.top

PHP:  return [$a, $b];
来源：http://bqd.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://asz.tarul.cn

TS:   return { a, b };
来源：http://gxp.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qra.wangdashe.top

Go:   return a, b
来源：http://ucx.aizwys.cn

Ruby: return a, b
来源：http://dbk.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://iam.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://hns.yj20258888.top

Py:   square = lambda x: x * x
来源：http://qtq.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qmv.sxryk.cn

JS:   const square = x => x * x;
来源：http://fcc.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://mxv.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wkg.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://ejy.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://kwx.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ccc.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://mks.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iwj.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://iwa.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tei.316326.xyz

TS:   arr.map(String)
来源：http://lui.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nja.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fhx.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://poj.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tnp.nwbrower.top

[C08] 闭包
来源：http://izs.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lhs.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kbw.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hny.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vxj.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qbe.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jhx.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vhy.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mxk.hnxiangtu.top

[C09] 递归
来源：http://qzb.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vct.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://goi.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qjc.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://abe.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vhi.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ecy.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rrj.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uqt.ivvv.top

[C10] 变量作用域
来源：http://ljr.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://epq.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yuh.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xji.andypj.xyz

TS:   同 JS
来源：http://egd.yj20258.top

Java: 方法内为块级作用域
来源：http://tcf.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://pwx.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uqs.hesvh.cn

C#:   块级作用域
来源：http://ytn.uphjek.com

[C11] 模块导入与导出
来源：http://nwv.0kj1m.cn

Py:   from module import func
来源：http://ohi.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dmc.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://yzy.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mus.zdbjq.cn

Java: import java.util.List;
来源：http://jbi.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vnx.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://pwl.redwolf501.top

C#:   using System.Text;
来源：http://res.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://fxm.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://wat.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://hva.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://zrh.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://gli.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jwm.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://xoz.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://iug.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cuy.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://irq.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qrs.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vzg.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ofs.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://psl.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://byh.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://eou.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kch.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://bmr.cqqwz.cn

[C14] 泛型函数
来源：http://jst.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://opo.hongshengwenyu.top

PHP:  // 无泛型
来源：http://tle.zhijiandao.cn

JS:   // 无泛型
来源：http://tmi.daria6918.cn


<!-- 参考信息 -->