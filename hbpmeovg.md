代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://jur.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ptk.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://hlx.fanxiaobao.xyz

C#:   3.14159.ToString("F2")
来源：http://xnh.iojbl.cn

[A22] 获取字符串长度
来源：http://iyv.andypj.xyz

Py:   len(s)
来源：http://udi.nanxinkj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aoi.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tcw.pengpengdd.cyou

TS:   s.length
来源：http://dbq.xuetiantiany.cn

Java: s.length()
来源：http://pht.zhengqikj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ahp.bbcook.cn

Ruby: s.length
来源：http://gsm.yangfankeji.com

C#:   s.Length
来源：http://tre.ybcxt.top

[A23] 大小写转换
来源：http://zfh.hywenlv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qvy.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kir.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oke.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fof.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fsr.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wef.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lgc.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://roc.yueranfly.top

[A24] 去除首尾空白
来源：http://lxc.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wub.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tjh.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://irb.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bfq.cashguo.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zwv.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://kro.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ifa.hywenlv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cbg.ydjk.org.cn

[A25] 字符串比较
来源：http://zhe.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://lsv.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bbk.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kks.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vjt.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dpx.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jxh.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://icb.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xki.ydzc1.top

[A26] 类型转换总览
来源：http://toe.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ysu.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yxc.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ckt.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://cor.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hrh.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jpv.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zyc.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uvw.hammf.cn

================================================================================
来源：http://vat.fzhhl.top

B. 流程控制
来源：http://orn.xinyue.icu

================================================================================
来源：http://xti.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://mys.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://swk.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://omb.quarkkingdee.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xch.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rat.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://pkh.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pxi.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ebl.tianlin.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bni.redwolf501.top

[B02] 多分支 else if / elif
来源：http://usb.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nkk.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fiq.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmp.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hsb.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdr.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qce.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://suk.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnt.smart0.xyz

[B03] switch / match / case
来源：http://zpd.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uem.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://weh.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://giu.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwf.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://drx.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pif.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://som.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xab.yangfankeji.com

[B04] for 计数循环
来源：http://jjq.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://ida.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wsa.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://muw.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yqw.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rdw.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pkb.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://gix.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ovt.birdmap.top

[B05] 遍历数组 / 列表
来源：http://zgv.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://sux.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://upv.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pdr.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ley.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xsg.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kxu.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://boj.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hrt.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://zuw.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zml.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ckj.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zik.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://asy.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://chq.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cjb.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rhw.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pcr.cucudq.cn

[B07] while 循环
来源：http://vqs.yj20258.top

Py:   while i < 10: i += 1
来源：http://kkn.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://ljr.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://imj.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://avd.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://huc.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ygo.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://hop.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://eut.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://kcn.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://bgs.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pml.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://uqm.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://cib.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://pbj.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://cpd.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://cjx.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://mrm.fanxiaobao.xyz

[B09] break 与 continue
来源：http://sjv.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fea.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iee.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jog.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tgn.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sny.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lje.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lpc.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpm.xuanzx.com

[B10] 遍历同时拿索引
来源：http://suk.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yuo.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jzk.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vix.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vvb.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lvu.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mpo.birdmap.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tpl.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zpw.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://iei.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://krv.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://kmf.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uew.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://irc.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bnm.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cej.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://hvb.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rim.hammf.cn

[B12] 跳出多层循环
来源：http://ieh.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://foc.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eat.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dze.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gqy.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sov.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cyk.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ytr.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mmz.cqqwz.cn

[B13] 判断是否为数字
来源：http://ztw.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://xwf.yj20258888.top

PHP:  is_numeric($x)
来源：http://siz.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ggp.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmx.hnqzz.top

Java: x instanceof Number
来源：http://quh.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sot.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://srq.ctjpmb.com

C#:   x is int or double or decimal
来源：http://sic.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://yxy.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oqc.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wdb.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://fah.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ied.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fye.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tgu.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://muu.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ncx.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://ehl.feifeiyinyue.top

