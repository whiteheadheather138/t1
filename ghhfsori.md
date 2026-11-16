代发 wailian999

TS:   s.length
来源：http://bcw.tianlin.xyz

Java: s.length()
来源：http://ytf.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lmf.ywan-chungtsiang.top

Ruby: s.length
来源：http://ths.jinghuilouyu.cn

C#:   s.Length
来源：http://iyd.cdnleiting.top

[A23] 大小写转换
来源：http://hhl.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ooh.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tmf.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tik.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mwk.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gzl.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uhg.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cre.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xgq.fzhhl.top

[A24] 去除首尾空白
来源：http://inm.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xdc.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://evc.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eiy.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tzn.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dma.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://bwn.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jwx.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://twc.redwolf501.top

[A25] 字符串比较
来源：http://yga.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://njf.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pao.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fcf.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zsg.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ddh.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dsb.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cqg.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rlt.shuidangran.top

[A26] 类型转换总览
来源：http://rpd.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ili.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jog.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zjj.yongpay.top

TS:   Number() String() Boolean() x as number
来源：http://chc.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tiw.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://peg.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gol.xinyue.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hlj.zhiwuduotai.top

================================================================================
来源：http://bkq.iojbl.cn

B. 流程控制
来源：http://gmo.0kj1m.cn

================================================================================
来源：http://cwj.shuidangran.top

[B01] 条件判断 if / else
来源：http://eqb.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://pyq.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xfm.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://npw.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pyt.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tar.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nii.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ogd.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ufh.hesvh.cn

[B02] 多分支 else if / elif
来源：http://prp.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mgk.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://twa.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uiv.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezd.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vae.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rbp.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wok.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wyk.birdmap.top

[B03] switch / match / case
来源：http://fkn.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fxr.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://usb.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xhi.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tge.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vdr.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://olv.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dab.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eea.bjfxy.top

[B04] for 计数循环
来源：http://cik.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://ecb.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dje.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bmr.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyd.jinyuanbaomall.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zbp.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vmf.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://ccl.xziqi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gxl.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://fhk.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://zft.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qny.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://wns.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://efn.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kvr.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://peu.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://ymc.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xwa.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://tar.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zvp.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yak.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kff.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lbs.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bql.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zhj.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dtm.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vuy.52xcode.cn

[B07] while 循环
来源：http://bwa.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://ccf.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://uap.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://ytd.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://ucn.epnwcf.com

Java: while (i < 10) { i++; }
来源：http://ids.dianchejie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mdt.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://ddy.sweek.top

C#:   while (i < 10) { i++; }
来源：http://ywj.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://abp.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://kcj.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uue.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://jyv.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://hls.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://bwa.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ibz.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://lcj.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://fub.jlsjyb.cn

[B09] break 与 continue
来源：http://rpn.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ses.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://olx.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://klk.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkk.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvm.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bqe.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dmn.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcr.cashguo.top

[B10] 遍历同时拿索引
来源：http://xyf.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lnb.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://toz.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zix.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bnu.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jug.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ejm.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xlt.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vhk.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://jvb.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://qun.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://erl.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xsl.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ivj.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jew.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://epk.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://fpc.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gcj.hnxiangtu.top

[B12] 跳出多层循环
来源：http://ixb.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gfb.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vxg.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmb.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ufe.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bor.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jzm.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://noy.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ura.dashuyun.cn

[B13] 判断是否为数字
来源：http://inu.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://zfa.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://byh.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zra.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dxr.shanyushiyangtech.top

Java: x instanceof Number
来源：http://ojw.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dmy.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://gbw.zdqjudy.top

C#:   x is int or double or decimal
来源：http://rjx.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://nfy.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fdl.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zwj.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://ywp.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://wpu.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lrr.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vwh.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eeh.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ehp.fehbvm.com

[B15] 布尔运算与取反
来源：http://ogo.hnqzz.top

