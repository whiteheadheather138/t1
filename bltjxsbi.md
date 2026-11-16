代发 wailian999

[A22] 获取字符串长度
来源：http://bdn.xinyue.icu

Py:   len(s)
来源：http://oif.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eor.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zdy.vqdsnc.cn

TS:   s.length
来源：http://wen.pengpengdd.cyou

Java: s.length()
来源：http://svb.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://typ.yfazqb.com

Ruby: s.length
来源：http://kgj.jqgufenzy.top

C#:   s.Length
来源：http://myq.guowangkeji.top

[A23] 大小写转换
来源：http://xmp.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ift.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gkr.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://htw.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uid.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://skt.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nfh.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hze.zycfv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uuq.tanke756.top

[A24] 去除首尾空白
来源：http://ktc.xingfuxueyuan.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hcw.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gyy.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://miz.meibo888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ksi.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://syh.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://abk.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sjn.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zjt.sweek.top

[A25] 字符串比较
来源：http://qqy.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://jsb.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dvy.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fqz.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dsq.yfazqb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://snp.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cfy.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://txn.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://har.zycfv.cn

[A26] 类型转换总览
来源：http://nza.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xqu.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uub.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vco.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://ycv.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xqe.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://igw.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xgy.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fhi.dianchejie.cn

================================================================================
来源：http://xsl.yangfankeji.com

B. 流程控制
来源：http://pva.birdmap.top

================================================================================
来源：http://jgd.fengsongda.top

[B01] 条件判断 if / else
来源：http://sam.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tav.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nuv.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jxt.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tfy.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ini.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ydo.zhaomingkeji.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nln.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xus.tian-w.cn

[B02] 多分支 else if / elif
来源：http://kqg.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sqp.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yyd.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gjg.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agd.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yad.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xix.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fnr.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kun.haohaochexian.top

[B03] switch / match / case
来源：http://bkk.xziqi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fap.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yix.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hcb.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxd.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cqm.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rls.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://icw.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gji.dianchejie.cn

[B04] for 计数循环
来源：http://zmt.havefunace.top

Py:   for i in range(10): print(i)
来源：http://yas.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cum.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lfk.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sdl.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zgb.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qvx.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://mtk.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sde.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://zsx.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://fpi.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sqs.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nyu.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bks.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oku.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://val.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://kgj.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ghc.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://uvd.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qkr.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ymd.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hlc.meibo888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ajx.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lec.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wwd.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bxu.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zgo.ivvv.top

[B07] while 循环
来源：http://rux.redwolf501.top

Py:   while i < 10: i += 1
来源：http://ubp.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://lhx.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://guy.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://cqj.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://xqt.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qyo.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://ziq.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://gds.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://cxm.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://ird.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kwb.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://lkb.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://nxk.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://cmm.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wqv.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://buv.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://gdd.zycfv.cn

[B09] break 与 continue
来源：http://afh.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qjq.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yil.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rth.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vfr.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcz.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mup.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://foq.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dyk.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://esf.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://whs.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zkx.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://exr.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ypd.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://her.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vsr.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wec.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pod.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://icu.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://nnn.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://ghe.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jwk.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nak.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lpl.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dyv.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://fnd.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pyz.zhijiandao.cn

[B12] 跳出多层循环
来源：http://lgc.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gji.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ynq.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zun.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ybh.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bup.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ton.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgd.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vrk.nwbrower.top

[B13] 判断是否为数字
来源：http://lee.chenlongwang.top

Py:   isinstance(x, (int, float))
来源：http://erl.guowangkeji.top

PHP:  is_numeric($x)
来源：http://wpf.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xom.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bri.fanxiaobao.xyz

Java: x instanceof Number
来源：http://vka.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kwg.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://cjp.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://kqx.hammf.cn

[B14] 判断值是否在集合内
来源：http://uup.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://trv.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gcr.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://mru.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://owr.smart0.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://tuk.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pkd.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yua.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jef.yj202588.top

