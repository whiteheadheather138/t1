代发 wailian999

C#:   s.Length
来源：http://vfl.gaohongyu789.top

[A23] 大小写转换
来源：http://rui.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://iui.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yaw.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fhh.bjfxy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yug.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xwm.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ona.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ycr.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uak.jiagoushi.top

[A24] 去除首尾空白
来源：http://nnw.ivvv.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hpu.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jvx.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://omz.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dwm.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bnb.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://sfu.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://afe.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iuz.sjlbkw.cn

[A25] 字符串比较
来源：http://mpq.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://fzw.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aks.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tam.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bhb.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fua.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lif.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kau.yonumen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cza.yonumen.top

[A26] 类型转换总览
来源：http://oqf.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zjy.redwolf501.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jjp.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jyj.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://ape.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wbd.xylfe.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hux.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://inf.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jlp.aibaodan.cn

================================================================================
来源：http://kvd.shzxlz.cn

B. 流程控制
来源：http://pzt.xuetiantiany.cn

================================================================================
来源：http://xpb.yuxming.cn

[B01] 条件判断 if / else
来源：http://qkn.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tqz.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zxz.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sfj.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xid.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cuw.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ahu.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yod.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gws.bbcook.cn

[B02] 多分支 else if / elif
来源：http://ybm.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tgb.gogol.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aai.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exi.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://isn.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mey.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kli.jinqigufen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qkt.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ags.9152youxi.cn

[B03] switch / match / case
来源：http://dsj.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://inp.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wgf.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gez.andypj.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://irs.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nlm.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://krh.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fjd.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yua.fktsv.cn

[B04] for 计数循环
来源：http://zdr.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://wed.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bff.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gxc.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uvy.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fao.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uxq.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://pdh.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qdv.hammf.cn

[B05] 遍历数组 / 列表
来源：http://huz.yfazqb.com

Py:   for item in arr: print(item)
来源：http://idp.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zzw.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://whp.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://gdg.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hmh.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://anu.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://bzg.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://miv.yonumen.top

[B06] 遍历字典 / 对象
来源：http://fcs.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://trq.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xqy.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxg.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nko.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lam.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tqn.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lgi.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sjg.ywan-chungtsiang.top

[B07] while 循环
来源：http://hvq.iojbl.cn

Py:   while i < 10: i += 1
来源：http://zow.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://qye.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://eln.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://neg.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://uqj.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fjh.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://lha.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://cjk.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://iby.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://seg.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://awy.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://lmo.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://uvz.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://tqn.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cja.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://zsc.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://pby.hfpthk.cn

[B09] break 与 continue
来源：http://nje.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fnu.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yzn.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rir.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtg.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qku.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cjr.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xuy.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdv.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://xom.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ths.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tkq.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blg.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zrm.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nxi.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eik.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lbm.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ppf.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://vve.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://kzn.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://irj.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://asj.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eni.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ctp.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uzb.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://mva.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://llv.zhixingplan.top

[B12] 跳出多层循环
来源：http://aop.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lwy.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://voo.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tug.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://isi.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mfj.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hch.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ntk.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wlv.sysykeji.top

[B13] 判断是否为数字
来源：http://xnb.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://suq.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://gjw.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hxz.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lbd.yvedp.cn

Java: x instanceof Number
来源：http://xzi.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vzr.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://ujr.xziqi.cn

C#:   x is int or double or decimal
来源：http://mpk.daria6918.cn

[B14] 判断值是否在集合内
来源：http://eaj.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uke.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cug.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://zro.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://cdz.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pfd.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gry.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://sav.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pgv.sufxvd.cn

[B15] 布尔运算与取反
来源：http://xgf.hammf.cn

Py:   a and b or not c
来源：http://pbc.xziqi.cn

PHP:  $a && $b || !$c
来源：http://wlc.hammf.cn

JS:   a && b || !c
来源：http://iyc.pengpengdd.cyou

