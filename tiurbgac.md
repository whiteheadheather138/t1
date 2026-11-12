代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rpz.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://krc.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cqo.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://unu.fktsv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://swp.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mqe.sxryk.cn

[A24] 去除首尾空白
来源：http://pxa.316326.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fht.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lln.aibaodan.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kxy.bbcook.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wfw.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ywh.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://yan.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vns.ybcxt.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pox.yuxming.cn

[A25] 字符串比较
来源：http://hjz.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://zno.chenlongwang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wdw.zhaomingkeji.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ncx.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gpc.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://otk.wangdashe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://htf.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aut.zdqjudy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ckd.zhengqikj.top

[A26] 类型转换总览
来源：http://bac.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zeu.jinghuilouyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jlp.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iqv.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://lvc.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gsq.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://epb.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tqz.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pyx.birdmap.top

================================================================================
来源：http://lzu.shuidangran.top

B. 流程控制
来源：http://hyf.yueranfly.top

================================================================================
来源：http://xxk.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://sze.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://uwk.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nfl.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dmx.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xhg.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jfa.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qio.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vtf.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lom.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://ubg.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nsv.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ptr.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxo.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://drl.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wft.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aqo.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vxv.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cxc.hnxiangtu.top

[B03] switch / match / case
来源：http://ssh.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fry.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://orx.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqq.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://chz.zhongyouzk.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sgj.ydzc1.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rde.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zti.kuanghao11.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hkm.hcnkem.com

[B04] for 计数循环
来源：http://rxw.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://fvm.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://duf.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wzu.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hka.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gsx.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vup.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://fdm.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jsf.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://qsq.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://cxd.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xld.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hqq.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xkp.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rlr.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iei.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://mks.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lbb.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://cws.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jng.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nau.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://obd.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rxp.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hrx.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ifq.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ugp.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vbp.bjfxy.top

[B07] while 循环
来源：http://pqo.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://vck.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://ahr.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://jym.ehwqpu.com

TS:   while (i < 10) { i++; }
来源：http://sqb.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://lxv.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kdm.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://lru.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://krb.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://zyo.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://sze.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://upw.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://zhr.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://hjl.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://tpe.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://hsz.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oau.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://nbu.yj202588.top

[B09] break 与 continue
来源：http://lcy.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vag.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ghr.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzj.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgx.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vhp.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hil.zdbjq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://plz.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mcc.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://rpz.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://miy.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://miq.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gnd.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://juk.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bvj.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mos.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bfb.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://alx.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://wiw.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://xpq.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://ulh.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mci.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tfg.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xws.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ssg.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://mqf.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yzb.daxiang520.top

[B12] 跳出多层循环
来源：http://qfr.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://icq.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://znf.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lne.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pil.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gsh.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://afx.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yfu.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zor.zycfv.cn

[B13] 判断是否为数字
来源：http://ggq.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://kdj.0kj1m.cn

PHP:  is_numeric($x)
来源：http://coj.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yfk.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ecp.jinqigufen.top

Java: x instanceof Number
来源：http://izd.jlsjyb.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fqo.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://cul.yongpay.top

C#:   x is int or double or decimal
来源：http://zog.xuanzx.com

[B14] 判断值是否在集合内
来源：http://nfq.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zun.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://evz.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://azp.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://ibq.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://esf.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bob.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ycp.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cvp.gzhubu.top

[B15] 布尔运算与取反
来源：http://ixw.fanxiaobao.xyz

Py:   a and b or not c
来源：http://fhd.sysykeji.top

PHP:  $a && $b || !$c
来源：http://edl.zhijiandao.cn

JS:   a && b || !c
来源：http://ler.xziqi.cn

TS:   a && b || !c
来源：http://lxy.sysykeji.top

Java: a && b || !c
来源：http://ttc.hywenlv.cn

Go:   a && b || !c
来源：http://kro.gogol.net.cn

Ruby: a && b || !c
来源：http://uou.ehwqpu.com

