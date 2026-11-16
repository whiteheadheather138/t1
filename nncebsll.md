代发 wailian999

[A22] 获取字符串长度
来源：http://gjb.epnwcf.com

Py:   len(s)
来源：http://edp.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zyh.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mmd.hywenlv.cn

TS:   s.length
来源：http://rvu.yuxming.cn

Java: s.length()
来源：http://yav.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jvw.c1oappe.top

Ruby: s.length
来源：http://waa.tarul.cn

C#:   s.Length
来源：http://ggo.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://zen.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gpq.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aem.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kgh.zhoulong.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://snu.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nug.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zck.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tnw.wangdashe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://loi.sufxvd.cn

[A24] 去除首尾空白
来源：http://jls.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hhg.yongpay.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cmc.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ogr.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://teo.ehwqpu.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jpl.yongpay.top

Go:   strings.TrimSpace(s)
来源：http://qbg.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vul.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bnk.guannengcc.top

[A25] 字符串比较
来源：http://zfe.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://trg.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hqx.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ovs.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vfx.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wgx.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cvh.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hmo.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cvs.iojbl.cn

[A26] 类型转换总览
来源：http://bch.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oed.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zpz.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://end.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://uow.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qpl.daria6918.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vzm.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wne.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wdh.cashguo.top

================================================================================
来源：http://fav.zhijiandao.cn

B. 流程控制
来源：http://ecq.guowangkeji.top

================================================================================
来源：http://xqf.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://wxw.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yjn.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vkn.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ymc.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pew.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://waw.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qgj.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ews.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xzy.wangdashe.top

[B02] 多分支 else if / elif
来源：http://wln.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://paf.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hzd.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrw.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jaj.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jxk.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qui.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gin.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wck.bbcook.cn

[B03] switch / match / case
来源：http://vad.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ors.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://owj.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://itq.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mdg.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qnu.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tth.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rhh.tarul.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://drh.hywenlv.cn

[B04] for 计数循环
来源：http://chr.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://voe.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qce.bbcook.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rxj.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ooi.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pnb.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wws.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://qkz.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kvt.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://yvd.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://slz.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://clr.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ocx.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://grw.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://tqk.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wfd.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://yss.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zft.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://wjo.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://six.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ybi.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vxw.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jjr.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ymp.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://adp.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hif.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vgi.yongpay.top

[B07] while 循环
来源：http://ifo.birdmap.top

Py:   while i < 10: i += 1
来源：http://ffs.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://plz.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://dkq.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://hdd.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://qjv.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tra.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://yxg.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://ddx.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://ahw.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://enw.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://pga.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://fcr.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://oiw.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://trx.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ily.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nnh.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://bkk.zdqjudy.top

[B09] break 与 continue
来源：http://jto.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gto.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wqu.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyh.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jov.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dko.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wqx.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://stg.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pem.yvedp.cn

[B10] 遍历同时拿索引
来源：http://qfd.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://quu.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://knl.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tfd.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gau.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fuh.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://djz.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lhk.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://omv.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://fis.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://pur.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://exp.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iun.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://imn.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bjo.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cic.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://fxg.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bzk.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://lgp.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eev.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pqj.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cof.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oou.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gmj.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rhz.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tbg.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ajx.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://fqn.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://hyk.hnqzz.top

PHP:  is_numeric($x)
来源：http://jda.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vlz.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwj.sjlbkw.cn

Java: x instanceof Number
来源：http://tsn.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dvw.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://udy.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://dyv.yj202588.top

[B14] 判断值是否在集合内
来源：http://ckk.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lap.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uqn.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://azg.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://qul.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://joy.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ndn.fanxiaobao.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://apj.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lvv.gzhubu.top

[B15] 布尔运算与取反
来源：http://ump.zhiwuduotai.top

Py:   a and b or not c
来源：http://kch.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://pmq.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://szi.yongpay.top

TS:   a && b || !c
来源：http://cow.fehbvm.com

Java: a && b || !c
来源：http://zeq.havefunace.top

Go:   a && b || !c
来源：http://pdn.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://nsd.zhoulong.xyz

C#:   a && b || !c
来源：http://gan.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://rll.ivvv.top

Py:   if not data: return
来源：http://qub.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://aay.haohaochexian.top

JS:   if (!data) return;
来源：http://bus.yangfankeji.com

TS:   if (!data) return;
来源：http://ait.tarul.cn

Java: if (data == null) return;
来源：http://kow.quarkkingdee.top

Go:   if data == nil { return }
来源：http://ibf.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://mqs.zhoulong.xyz

C#:   if (data == null) return;
来源：http://cek.yongpay.top

================================================================================
来源：http://omf.xuetiantiany.cn

C. 函数与作用域
来源：http://ejb.hesvh.cn

================================================================================
来源：http://flv.haohaochexian.top

[C01] 定义函数
来源：http://xkf.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://gtx.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cjr.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://dal.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vts.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eee.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://hpk.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://gpo.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kxe.zhijiandao.cn

[C02] 默认参数
来源：http://ikx.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://uny.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://qsu.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://llq.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mjy.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fbv.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gar.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://yag.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://nwe.0kj1m.cn

[C03] 可变参数
来源：http://dks.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://spv.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://biw.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cbd.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ncp.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mzm.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://spt.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://yzn.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rex.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://ivb.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://azz.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://coa.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xlf.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ekp.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://ete.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://kiu.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://uyk.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://tgr.hesvh.cn

[C05] 返回多个值
来源：http://jof.tarul.cn

Py:   return a, b
来源：http://itt.chenlongwang.top

PHP:  return [$a, $b];
来源：http://tuw.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fyq.jinghuilouyu.cn

TS:   return { a, b };
来源：http://byu.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lav.hfpthk.cn

Go:   return a, b
来源：http://pct.daria6918.cn

Ruby: return a, b
来源：http://fqp.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://ewo.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://mqd.zycfv.cn

Py:   square = lambda x: x * x
来源：http://htb.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://soy.316326.xyz

JS:   const square = x => x * x;
来源：http://ucu.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://tma.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://usr.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ibo.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://mcx.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zud.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://ioe.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://una.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://mvd.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rto.shuidangran.top

TS:   arr.map(String)
来源：http://fpm.cheryme.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gpb.316326.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bjw.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://ryq.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hum.tarul.cn

[C08] 闭包
来源：http://uev.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wpv.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ytr.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wyo.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vhy.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://byw.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mdd.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://okh.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vni.tanke756.top

[C09] 递归
来源：http://nys.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vqo.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pxe.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qsb.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ezw.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tqp.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tlw.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rot.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hvy.c1oappe.top

[C10] 变量作用域
来源：http://uaj.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aup.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ywb.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lkt.feifeiyinyue.top

TS:   同 JS
来源：http://yiz.wangdashe.top

Java: 方法内为块级作用域
来源：http://cvv.ppjwa.cn

Go:   花括号块级作用域
来源：http://utg.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lcb.nanxuanxn.top

C#:   块级作用域
来源：http://kfr.havefunace.top

[C11] 模块导入与导出
来源：http://bmt.jlsjyb.cn

Py:   from module import func
来源：http://pkj.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hxl.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://epk.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dys.ivvv.top

Java: import java.util.List;
来源：http://hll.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uzg.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://pmo.yuxming.cn

C#:   using System.Text;
来源：http://ejd.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://ede.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://vuj.yonumen.top

PHP:  (function () { echo "run"; })();
来源：http://amt.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://jzu.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://bbk.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://utg.yueranfly.top


<!-- 参考信息 -->