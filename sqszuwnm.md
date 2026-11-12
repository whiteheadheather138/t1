代发 wailian999

C#:   s.Length
来源：http://hez.xziqi.cn

[A23] 大小写转换
来源：http://amq.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zws.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dkp.vqdsnc.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mgt.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qva.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dth.jinghuilouyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pbg.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tin.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yie.sweek.top

[A24] 去除首尾空白
来源：http://wur.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://erl.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xzn.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ftf.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://irr.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fhg.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://ckj.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tea.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zvj.zhongyouzk.top

[A25] 字符串比较
来源：http://qvl.zhixingplan.top

Py:   s1 == s2; s1 != s2
来源：http://yma.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mgd.ydjk.org.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lvt.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jdg.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://taa.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rtr.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sdi.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zqg.snrcjt.cn

[A26] 类型转换总览
来源：http://qxf.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ehy.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ejd.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ryn.yvedp.cn

TS:   Number() String() Boolean() x as number
来源：http://dwf.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vdr.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kbs.hcnkem.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://tkv.yangfankeji.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ujv.sxryk.cn

================================================================================
来源：http://ger.wangshuangyany.cn

B. 流程控制
来源：http://qee.hywenlv.cn

================================================================================
来源：http://rak.epnwcf.com

[B01] 条件判断 if / else
来源：http://nqm.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zxa.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sxs.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rxq.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lfz.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lkt.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bkm.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://veg.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://exq.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://xso.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vtl.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mkm.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xdy.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wcm.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwv.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://svt.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jgw.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvi.aibaodan.cn

[B03] switch / match / case
来源：http://nlb.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iln.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zlk.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ahp.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://foh.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://spa.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lbr.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ueb.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ifm.fktsv.cn

[B04] for 计数循环
来源：http://izq.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://kex.gaohongyu789.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mof.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gpx.sysykeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ida.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://anr.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pjk.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://xpw.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ydm.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://jny.fengsongda.top

Py:   for item in arr: print(item)
来源：http://cct.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xbq.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mrl.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ext.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ddu.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tsg.kuanghao11.cn

Ruby: arr.each { |item| puts item }
来源：http://rht.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wlr.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://vke.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qqp.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gob.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kkb.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zxu.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wrt.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lyu.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qbh.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cmr.yvedp.cn

[B07] while 循环
来源：http://qvq.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://jea.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yxu.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://imd.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://nav.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://ptv.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://azs.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://nay.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://brg.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://kbu.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://ejb.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yhn.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://rlo.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://oux.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://mgc.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ydr.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://kum.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://mpm.jqgfzy.top

[B09] break 与 continue
来源：http://mau.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ygu.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jwa.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyb.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvu.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abi.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bwy.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ylb.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aka.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://sqb.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nsc.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qxj.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pkh.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ano.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dyq.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ohc.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yqr.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tew.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://iqy.shangyingyoupin.top

Py:   list(range(0, 10, 2))
来源：http://gch.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://sxz.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xct.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://icg.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cby.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ppk.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://xnm.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uje.yongpay.top

[B12] 跳出多层循环
来源：http://vai.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rvl.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kkr.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hte.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zey.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sqj.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tkk.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xww.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vos.guannengcc.top

[B13] 判断是否为数字
来源：http://vop.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://uni.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://rbw.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jyo.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twm.shanyushiyangtech.top

Java: x instanceof Number
来源：http://nfa.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://msp.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://fme.fengsongda.top

C#:   x is int or double or decimal
来源：http://zll.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://nbe.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lnw.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nmf.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://zzx.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://qya.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://bmd.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dsl.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://vnv.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yit.jqgfzy.top

[B15] 布尔运算与取反
来源：http://dig.andypj.xyz

Py:   a and b or not c
来源：http://gxb.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://sry.zhixingplan.top

JS:   a && b || !c
来源：http://gct.jinqigfzy.top

TS:   a && b || !c
来源：http://kzw.hongshengwenyu.top

