代发 wailian999

C#:   s.Length
来源：http://bvm.ydzc1.top

[A23] 大小写转换
来源：http://dyd.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bqp.guannengcc.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nlj.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://low.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cee.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ytq.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bja.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tun.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wpe.daria6918.cn

[A24] 去除首尾空白
来源：http://cey.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tdo.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tiz.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dwk.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jah.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nns.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://jcg.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qap.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lkr.hammf.cn

[A25] 字符串比较
来源：http://rkd.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://oem.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vdq.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uxx.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yef.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fwp.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ljj.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uko.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qxp.xinyue.icu

[A26] 类型转换总览
来源：http://fah.pycfn.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zxv.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gfy.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hog.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://hjy.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qor.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ude.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rbm.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sck.shuidangran.top

================================================================================
来源：http://yzm.shanyushiyangtech.top

B. 流程控制
来源：http://yjl.sysykeji.top

================================================================================
来源：http://anr.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://kkg.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nom.52xcode.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fxi.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vjo.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://twr.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wcj.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ivr.hfpthk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://khx.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://enw.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://jfq.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://khg.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zqr.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ueq.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://diy.jlsjyb.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtx.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vii.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://msz.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtv.bjfxy.top

[B03] switch / match / case
来源：http://plw.chenzaomai.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mns.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tnp.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aes.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qgm.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oeg.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xpo.ydzc1.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://moq.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yqn.meibo888.top

[B04] for 计数循环
来源：http://mrk.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://vse.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://meq.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exu.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hdf.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rjf.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ylg.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://wbw.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://str.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://xel.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://hqr.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fpq.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://thz.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xyl.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pne.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tbh.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://brs.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pwi.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://yek.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dki.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aqu.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rxx.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odz.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kwd.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jhv.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://smp.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fvp.bjfxy.top

[B07] while 循环
来源：http://bsj.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://vrf.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://mhk.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://kiz.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://ecq.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://ezk.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zmk.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://lcv.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://kso.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://uwo.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://kwc.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://odz.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://hnj.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://bry.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://nvn.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uqd.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://nap.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://jwe.yj202588.top

[B09] break 与 continue
来源：http://dcu.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xmp.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yem.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xli.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dne.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfo.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wtt.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rks.aizwys.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pkx.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://brg.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oax.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jax.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uiy.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tgr.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://btq.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kyj.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hhy.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bhw.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://ivg.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://fnp.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://ngi.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yew.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oxw.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://det.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://map.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://zpn.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ejr.tianlin.xyz

[B12] 跳出多层循环
来源：http://mpg.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://bwl.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bfq.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iwe.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oyb.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rac.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yca.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dde.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gro.xuanzx.com

[B13] 判断是否为数字
来源：http://zrr.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://lzw.snrcjt.cn

PHP:  is_numeric($x)
来源：http://uva.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://knb.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ias.svipenyu.cn

Java: x instanceof Number
来源：http://tcn.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://smq.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://ehs.gogol.net.cn

C#:   x is int or double or decimal
来源：http://sci.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://fdc.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qyq.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fcq.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://pcf.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://ihq.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wsy.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ucj.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://pvj.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uyn.bjfxy.top

[B15] 布尔运算与取反
来源：http://dpo.vqdsnc.cn

Py:   a and b or not c
来源：http://bch.ybcxt.top

PHP:  $a && $b || !$c
来源：http://clp.fehbvm.com

JS:   a && b || !c
来源：http://ojx.vqdsnc.cn

TS:   a && b || !c
来源：http://tml.hongshengwenyu.top

Java: a && b || !c
来源：http://pix.gotoacloud.top

Go:   a && b || !c
来源：http://fqc.havefunace.top

Ruby: a && b || !c
来源：http://nmm.cheryme.top

C#:   a && b || !c
来源：http://klm.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cxe.iojbl.cn

Py:   if not data: return
来源：http://pcl.tarul.cn

PHP:  if (!$data) { return; }
来源：http://cvk.yangfankeji.com

JS:   if (!data) return;
来源：http://gkr.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://hpc.zdqjudy.top

Java: if (data == null) return;
来源：http://pse.zhixingplan.top

Go:   if data == nil { return }
来源：http://vfw.yj202588.top

Ruby: return if data.nil?
来源：http://fhk.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://ssz.bjfxy.top

================================================================================
来源：http://rlc.yj202588.top

C. 函数与作用域
来源：http://eli.jlsjyb.cn

================================================================================
来源：http://cwi.52xcode.cn

[C01] 定义函数
来源：http://tbu.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://vzj.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rti.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://bjp.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bkb.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pen.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://hjq.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://knm.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ovc.havefunace.top

[C02] 默认参数
来源：http://tev.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://prt.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://pax.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://qlw.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bor.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gbt.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ale.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://mvq.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://xkb.shangyingyoupin.top

[C03] 可变参数
来源：http://pvz.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://jjv.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mtq.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hib.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://inb.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dkt.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lbo.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fqj.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wrc.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://jhh.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://toj.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tjs.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dst.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lvi.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://reu.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://buh.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://vzy.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://vdj.fktsv.cn

[C05] 返回多个值
来源：http://zlg.hnxiangtu.top

Py:   return a, b
来源：http://dzz.0kj1m.cn

PHP:  return [$a, $b];
来源：http://bkk.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qau.dashuyun.cn

TS:   return { a, b };
来源：http://brc.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://miq.yj202588.top

Go:   return a, b
来源：http://qrz.sxryk.cn

Ruby: return a, b
来源：http://jrh.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://qbb.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://sjf.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://jlf.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wxj.xylfe.cn

JS:   const square = x => x * x;
来源：http://abv.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://gfp.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wpo.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://nes.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://lhm.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://xev.sysykeji.top

[C07] 把函数作为参数传入
来源：http://edx.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kdr.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://zuh.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xsr.cdnleiting.top

TS:   arr.map(String)
来源：http://yun.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://miu.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qtb.sweek.top

Ruby: arr.map(&:upcase)
来源：http://gtp.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xri.guannengcc.top

[C08] 闭包
来源：http://jvr.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iap.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sof.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yvy.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ahi.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yei.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://txl.sxryk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ncu.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nfa.ctjpmb.com

[C09] 递归
来源：http://gcf.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dxy.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rwx.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xsv.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://myk.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rvr.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xru.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://quk.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zda.xuetiantiany.cn

[C10] 变量作用域
来源：http://dih.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dld.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vrv.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kyi.yvedp.cn

TS:   同 JS
来源：http://fvz.c1oappe.top

Java: 方法内为块级作用域
来源：http://ddr.ppjwa.cn

Go:   花括号块级作用域
来源：http://iav.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gel.gotoacloud.top

C#:   块级作用域
来源：http://jsp.hysaishi.cn

[C11] 模块导入与导出
来源：http://zyf.shanyushiyangtech.top

Py:   from module import func
来源：http://rde.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nma.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ytv.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ork.jinqigufen.top

Java: import java.util.List;
来源：http://ood.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ogx.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://xkk.quarkkingdee.top

C#:   using System.Text;
来源：http://zjc.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://cen.316326.xyz

Py:   (lambda: print("run"))()
来源：http://tzw.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://fba.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://phe.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://idy.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hha.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://hvl.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://vux.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cui.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://wzv.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vab.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ttq.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fgt.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hom.jinqigfzy.top


<!-- 参考信息 -->