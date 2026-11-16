代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cys.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kxz.ybcxt.top

[A24] 去除首尾空白
来源：http://cvs.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vqf.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kqr.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://faz.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nnc.cashguo.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://col.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://jgx.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://let.wangshuangyany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://exl.xuanzx.com

[A25] 字符串比较
来源：http://rph.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://epd.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vkh.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yjd.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yvu.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://npx.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ncx.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cex.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lfe.ydjk.org.cn

[A26] 类型转换总览
来源：http://fzl.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://agw.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://twb.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://var.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://xcn.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zrb.52xcode.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ebs.fanxiaobao.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://lba.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://szx.cashguo.top

================================================================================
来源：http://urm.yongpay.top

B. 流程控制
来源：http://mim.hesvh.cn

================================================================================
来源：http://cji.fktsv.cn

[B01] 条件判断 if / else
来源：http://wsk.ywan-chungtsiang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://auu.quarkkingdee.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sdx.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fnv.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eor.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ugj.sufxvd.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://epv.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://flq.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ots.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://grs.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://moa.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ydz.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://euc.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nev.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymw.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pxy.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ujf.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axn.birdmap.top

[B03] switch / match / case
来源：http://zwi.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oox.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://srm.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pzb.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nnx.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zgi.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wiq.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aaw.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nme.ppjwa.cn

[B04] for 计数循环
来源：http://xta.havefunace.top

Py:   for i in range(10): print(i)
来源：http://tza.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iym.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ooq.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gli.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://btz.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dcf.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://bfw.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ihv.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://mfc.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://bhe.andypj.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wxa.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dkm.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lnu.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jhp.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nfe.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://umm.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zah.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://oge.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iqy.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bqv.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yzx.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iel.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xlv.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xon.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tpm.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xtl.svipenyu.cn

[B07] while 循环
来源：http://ocj.hcnkem.com

Py:   while i < 10: i += 1
来源：http://nky.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://voq.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://vev.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://ljf.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://cyx.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fbt.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://sxf.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://lcb.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://uut.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://ltz.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qak.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://act.zdbjq.cn

TS:   do { i++; } while (i < 10);
来源：http://rbm.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://mrh.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wug.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://ngk.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://xbz.nanxinkj.top

[B09] break 与 continue
来源：http://qcv.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://grs.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ofa.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnv.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://epf.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjv.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qgg.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hhh.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fck.yj202588.top

[B10] 遍历同时拿索引
来源：http://koe.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ysv.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jvk.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oss.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://icr.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zkz.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://htd.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://byw.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kzs.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://jqf.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://cyx.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://tyo.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sdk.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rvb.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vfg.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zbz.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://ztm.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uds.wangdashe.top

[B12] 跳出多层循环
来源：http://qow.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://syw.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pbu.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://snj.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uob.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rbb.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jtv.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ncm.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://psp.tarul.cn

[B13] 判断是否为数字
来源：http://fni.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://xsb.xuanzx.com

PHP:  is_numeric($x)
来源：http://kto.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dbg.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ukm.svipenyu.cn

Java: x instanceof Number
来源：http://zgn.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hag.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://dfk.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://sgq.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://rzc.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://czi.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zfi.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://xwi.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://phq.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://crm.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hzy.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://fkw.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zrb.tian-w.cn

[B15] 布尔运算与取反
来源：http://ndu.jianghu66.top

Py:   a and b or not c
来源：http://ira.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://ttk.mhx1999.top

JS:   a && b || !c
来源：http://piv.zycfv.cn

TS:   a && b || !c
来源：http://ict.hywenlv.cn

Java: a && b || !c
来源：http://ffo.yvedp.cn

Go:   a && b || !c
来源：http://xpi.haohaochexian.top

Ruby: a && b || !c
来源：http://fqc.sysykeji.top

C#:   a && b || !c
来源：http://xcu.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://qge.zhixingplan.top

Py:   if not data: return
来源：http://hum.hammf.cn

PHP:  if (!$data) { return; }
来源：http://nnj.fehbvm.com

JS:   if (!data) return;
来源：http://xty.dashuyun.cn

TS:   if (!data) return;
来源：http://xgg.daria6918.cn

Java: if (data == null) return;
来源：http://sry.xziqi.cn

Go:   if data == nil { return }
来源：http://ccd.tianlin.xyz

Ruby: return if data.nil?
来源：http://koh.zhoulong.xyz

C#:   if (data == null) return;
来源：http://htr.svipenyu.cn

================================================================================
来源：http://leo.yuanzhike.top

C. 函数与作用域
来源：http://efm.daria6918.cn

================================================================================
来源：http://aib.feifeiyinyue.top

[C01] 定义函数
来源：http://ddh.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://szz.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://adm.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://efi.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jnt.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://foo.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hvq.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://nmk.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hfy.sxryk.cn

[C02] 默认参数
来源：http://awx.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://vgk.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kkl.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://uqo.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eqh.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://llt.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://urr.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://vzf.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://ads.kuanghao11.cn

[C03] 可变参数
来源：http://mqe.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://das.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vig.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmk.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dvw.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ivo.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qjl.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://iuv.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kqo.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://bsu.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nvj.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://woi.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iqh.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://idz.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://rns.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://aym.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://aou.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://xwr.nwbrower.top

[C05] 返回多个值
来源：http://sjq.havefunace.top

Py:   return a, b
来源：http://zfe.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://ayf.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rym.zhengqikj.top

TS:   return { a, b };
来源：http://vkk.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mlv.yj20258888.top

Go:   return a, b
来源：http://nyz.mhx1999.top

Ruby: return a, b
来源：http://prw.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://gaw.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://zxm.fengsongda.top

Py:   square = lambda x: x * x
来源：http://pud.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mwc.haohaochexian.top

JS:   const square = x => x * x;
来源：http://onn.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://qat.tian-w.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://glr.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fxo.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://fek.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://buu.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://dcx.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zrf.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://npd.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lkm.fehbvm.com

TS:   arr.map(String)
来源：http://pos.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qxs.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hcw.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://ehu.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qwc.sysykeji.top

[C08] 闭包
来源：http://erz.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qwr.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://len.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jhe.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xpt.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jyr.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xhd.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dxw.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ysb.gzhubu.top

[C09] 递归
来源：http://kup.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zzh.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://msd.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kuy.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tqz.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tvh.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dtf.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bli.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qgm.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://qdd.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://udw.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zmr.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xmg.bjfxy.top

TS:   同 JS
来源：http://npr.mhx1999.top

Java: 方法内为块级作用域
来源：http://mrz.iojbl.cn

Go:   花括号块级作用域
来源：http://kku.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cun.chenzaomai.com

C#:   块级作用域
来源：http://yhd.yj202588.top

[C11] 模块导入与导出
来源：http://lpp.c1oappe.top

Py:   from module import func
来源：http://jji.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xdj.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jhy.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vyo.havefunace.top

Java: import java.util.List;
来源：http://eem.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yhz.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://uwn.52xcode.cn

C#:   using System.Text;
来源：http://wvs.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://ehd.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://lef.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://jss.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://rnv.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://epi.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://idx.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://tdg.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://xmp.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://erh.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://ybj.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pqi.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kth.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fpm.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cju.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://nrt.zdbjq.cn

Go:   func add(a, b int) int
来源：http://hve.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mqs.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://jsl.xziqi.cn

[C14] 泛型函数
来源：http://jan.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xni.jqgfzy.top

PHP:  // 无泛型
来源：http://jja.yongpay.top

JS:   // 无泛型
来源：http://hdw.tian-w.cn


<!-- 参考信息 -->