[B15] 布尔运算与取反
来源：http://avh.cucudq.cn

Py:   a and b or not c
来源：http://pyx.nwbrower.top

PHP:  $a && $b || !$c
来源：http://clp.hfpthk.cn

JS:   a && b || !c
来源：http://fee.pengpengdd.cyou

TS:   a && b || !c
来源：http://ydr.cdnleiting.top

Java: a && b || !c
来源：http://kro.ydzc1.top

Go:   a && b || !c
来源：http://smq.xylfe.cn

Ruby: a && b || !c
来源：http://cqt.wangdashe.top

C#:   a && b || !c
来源：http://apc.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ops.iojbl.cn

Py:   if not data: return
来源：http://xqj.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://ahi.birdmap.top

JS:   if (!data) return;
来源：http://lgo.jlsjyb.cn

TS:   if (!data) return;
来源：http://eky.vehdjk.com

Java: if (data == null) return;
来源：http://cbu.xylfe.cn

Go:   if data == nil { return }
来源：http://zvk.sufxvd.cn

Ruby: return if data.nil?
来源：http://aau.mhx1999.top

C#:   if (data == null) return;
来源：http://cin.cashguo.top

================================================================================
来源：http://kcf.ivvv.top

C. 函数与作用域
来源：http://nzt.jlsjyb.cn

================================================================================
来源：http://ihq.sufxvd.cn

[C01] 定义函数
来源：http://was.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://igc.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tkd.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://xch.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rgl.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ski.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://cdw.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://pnk.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bsj.zhengqikj.top

[C02] 默认参数
来源：http://dal.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://krn.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://qlx.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://wog.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bqp.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://thl.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kqk.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://zdd.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://akm.xziqi.cn

[C03] 可变参数
来源：http://aqd.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://iqc.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wyc.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bog.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ftd.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nff.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nkd.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://biw.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eab.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://xri.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fem.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://anz.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bat.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rqw.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://woy.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://eiz.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://qxv.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://bdt.yonumen.top

[C05] 返回多个值
来源：http://djb.sufxvd.cn

Py:   return a, b
来源：http://rky.cqqwz.cn

PHP:  return [$a, $b];
来源：http://qvd.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mud.tanke756.top

TS:   return { a, b };
来源：http://jmt.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jed.ybcxt.top

Go:   return a, b
来源：http://kew.jinyuanbaomall.cn

Ruby: return a, b
来源：http://zuz.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://que.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://sqx.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://awk.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gri.jyoumei.cn

JS:   const square = x => x * x;
来源：http://lln.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://qgp.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qcc.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://kfq.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://pvc.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://chk.c1oappe.top

[C07] 把函数作为参数传入
来源：http://rmr.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lic.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dmr.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ttr.xziqi.cn

TS:   arr.map(String)
来源：http://pkj.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zsl.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cqn.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://vjn.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://psb.kuanghao11.cn

[C08] 闭包
来源：http://cgz.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vfu.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://esa.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ukx.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gmu.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lco.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ave.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rkp.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ieu.ivvv.top

[C09] 递归
来源：http://tyu.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://utt.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://chg.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ipr.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pfy.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://llr.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zdb.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rah.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kqc.wangdashe.top

[C10] 变量作用域
来源：http://mdl.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jwb.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yjj.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://khj.zhiwuduotai.top

TS:   同 JS
来源：http://rzd.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://rfn.hcnkem.com

Go:   花括号块级作用域
来源：http://vrq.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dxe.yfazqb.com

C#:   块级作用域
来源：http://god.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://vvq.xinyue.icu

Py:   from module import func
来源：http://lvo.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://okm.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tiz.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://elw.nwbrower.top

Java: import java.util.List;
来源：http://mfg.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iwg.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://uqh.ctjpmb.com

C#:   using System.Text;
来源：http://ird.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://lrg.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://iqg.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://blv.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://iip.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://aom.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bya.xylfe.cn


<!-- 参考信息 -->