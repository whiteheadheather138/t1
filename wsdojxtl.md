代发 wailian999

TS:   s.length
来源：http://ech.jinqigfzy.top

Java: s.length()
来源：http://iju.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dwz.chenzaomai.com

Ruby: s.length
来源：http://aoc.daria6918.cn

C#:   s.Length
来源：http://dks.guowangkeji.top

[A23] 大小写转换
来源：http://rmn.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://eku.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ggt.cqqwz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nfe.wangshuangyany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yzs.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dqs.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vkq.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://atb.jqgfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rfe.fehbvm.com

[A24] 去除首尾空白
来源：http://zaw.ivvv.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nyo.snrcjt.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bng.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bkx.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tqa.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://shr.aizwys.cn

Go:   strings.TrimSpace(s)
来源：http://xjw.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://geu.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wjf.hfpthk.cn

[A25] 字符串比较
来源：http://xpa.zhixingplan.top

Py:   s1 == s2; s1 != s2
来源：http://kms.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bkd.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xtq.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tdv.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jxy.jlsjyb.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fai.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://spu.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hzg.zycfv.cn

[A26] 类型转换总览
来源：http://mtp.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gle.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://brl.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ebd.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://bwn.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://svu.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sic.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sqj.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vgo.wangshuangyany.cn

================================================================================
来源：http://epk.zdqjudy.top

B. 流程控制
来源：http://ggw.yuxming.cn

================================================================================
来源：http://hci.xinyue.icu

[B01] 条件判断 if / else
来源：http://bex.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kfi.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rox.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kfv.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cwj.yonumen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gsu.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ooe.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qvo.jyoumei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qzi.zycfv.cn

[B02] 多分支 else if / elif
来源：http://fqi.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fvp.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ddc.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezh.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mso.yj202588.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mwe.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rfn.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hhs.daria6918.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfl.jqgfzy.top

[B03] switch / match / case
来源：http://iqh.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ebb.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kel.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://prn.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vmm.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dft.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nwa.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dke.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dge.yj20258.top

[B04] for 计数循环
来源：http://qdk.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://rdd.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qvq.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wma.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://smy.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pnl.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ybc.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://fiv.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ljv.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://pfh.yongpay.top

Py:   for item in arr: print(item)
来源：http://ejw.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cnv.jinqigfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fqo.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ohe.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vwb.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qgv.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://pux.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xrh.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://igp.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ywd.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xxb.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pvn.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://czr.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wog.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cty.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ddb.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sdk.ctjpmb.com

[B07] while 循环
来源：http://upr.yj20258.top

Py:   while i < 10: i += 1
来源：http://eww.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ejc.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://hsr.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://lmh.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://mkq.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ejj.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://euc.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://skz.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://xzc.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://ndc.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pzy.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://wcs.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://rld.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://vom.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jre.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yja.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://dvm.smart0.xyz

[B09] break 与 continue
来源：http://cnv.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nhv.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pkc.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smj.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnc.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djh.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://szq.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lpp.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqy.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://puk.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dsn.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dds.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nux.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gzw.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fiy.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uha.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rgt.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yox.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://jvb.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://alk.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://hvj.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fdt.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bhm.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uqd.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hjr.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://ptf.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mdj.tanke756.top

[B12] 跳出多层循环
来源：http://okt.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mex.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fzi.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpj.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eqq.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ksw.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aev.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rod.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ffk.jyoumei.cn

[B13] 判断是否为数字
来源：http://ejc.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://bpj.vehdjk.com

PHP:  is_numeric($x)
来源：http://zvi.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://exe.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zgw.hnqzz.top

Java: x instanceof Number
来源：http://uru.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pqk.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://zda.zhixingplan.top

C#:   x is int or double or decimal
来源：http://svd.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://jra.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zft.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rjz.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://uvz.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://zgg.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dja.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zzu.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://afx.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ego.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://yim.cashguo.top