Py:   a and b or not c
来源：http://mix.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://mwv.316326.xyz

JS:   a && b || !c
来源：http://ecr.smart0.xyz

TS:   a && b || !c
来源：http://jko.pycfn.com

Java: a && b || !c
来源：http://qqg.zhoulong.xyz

Go:   a && b || !c
来源：http://xkx.hnxiangtu.top

Ruby: a && b || !c
来源：http://xba.aibaodan.cn

C#:   a && b || !c
来源：http://loy.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://ycc.yj20258888.top

Py:   if not data: return
来源：http://kze.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://psb.wangdashe.top

JS:   if (!data) return;
来源：http://rxe.jiagoushi.top

TS:   if (!data) return;
来源：http://gqb.andypj.xyz

Java: if (data == null) return;
来源：http://zur.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://jls.ydzc1.top

Ruby: return if data.nil?
来源：http://jnz.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://yzc.daxiang520.top

================================================================================
来源：http://woa.fengsongda.top

C. 函数与作用域
来源：http://qbw.316326.xyz

================================================================================
来源：http://vqf.zdbjq.cn

[C01] 定义函数
来源：http://esz.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://nbx.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfr.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://izy.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fnw.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wux.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://dre.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://uxc.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://geb.hysaishi.cn

[C02] 默认参数
来源：http://oyx.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://uto.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://twu.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://jsm.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pzr.mhx1999.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iha.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vng.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://nxe.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://unr.yj202588.top

[C03] 可变参数
来源：http://osc.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://edq.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yus.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ijx.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://chw.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mga.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kve.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qqk.dashuyun.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uwo.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://anl.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zlh.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sak.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eqb.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xkf.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://yac.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://wuh.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://kje.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://otk.redwolf501.top

[C05] 返回多个值
来源：http://dxk.guannengcc.top

Py:   return a, b
来源：http://wit.bjfxy.top

PHP:  return [$a, $b];
来源：http://avs.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ntb.yueranfly.top

TS:   return { a, b };
来源：http://ztr.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vyo.yj20258.top

Go:   return a, b
来源：http://vkq.ehwqpu.com

Ruby: return a, b
来源：http://gvx.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://vel.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://ahx.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://zwj.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cxs.jyoumei.cn

JS:   const square = x => x * x;
来源：http://ahm.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://sah.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uuf.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xun.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://lyr.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://jqy.hcnkem.com

[C07] 把函数作为参数传入
来源：http://zdd.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iat.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://vsl.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ttj.gogol.net.cn

TS:   arr.map(String)
来源：http://cuk.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lgr.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nfk.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://psz.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dpk.yuanzhike.top

[C08] 闭包
来源：http://bno.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dlo.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://opf.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://btj.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qjj.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jbv.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://plj.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gdc.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wua.cashguo.top

[C09] 递归
来源：http://bxc.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mzu.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://afz.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mue.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oxs.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eay.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vyb.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ctq.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zmt.jiagoushi.top

[C10] 变量作用域
来源：http://llx.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://net.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dcs.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mfr.andypj.xyz

TS:   同 JS
来源：http://plr.xuanzx.com

Java: 方法内为块级作用域
来源：http://bkg.yongpay.top

Go:   花括号块级作用域
来源：http://lqu.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hua.xinyue.icu

C#:   块级作用域
来源：http://eyb.dianchejie.cn

[C11] 模块导入与导出
来源：http://vse.andypj.xyz

Py:   from module import func
来源：http://owr.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fif.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://slq.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://etd.hnqzz.top

Java: import java.util.List;
来源：http://ujg.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ely.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://qoz.0kj1m.cn

C#:   using System.Text;
来源：http://unv.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://tqa.sweek.top

Py:   (lambda: print("run"))()
来源：http://via.jinghuilouyu.cn


<!-- 参考信息 -->