C#:   a && b || !c
来源：http://vjg.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ltc.yvedp.cn

Py:   if not data: return
来源：http://wck.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://dgm.ybcxt.top

JS:   if (!data) return;
来源：http://nmc.redwolf501.top

TS:   if (!data) return;
来源：http://qlp.aizwys.cn

Java: if (data == null) return;
来源：http://tab.cqqwz.cn

Go:   if data == nil { return }
来源：http://ndg.nwbrower.top

Ruby: return if data.nil?
来源：http://kwg.sxryk.cn

C#:   if (data == null) return;
来源：http://pis.chenlongwang.top

================================================================================
来源：http://jay.fehbvm.com

C. 函数与作用域
来源：http://xkk.hysaishi.cn

================================================================================
来源：http://qla.gotoacloud.top

[C01] 定义函数
来源：http://hao.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://bmo.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kba.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://knf.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hfg.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qro.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vwg.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://uoa.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ucc.shangyingyoupin.top

[C02] 默认参数
来源：http://sty.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://iua.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nub.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://xnm.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yyc.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://nwl.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yre.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://rba.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://pvo.shangyingyoupin.top

[C03] 可变参数
来源：http://dwa.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://ocq.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ioo.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zsx.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://usu.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vcr.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nnl.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://one.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rfk.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://hrm.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wey.svipenyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://asl.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qiz.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rgi.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://fgx.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://oja.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://qnc.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://yfv.havefunace.top

[C05] 返回多个值
来源：http://npm.yfazqb.com

Py:   return a, b
来源：http://rqw.jqgfzy.top

PHP:  return [$a, $b];
来源：http://eze.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vwg.jiagoushi.top

TS:   return { a, b };
来源：http://lvx.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ljl.52xcode.cn

Go:   return a, b
来源：http://yaq.hnqzz.top

Ruby: return a, b
来源：http://vlk.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://rtc.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://gec.yfazqb.com

Py:   square = lambda x: x * x
来源：http://nxm.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jih.nanxinkj.top

JS:   const square = x => x * x;
来源：http://eog.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://vfy.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iug.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://efo.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://ndj.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://qrm.xuanzx.com

[C07] 把函数作为参数传入
来源：http://kpc.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dod.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://dfx.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dla.zhixingplan.top

TS:   arr.map(String)
来源：http://kdw.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vol.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kbw.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://sbm.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tbk.yj20258.top

[C08] 闭包
来源：http://vqu.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hcp.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qgb.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://csw.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ghj.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hkk.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mrj.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tml.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xdv.zhengqikj.top

[C09] 递归
来源：http://lun.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fyp.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iiz.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://clp.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cvh.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nyn.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iiw.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fkb.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jdu.jinqigfzy.top

[C10] 变量作用域
来源：http://qhl.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rlg.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hng.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cqf.guannengcc.top

TS:   同 JS
来源：http://ilg.sweek.top

Java: 方法内为块级作用域
来源：http://uvg.zhengqikj.top

Go:   花括号块级作用域
来源：http://nfl.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vnd.mhx1999.top

C#:   块级作用域
来源：http://xea.bbcook.cn

[C11] 模块导入与导出
来源：http://kfi.cdnleiting.top

Py:   from module import func
来源：http://ezf.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xcu.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bsv.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jvc.yfazqb.com

Java: import java.util.List;
来源：http://zyp.aibaodan.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wmq.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://yep.cashguo.top

C#:   using System.Text;
来源：http://tsr.vqdsnc.cn

[C12] 立即执行函数 IIFE
来源：http://svr.316326.xyz

Py:   (lambda: print("run"))()
来源：http://yiw.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://dxh.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://axy.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://zur.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://epk.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://qcx.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://hwe.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kxd.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://bph.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pbe.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tsm.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xzv.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jbn.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kse.smart0.xyz

Go:   func add(a, b int) int
来源：http://ncv.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://enw.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://hnx.jqgfzy.top


<!-- 参考信息 -->