Py:   a and b or not c
来源：http://vlf.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://zsc.gogol.net.cn

JS:   a && b || !c
来源：http://kvd.zhongyouzk.top

TS:   a && b || !c
来源：http://chx.xziqi.cn

Java: a && b || !c
来源：http://dmp.jlsjyb.cn

Go:   a && b || !c
来源：http://qij.vehdjk.com

Ruby: a && b || !c
来源：http://eoo.316326.xyz

C#:   a && b || !c
来源：http://eeb.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nza.sysykeji.top

Py:   if not data: return
来源：http://vmj.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://rkf.zdqjudy.top

JS:   if (!data) return;
来源：http://jvw.c1oappe.top

TS:   if (!data) return;
来源：http://tta.xuetiantiany.cn

Java: if (data == null) return;
来源：http://ube.yvedp.cn

Go:   if data == nil { return }
来源：http://cds.ivvv.top

Ruby: return if data.nil?
来源：http://gzj.fehbvm.com

C#:   if (data == null) return;
来源：http://gez.havefunace.top

================================================================================
来源：http://gxh.fanxiaobao.xyz

C. 函数与作用域
来源：http://vtg.yvedp.cn

================================================================================
来源：http://ami.cdnleiting.top

[C01] 定义函数
来源：http://xxi.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://veq.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sca.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://hja.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ikv.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lwp.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ejm.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://uvy.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oql.daxiang520.top

[C02] 默认参数
来源：http://awl.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://vux.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nfj.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://mfs.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qbk.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://jzz.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xnu.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://nmo.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://kcx.birdmap.top

[C03] 可变参数
来源：http://cwf.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://uvu.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wqc.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pen.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://avs.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wpt.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fjg.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://san.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pjc.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://jui.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://icg.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jrt.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lsx.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pun.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://tzi.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://zqw.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://jol.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://aeq.gzhubu.top

[C05] 返回多个值
来源：http://vob.chenzaomai.com

Py:   return a, b
来源：http://eih.sufxvd.cn

PHP:  return [$a, $b];
来源：http://zhu.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qiz.zhoulong.xyz

TS:   return { a, b };
来源：http://odg.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://abc.ybcxt.top

Go:   return a, b
来源：http://mid.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://car.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://omu.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://mpa.bbcook.cn

Py:   square = lambda x: x * x
来源：http://mkv.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://upx.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://ijx.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://ope.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ngg.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://blu.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://fso.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://wgk.bjfxy.top

[C07] 把函数作为参数传入
来源：http://adj.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jbp.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mdn.sysykeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vaq.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://eds.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gnz.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hbs.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://uex.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lek.snrcjt.cn

[C08] 闭包
来源：http://ryj.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sht.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ylp.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xnr.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xlh.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kst.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zyp.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gfw.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://afz.tarul.cn

[C09] 递归
来源：http://gdv.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bse.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tfd.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hez.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tff.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cos.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fad.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dvr.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vhi.yuxming.cn

[C10] 变量作用域
来源：http://pbn.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pjn.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ovf.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://auw.fzhhl.top

TS:   同 JS
来源：http://wrq.meibo888.top

Java: 方法内为块级作用域
来源：http://vym.dianchejie.cn

Go:   花括号块级作用域
来源：http://ttc.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gby.xylfe.cn

C#:   块级作用域
来源：http://vll.yj202588.top

[C11] 模块导入与导出
来源：http://rli.zdqjudy.top

Py:   from module import func
来源：http://gsf.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://irz.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uro.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fli.sufxvd.cn

Java: import java.util.List;
来源：http://htu.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nuh.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://gao.cqqwz.cn

C#:   using System.Text;
来源：http://nzm.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://wwq.meibo888.top

Py:   (lambda: print("run"))()
来源：http://idz.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://ymz.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://eab.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://hjv.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ekm.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://hxf.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://wsi.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://juq.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://mqt.52xcode.cn


<!-- 参考信息 -->