TS:   a && b || !c
来源：http://coj.tarul.cn

Java: a && b || !c
来源：http://eia.daria6918.cn

Go:   a && b || !c
来源：http://jlg.vehdjk.com

Ruby: a && b || !c
来源：http://dim.cashguo.top

C#:   a && b || !c
来源：http://opn.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eov.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://wfq.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://esd.xziqi.cn

JS:   if (!data) return;
来源：http://dmb.meibo888.top

TS:   if (!data) return;
来源：http://xdq.chenjidiqi.icu

Java: if (data == null) return;
来源：http://ycw.nanxuanxn.top

Go:   if data == nil { return }
来源：http://dtg.wangdashe.top

Ruby: return if data.nil?
来源：http://qvj.ehwqpu.com

C#:   if (data == null) return;
来源：http://mno.andypj.xyz

================================================================================
来源：http://ajx.ehwqpu.com

C. 函数与作用域
来源：http://beg.ppjwa.cn

================================================================================
来源：http://fiz.aibaodan.cn

[C01] 定义函数
来源：http://mqf.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://yxs.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jpq.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://yad.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fvq.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bnw.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qrm.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://oho.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ust.zdqjudy.top

[C02] 默认参数
来源：http://goj.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://tyc.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://niv.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://hwm.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ztc.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dhe.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rsp.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://kzj.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://axc.yuanzhike.top

[C03] 可变参数
来源：http://hsy.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://lbe.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xuo.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://epf.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwa.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oni.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uvx.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://dtn.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wgg.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://hff.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dhd.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jtt.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vcf.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fge.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://vag.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://ltt.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://yuc.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://hsq.jlsjyb.cn

[C05] 返回多个值
来源：http://eom.0kj1m.cn

Py:   return a, b
来源：http://kjr.nwbrower.top

PHP:  return [$a, $b];
来源：http://lsh.dianchejie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zeh.fzhhl.top

TS:   return { a, b };
来源：http://qly.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bdx.tarul.cn

Go:   return a, b
来源：http://edh.tianlin.xyz

Ruby: return a, b
来源：http://nnz.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://jwd.vehdjk.com

[C06] 匿名函数 / lambda
来源：http://iru.yj202588.top

Py:   square = lambda x: x * x
来源：http://cup.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wuu.yj20258888.top

JS:   const square = x => x * x;
来源：http://mat.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://vyh.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpq.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://rvl.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://gmw.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vtd.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://spp.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sdd.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://end.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uxl.feifeiyinyue.top

TS:   arr.map(String)
来源：http://ylg.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iio.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://htc.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://tgt.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://txr.aibaodan.cn

[C08] 闭包
来源：http://oga.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ljp.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rxg.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vuh.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://frf.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dth.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xgi.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ixd.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://seq.jlsjyb.cn

[C09] 递归
来源：http://vyv.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pft.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wtt.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dci.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qef.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uyl.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://frj.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iuf.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xzq.ydzc1.top

[C10] 变量作用域
来源：http://jta.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lko.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rrx.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ofu.jinghuilouyu.cn

TS:   同 JS
来源：http://nsr.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://uga.jqgfzy.top

Go:   花括号块级作用域
来源：http://jaj.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aat.52xcode.cn

C#:   块级作用域
来源：http://vnk.zhengqikj.top

[C11] 模块导入与导出
来源：http://hnw.iojbl.cn

Py:   from module import func
来源：http://cgv.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zix.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ybw.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uej.tanke756.top

Java: import java.util.List;
来源：http://tct.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kxj.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://wxm.yj202588.top

C#:   using System.Text;
来源：http://pad.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://dsr.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://lpj.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://xha.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://pfk.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://gyy.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eyu.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://bur.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://nbp.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://vum.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://iuk.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wdy.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vcr.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jhi.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qfw.sweek.top


<!-- 参考信息 -->