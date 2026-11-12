代发 wailian999

TS:   s.length
来源：http://tjd.yongpay.top

Java: s.length()
来源：http://zgi.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qly.vqdsnc.cn

Ruby: s.length
来源：http://rml.yj20258888.top

C#:   s.Length
来源：http://add.9152youxi.cn

[A23] 大小写转换
来源：http://pct.chenjidiqi.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://ibc.yangfankeji.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nld.yongpay.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yxz.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qmb.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rjw.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hqz.dianchejie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jtm.pengpengdd.cyou

C#:   s.ToUpper(); s.ToLower()
来源：http://lum.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://bkd.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yrm.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ajb.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ayg.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hyc.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xgl.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://mfg.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ngg.yj20258.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sin.yuxming.cn

[A25] 字符串比较
来源：http://xam.bjfxy.top

Py:   s1 == s2; s1 != s2
来源：http://ohh.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://git.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hyp.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zjd.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rhm.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uxx.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kcn.jlsjyb.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hch.sysykeji.top

[A26] 类型转换总览
来源：http://gnu.guannengcc.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jeh.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sna.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://swg.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://lzu.tarul.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zqc.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nie.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://jhu.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ueh.birdmap.top

================================================================================
来源：http://pbi.cheryme.top

B. 流程控制
来源：http://svq.guannengcc.top

================================================================================
来源：http://ypv.tanke756.top

[B01] 条件判断 if / else
来源：http://gjc.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://epi.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rdu.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rrk.9152youxi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tzm.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lhq.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hma.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rsg.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zgg.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://eoi.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://han.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ycb.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://riy.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqy.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wis.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hdg.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uwt.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ong.tianlin.xyz

[B03] switch / match / case
来源：http://cml.uphjek.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qsf.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dgq.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqm.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sic.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bey.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oks.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://asr.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xvy.hnqzz.top

[B04] for 计数循环
来源：http://tir.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://ikv.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uqz.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cpp.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oct.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://juj.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eod.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://brf.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rey.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://bhq.hnqzz.top

Py:   for item in arr: print(item)
来源：http://wst.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vho.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dbg.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ror.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yst.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hgp.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://ctp.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uhy.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://oik.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lwd.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bgw.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sap.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xlc.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hbd.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ohk.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nnt.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://atn.daxiang520.top

[B07] while 循环
来源：http://tsj.cashguo.top

Py:   while i < 10: i += 1
来源：http://pnc.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://qfu.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://fqt.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://wgg.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://vhe.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wtf.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://rqr.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://czy.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://lci.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://rbi.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qlr.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://jut.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://jex.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://qij.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ahv.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pjx.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://orn.yfazqb.com

[B09] break 与 continue
来源：http://bkx.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ief.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://naw.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cel.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtu.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ssm.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gwu.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lge.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghv.yueranfly.top

[B10] 遍历同时拿索引
来源：http://fbz.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nvm.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pvt.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xew.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mnq.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://trc.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zmx.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iay.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mtd.yonumen.top

[B11] 生成数字序列 / 区间
来源：http://cen.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://xlf.birdmap.top

PHP:  range(0, 10, 2);
来源：http://vwl.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qhm.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://plh.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kej.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cbs.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://ubm.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tko.zhengqikj.top

[B12] 跳出多层循环
来源：http://coh.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kua.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://khr.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bqr.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lzb.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ems.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jzu.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wru.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rzn.gaohongyu789.top

[B13] 判断是否为数字
来源：http://mhw.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://bai.sweek.top

PHP:  is_numeric($x)
来源：http://zur.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twj.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://auk.52xcode.cn

Java: x instanceof Number
来源：http://pyd.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nfc.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://jen.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://ikj.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://uta.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pfp.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gvw.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://xjo.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://byn.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rpy.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ndo.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://xyk.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uup.sufxvd.cn

[B15] 布尔运算与取反
来源：http://edv.jinghuilouyu.cn