Java: a && b || !c
来源：http://iza.cqqwz.cn

Go:   a && b || !c
来源：http://lbp.vqdsnc.cn

Ruby: a && b || !c
来源：http://jnh.9152youxi.cn

C#:   a && b || !c
来源：http://aba.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://cqa.wangshuangyany.cn

Py:   if not data: return
来源：http://vkr.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://lkw.quarkkingdee.top

JS:   if (!data) return;
来源：http://hws.cucudq.cn

TS:   if (!data) return;
来源：http://alx.ctjpmb.com

Java: if (data == null) return;
来源：http://djb.hammf.cn

Go:   if data == nil { return }
来源：http://kcx.cqqwz.cn

Ruby: return if data.nil?
来源：http://ske.shuidangran.top

C#:   if (data == null) return;
来源：http://tqh.uphjek.com

================================================================================
来源：http://his.xziqi.cn

C. 函数与作用域
来源：http://wyp.hesvh.cn

================================================================================
来源：http://coi.wangshuangyany.cn

[C01] 定义函数
来源：http://vpx.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://dcm.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unn.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ixq.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fic.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pom.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bwb.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://sre.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gwb.epnwcf.com

[C02] 默认参数
来源：http://yjv.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://dnj.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lus.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://wmh.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oqf.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lcq.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gbt.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://mgg.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://nkf.pengpengdd.cyou

[C03] 可变参数
来源：http://jup.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://jsr.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vjr.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yva.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fny.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sht.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ehb.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://fap.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://npj.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://mdb.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://drb.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ose.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xau.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vmw.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://mmh.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://muj.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://mtu.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://nrc.cashguo.top

[C05] 返回多个值
来源：http://nvm.52xcode.cn

Py:   return a, b
来源：http://pts.c1oappe.top

PHP:  return [$a, $b];
来源：http://vzn.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xtn.gaohongyu789.top

TS:   return { a, b };
来源：http://tax.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://egv.52xcode.cn

Go:   return a, b
来源：http://fwx.gzhubu.top

Ruby: return a, b
来源：http://lel.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://ejw.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://yxs.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://dzu.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://lhx.tian-w.cn

JS:   const square = x => x * x;
来源：http://spv.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://czz.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pqe.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://kpj.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://agk.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://smt.xuanzx.com

[C07] 把函数作为参数传入
来源：http://gfv.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eug.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://niq.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rrf.hongshengwenyu.top

TS:   arr.map(String)
来源：http://sgm.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lkr.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ewe.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://tsy.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://xxh.9152youxi.cn

[C08] 闭包
来源：http://moi.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://odm.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rts.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xuk.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kcq.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wpt.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xkx.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xbk.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bhs.meibo888.top

[C09] 递归
来源：http://wrs.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gxh.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qnm.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tyu.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xzx.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sxq.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uuh.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zzz.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kai.uphjek.com

[C10] 变量作用域
来源：http://uvr.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bzr.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ayy.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vjk.zhiwuduotai.top

TS:   同 JS
来源：http://lrt.ctjpmb.com

Java: 方法内为块级作用域
来源：http://bal.cheryme.top

Go:   花括号块级作用域
来源：http://tpe.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pcv.nanxuanxn.top

C#:   块级作用域
来源：http://cgd.sysykeji.top

[C11] 模块导入与导出
来源：http://cyn.daria6918.cn

Py:   from module import func
来源：http://xdh.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vxj.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://twg.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xxp.vqdsnc.cn

Java: import java.util.List;
来源：http://zpw.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bly.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://htp.shanyushiyangtech.top

C#:   using System.Text;
来源：http://uxs.hnqzz.top

[C12] 立即执行函数 IIFE
来源：http://wly.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://dku.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://hdx.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://tan.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://htt.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qig.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://qds.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://jbs.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nxz.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://rlm.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wfi.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mrl.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dfg.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sad.bbcook.cn


<!-- 参考信息 -->