Py:   a and b or not c
来源：http://cdi.hnqzz.top

PHP:  $a && $b || !$c
来源：http://qem.guannengcc.top

JS:   a && b || !c
来源：http://ueh.birdmap.top

TS:   a && b || !c
来源：http://vai.kuanghao11.cn

Java: a && b || !c
来源：http://kcc.chenzaomai.com

Go:   a && b || !c
来源：http://sca.ppjwa.cn

Ruby: a && b || !c
来源：http://mtb.svipenyu.cn

C#:   a && b || !c
来源：http://ngp.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://czm.shuidangran.top

Py:   if not data: return
来源：http://rfg.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://vhh.quarkkingdee.top

JS:   if (!data) return;
来源：http://qzw.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://ugw.yfazqb.com

Java: if (data == null) return;
来源：http://duq.aizwys.cn

Go:   if data == nil { return }
来源：http://nli.yonumen.top

Ruby: return if data.nil?
来源：http://phz.svipenyu.cn

C#:   if (data == null) return;
来源：http://dwb.iojbl.cn

================================================================================
来源：http://qui.snrcjt.cn

C. 函数与作用域
来源：http://fmp.xziqi.cn

================================================================================
来源：http://pfa.xuanzx.com

[C01] 定义函数
来源：http://izd.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://cxb.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jti.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://ovp.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tlu.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jkh.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://pou.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://vnm.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://psx.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://xoh.cashguo.top

Py:   def greet(name="World"): return name
来源：http://ene.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wyt.guowangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://gur.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fwm.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jpl.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rsk.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://atv.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://fxp.wangshuangyany.cn

[C03] 可变参数
来源：http://xlr.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://gqf.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://not.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://knm.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uiw.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wtd.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mdq.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://eoq.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oie.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://pfp.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ytk.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zuy.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zsi.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zzm.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://oui.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://usq.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://uam.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://tyh.daxiang520.top

[C05] 返回多个值
来源：http://vom.jinyuanbaomall.cn

Py:   return a, b
来源：http://rzo.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://ddx.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bry.yvedp.cn

TS:   return { a, b };
来源：http://nzf.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jph.fehbvm.com

Go:   return a, b
来源：http://mau.xuanzx.com

Ruby: return a, b
来源：http://vtm.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://gjh.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://khe.yongpay.top

Py:   square = lambda x: x * x
来源：http://ibi.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://exw.fehbvm.com

JS:   const square = x => x * x;
来源：http://dsp.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://vdm.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eyn.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nle.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://tor.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://frj.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://lvo.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://awr.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://bsu.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rif.redwolf501.top

TS:   arr.map(String)
来源：http://jsg.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hvg.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zcq.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://mag.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ctx.mhx1999.top

[C08] 闭包
来源：http://bdf.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ofe.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vqr.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ubn.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://edg.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pid.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rsr.hysaishi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oyw.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qtc.jiagoushi.top

[C09] 递归
来源：http://evn.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cfz.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://okz.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rnr.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://muf.9152youxi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fkg.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wdv.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hsm.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cmg.bbcook.cn

[C10] 变量作用域
来源：http://mww.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dbs.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ruo.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://scv.zhijiandao.cn

TS:   同 JS
来源：http://diu.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://shg.vqdsnc.cn

Go:   花括号块级作用域
来源：http://dad.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zxa.jinghuilouyu.cn

C#:   块级作用域
来源：http://zxl.cqqwz.cn

[C11] 模块导入与导出
来源：http://bhu.ehwqpu.com

Py:   from module import func
来源：http://qyf.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bcm.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://azh.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dee.redwolf501.top

Java: import java.util.List;
来源：http://vhy.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jiu.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://ume.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://ltr.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://zjg.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://eac.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://mkv.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://wjb.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://bux.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wso.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://dje.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://mxj.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pun.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://jok.pycfn.com


<!-- 参考信息 -->