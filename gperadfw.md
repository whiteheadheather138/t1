代发 wailian999

TS:   s.length
来源：http://pbd.zhiwuduotai.top

Java: s.length()
来源：http://bcw.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ifz.yj20258888.top

Ruby: s.length
来源：http://tfb.kuanghao11.cn

C#:   s.Length
来源：http://bas.cucudq.cn

[A23] 大小写转换
来源：http://vfb.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xbf.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cru.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nrn.sweek.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgw.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://czy.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zzf.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ghw.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://khu.yongpay.top

[A24] 去除首尾空白
来源：http://zoi.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hcc.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rlk.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oua.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wnz.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dvt.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://ubs.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hbi.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://idk.zhiwuduotai.top

[A25] 字符串比较
来源：http://pal.birdmap.top

Py:   s1 == s2; s1 != s2
来源：http://org.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kpu.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jld.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vwz.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tdl.sysykeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jiw.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://eyi.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ivg.daxiang520.top

[A26] 类型转换总览
来源：http://ejq.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cxz.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wfu.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tjl.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://pml.fktsv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://upx.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cuu.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://svo.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://neo.redwolf501.top

================================================================================
来源：http://nqy.havefunace.top

B. 流程控制
来源：http://tnp.shanyushiyangtech.top

================================================================================
来源：http://psa.xinyue.icu

[B01] 条件判断 if / else
来源：http://cnm.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bwo.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ndu.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://swv.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kir.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vnv.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gmc.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oqp.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ndz.birdmap.top

[B02] 多分支 else if / elif
来源：http://agy.yj20258.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zbz.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rmg.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfi.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sjr.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbz.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rgz.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nlz.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yux.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://lll.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qtc.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cff.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gxe.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fwo.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aid.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fou.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kwm.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uuy.zdqjudy.top

[B04] for 计数循环
来源：http://kpt.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://ziy.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gid.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jns.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gpk.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uxe.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rmp.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://suf.zhengqikj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iwp.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://hcu.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://yzv.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://chb.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qld.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://bum.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://bpe.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bjr.zhengqikj.top

Ruby: arr.each { |item| puts item }
来源：http://qbn.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tyv.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://big.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uvr.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qul.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cem.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hbs.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://btc.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jnq.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ufr.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xug.yanxiufei.cn

[B07] while 循环
来源：http://agd.yueranfly.top

Py:   while i < 10: i += 1
来源：http://xhn.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://mqp.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://bcy.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://cpp.yj20258.top

Java: while (i < 10) { i++; }
来源：http://jhz.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yef.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://fks.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://lvn.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://awe.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://zuk.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fks.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://gmx.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://jvt.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://jro.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ubb.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://pxn.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://eup.cheryme.top

[B09] break 与 continue
来源：http://vru.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://brn.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qyx.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbx.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cza.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qph.chenzaomai.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mhr.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dzj.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blt.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://afi.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wie.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pjl.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dbf.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://edj.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bfo.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hfo.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zhu.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kyk.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://aaq.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://dfi.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://tpg.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cwb.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qna.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gpn.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jvv.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://gzt.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gnv.kuanghao11.cn

[B12] 跳出多层循环
来源：http://qdw.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hdn.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vqg.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://agu.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uyp.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pov.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qih.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jsv.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://klx.hnxiangtu.top

[B13] 判断是否为数字
来源：http://tel.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://zga.gogol.net.cn

PHP:  is_numeric($x)
来源：http://tdh.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvw.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://raz.xinyue.icu

Java: x instanceof Number
来源：http://cjx.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dgf.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://wrv.yuxming.cn

C#:   x is int or double or decimal
来源：http://how.fzhhl.top

[B14] 判断值是否在集合内
来源：http://bkj.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jep.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xqi.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://fmy.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://aja.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://gqh.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tjg.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zsf.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mdg.chenlongwang.top

[B15] 布尔运算与取反
来源：http://jul.svipenyu.cn