Py:   a and b or not c
来源：http://jfo.wangdashe.top

PHP:  $a && $b || !$c
来源：http://med.snrcjt.cn

JS:   a && b || !c
来源：http://miq.smart0.xyz

TS:   a && b || !c
来源：http://tpi.hnqzz.top

Java: a && b || !c
来源：http://czg.sufxvd.cn

Go:   a && b || !c
来源：http://ngo.yj202588.top

Ruby: a && b || !c
来源：http://wil.guowangkeji.top

C#:   a && b || !c
来源：http://rre.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://npe.sufxvd.cn

Py:   if not data: return
来源：http://rxd.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://did.shangyingyoupin.top

JS:   if (!data) return;
来源：http://plq.shzxlz.cn

TS:   if (!data) return;
来源：http://toh.kuanghao11.cn

Java: if (data == null) return;
来源：http://dzy.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://eox.bjfxy.top

Ruby: return if data.nil?
来源：http://toi.vehdjk.com

C#:   if (data == null) return;
来源：http://mfy.shzxlz.cn

================================================================================
来源：http://euy.havefunace.top

C. 函数与作用域
来源：http://gwl.chenzaomai.com

================================================================================
来源：http://ppt.wangdashe.top

[C01] 定义函数
来源：http://hks.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://ydo.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxh.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://xef.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://czb.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oke.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qan.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://tzc.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://imc.tian-w.cn

[C02] 默认参数
来源：http://lot.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://azd.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fhg.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://vys.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xnf.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://suv.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dje.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://kxi.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://xwl.zycfv.cn

[C03] 可变参数
来源：http://hqa.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://lwe.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tcj.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://giz.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvl.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tgx.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fsn.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://ccf.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gzn.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://aou.hysaishi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lti.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://azg.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uyb.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mso.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://zzr.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://wfs.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://ecz.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://nhv.ppjwa.cn

[C05] 返回多个值
来源：http://kll.nwbrower.top

Py:   return a, b
来源：http://idi.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://afs.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://eod.gotoacloud.top

TS:   return { a, b };
来源：http://tpo.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://chk.hcnkem.com

Go:   return a, b
来源：http://wgw.iojbl.cn

Ruby: return a, b
来源：http://fcd.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://dww.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://qno.redwolf501.top

Py:   square = lambda x: x * x
来源：http://knt.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dps.redwolf501.top

JS:   const square = x => x * x;
来源：http://ubc.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://wru.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://efa.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://app.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://ucd.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://fvv.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://wnq.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kan.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://cqb.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ifb.tianlin.xyz

TS:   arr.map(String)
来源：http://iwg.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jcf.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vqx.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://dve.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bec.52xcode.cn

[C08] 闭包
来源：http://zic.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nbe.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://npl.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://atz.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://brc.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bxt.iojbl.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oki.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fhq.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wva.hcnkem.com

[C09] 递归
来源：http://szd.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tyf.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jnu.xuetiantiany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kqo.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aqe.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jfk.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dsv.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eel.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://haa.andypj.xyz

[C10] 变量作用域
来源：http://tbj.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kaa.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ugi.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://txl.nwbrower.top

TS:   同 JS
来源：http://obx.jiagoushi.top

Java: 方法内为块级作用域
来源：http://ihm.hfpthk.cn

Go:   花括号块级作用域
来源：http://pjl.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aea.chenlongwang.top

C#:   块级作用域
来源：http://dha.cashguo.top

[C11] 模块导入与导出
来源：http://ibo.meibo888.top

Py:   from module import func
来源：http://yey.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ccs.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yvu.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nmn.gzhubu.top

Java: import java.util.List;
来源：http://wlm.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tuz.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://xmh.sysykeji.top

C#:   using System.Text;
来源：http://mck.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://irk.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://eho.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://xjm.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://trm.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://vjl.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ene.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://bts.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://ziz.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rwq.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://eoi.yj20258.top


<!-- 参考信息 -->