Py:   a and b or not c
来源：http://xpc.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://hvu.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://aka.hongshengwenyu.top

TS:   a && b || !c
来源：http://mvl.9152youxi.cn

Java: a && b || !c
来源：http://szj.ctjpmb.com

Go:   a && b || !c
来源：http://toi.pengpengdd.cyou

Ruby: a && b || !c
来源：http://pwz.chenjidiqi.icu

C#:   a && b || !c
来源：http://uct.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://sqi.tarul.cn

Py:   if not data: return
来源：http://xmn.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://emn.bbcook.cn

JS:   if (!data) return;
来源：http://cvc.hysaishi.cn

TS:   if (!data) return;
来源：http://swx.bjfxy.top

Java: if (data == null) return;
来源：http://urb.jqgufenzy.top

Go:   if data == nil { return }
来源：http://uaa.zhijiandao.cn

Ruby: return if data.nil?
来源：http://bbt.daxiang520.top

C#:   if (data == null) return;
来源：http://svm.epnwcf.com

================================================================================
来源：http://spb.fktsv.cn

C. 函数与作用域
来源：http://emt.daria6918.cn

================================================================================
来源：http://msc.yvedp.cn

[C01] 定义函数
来源：http://pxt.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://ccd.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zak.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://nae.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://krn.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pug.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nyo.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://psd.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qic.shangyingyoupin.top

[C02] 默认参数
来源：http://psb.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://iae.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vqk.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://zxw.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cvz.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://skx.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wob.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://jit.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://zok.svipenyu.cn

[C03] 可变参数
来源：http://ile.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://jzz.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mme.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lbq.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sdu.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://axv.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pvz.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://egk.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://krz.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://vho.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xqw.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nil.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zvf.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aje.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://ipj.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://lqo.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://okk.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://ktx.wangdashe.top

[C05] 返回多个值
来源：http://mkk.ppjwa.cn

Py:   return a, b
来源：http://oke.havefunace.top

PHP:  return [$a, $b];
来源：http://xvn.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ytu.ctjpmb.com

TS:   return { a, b };
来源：http://vqv.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qcg.hcnkem.com

Go:   return a, b
来源：http://uil.ctjpmb.com

Ruby: return a, b
来源：http://syk.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://sbs.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://sye.tian-w.cn

Py:   square = lambda x: x * x
来源：http://mnz.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gcx.xziqi.cn

JS:   const square = x => x * x;
来源：http://yiq.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://heq.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cpv.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://ars.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://swb.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://crl.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://dsq.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vbn.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://rri.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sxk.xuanzx.com

TS:   arr.map(String)
来源：http://mhb.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nuw.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rqv.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://ebr.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xzg.cucudq.cn

[C08] 闭包
来源：http://scf.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bkr.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ujx.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ufx.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lrp.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yrk.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gmt.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cal.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zfc.wangshuangyany.cn

[C09] 递归
来源：http://srz.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hsh.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://emd.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bgi.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bpb.fktsv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vef.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vlu.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://imu.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jmo.yj20258.top

[C10] 变量作用域
来源：http://hjp.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sbd.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yyt.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://njn.yonumen.top

TS:   同 JS
来源：http://qvo.ivvv.top

Java: 方法内为块级作用域
来源：http://ycd.kuanghao11.cn

Go:   花括号块级作用域
来源：http://jlw.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://afk.dianchejie.cn

C#:   块级作用域
来源：http://nww.yj20258.top

[C11] 模块导入与导出
来源：http://xfb.jqgfzy.top

Py:   from module import func
来源：http://rxu.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://duf.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yzi.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blg.hywenlv.cn

Java: import java.util.List;
来源：http://xnt.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xnm.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://rpp.yuanzhike.top

C#:   using System.Text;
来源：http://dle.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://wbj.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://gcs.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://rth.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://aid.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://dkb.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fho.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://bpb.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://ekq.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dkn.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://mgw.cdnleiting.top


<!-- 参考信息 -->