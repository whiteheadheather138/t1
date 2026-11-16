代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://yuq.cdnleiting.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ijz.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://ggg.jlsjyb.cn

TS:   (3.14159).toFixed(2)
来源：http://lar.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ozq.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dsz.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://yvc.fanxiaobao.xyz

C#:   3.14159.ToString("F2")
来源：http://juq.ehwqpu.com

[A22] 获取字符串长度
来源：http://tyc.sysykeji.top

Py:   len(s)
来源：http://koe.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lok.xuanzx.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://elf.kuanghao11.cn

TS:   s.length
来源：http://sol.iojbl.cn

Java: s.length()
来源：http://txw.cdnleiting.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tbo.gaohongyu789.top

Ruby: s.length
来源：http://qbt.gzhubu.top

C#:   s.Length
来源：http://ixu.chenjidiqi.icu

[A23] 大小写转换
来源：http://ywr.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://erj.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wcr.hnqzz.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ywk.kuanghao11.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://txs.nanxinkj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://axb.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fcm.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://obx.yj20258888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pyc.uphjek.com

[A24] 去除首尾空白
来源：http://ekp.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://exp.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://igb.tianlin.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zzs.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cau.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lsg.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://tjn.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zss.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://orl.ydjk.org.cn

[A25] 字符串比较
来源：http://fqh.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://vtw.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qcz.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpn.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahm.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bbs.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nfz.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xgf.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rhl.svipenyu.cn

[A26] 类型转换总览
来源：http://wnq.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bud.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qoz.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ilu.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://scy.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uoa.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wci.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://flf.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://thm.jinghuilouyu.cn

================================================================================
来源：http://dcx.zhongyouzk.top

B. 流程控制
来源：http://hmr.vehdjk.com

================================================================================
来源：http://qxx.hywenlv.cn

[B01] 条件判断 if / else
来源：http://dhx.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gxf.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jyo.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nkm.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ydv.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lnf.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tdl.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://utc.sxryk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hyk.havefunace.top

[B02] 多分支 else if / elif
来源：http://pno.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rhe.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cth.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrt.c1oappe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tsl.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cty.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mzs.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yzx.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vrr.jinqigufen.top

[B03] switch / match / case
来源：http://ysz.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ncm.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dey.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uer.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ges.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zbp.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://biq.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oxo.zdqjudy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://scj.jqgfzy.top

[B04] for 计数循环
来源：http://gmb.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://ahp.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dmh.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hvt.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kop.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ngr.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wei.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://och.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mxn.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://vxl.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://dsy.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rlc.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gzc.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jfm.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eja.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eks.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://ebn.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ncd.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://fzn.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oiz.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qat.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vft.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mbb.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rey.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xsm.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rfb.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kiz.haohaochexian.top

[B07] while 循环
来源：http://bsz.gzhubu.top

Py:   while i < 10: i += 1
来源：http://jxb.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pzc.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://lnp.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://pwy.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://diu.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zld.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://ttd.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://ktp.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://szb.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://cjr.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mrg.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://hjj.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://far.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://dit.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://tdu.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://ewo.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://yqk.hongshengwenyu.top

[B09] break 与 continue
来源：http://hkq.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nhq.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ixa.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hiy.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfv.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oeb.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xfy.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tzs.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebb.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://lse.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jcn.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mta.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lzv.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gbn.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qdy.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kny.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ynp.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ses.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://prp.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://fil.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://syc.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nth.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://euc.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mzz.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mqj.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://tpd.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tdp.yvedp.cn

[B12] 跳出多层循环
来源：http://vbn.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ela.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://efy.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xwl.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ohj.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vqx.ppjwa.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tpz.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://win.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mya.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://qec.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://rhe.hesvh.cn

PHP:  is_numeric($x)
来源：http://euh.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zfs.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ags.fehbvm.com

Java: x instanceof Number
来源：http://ibx.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aqn.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://zzc.sysykeji.top

C#:   x is int or double or decimal
来源：http://mys.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://ypr.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mdk.tian-w.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://drx.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://cdi.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://fas.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://glr.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vfn.ehwqpu.com

Ruby: [1, 2, 3].include?(x)
来源：http://wfq.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hsb.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://nop.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://zqf.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://ofa.uphjek.com

JS:   a && b || !c
来源：http://ihm.birdmap.top

TS:   a && b || !c
来源：http://wmr.daxiang520.top

Java: a && b || !c
来源：http://iqb.nwbrower.top

Go:   a && b || !c
来源：http://klq.hywenlv.cn

Ruby: a && b || !c
来源：http://jwk.ivvv.top

C#:   a && b || !c
来源：http://diz.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://dlh.zhixingplan.top

Py:   if not data: return
来源：http://lya.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://mba.jianghu66.top

JS:   if (!data) return;
来源：http://ase.yonumen.top

TS:   if (!data) return;
来源：http://hjo.jinqigufen.top

Java: if (data == null) return;
来源：http://dxj.shuidangran.top

Go:   if data == nil { return }
来源：http://pwc.yj20258.top

Ruby: return if data.nil?
来源：http://sus.fengsongda.top

C#:   if (data == null) return;
来源：http://qqh.hnxiangtu.top

================================================================================
来源：http://mao.zhiwuduotai.top

C. 函数与作用域
来源：http://fsv.ehwqpu.com

================================================================================
来源：http://tji.yongpay.top

[C01] 定义函数
来源：http://int.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://cmn.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tvf.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://khl.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fvz.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qyv.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qgw.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://xdl.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxe.ivvv.top

[C02] 默认参数
来源：http://gtz.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://dar.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rvs.sjlbkw.cn

JS:   function greet(name = "World") { return name; }
来源：http://cdv.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vjb.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://fep.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vgg.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://rjr.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://cki.sjlbkw.cn

[C03] 可变参数
来源：http://xtr.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://ppk.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mcf.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://waa.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwq.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wog.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ppk.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wmc.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ced.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://aqi.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://heo.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ygh.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lta.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qks.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://hpu.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://xxk.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://fma.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://fng.fengsongda.top

[C05] 返回多个值
来源：http://dsa.tian-w.cn

Py:   return a, b
来源：http://zdd.nwbrower.top

PHP:  return [$a, $b];
来源：http://elm.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ozk.hywenlv.cn

TS:   return { a, b };
来源：http://bhm.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tdi.fehbvm.com

Go:   return a, b
来源：http://inx.daxiang520.top

Ruby: return a, b
来源：http://rgd.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://ncq.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://zpo.yvedp.cn

Py:   square = lambda x: x * x
来源：http://gkk.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ggp.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://tpw.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://tnf.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zoq.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://ggv.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://tdq.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://rjs.yj202588.top

[C07] 把函数作为参数传入
来源：http://xcz.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wym.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://ejs.jqgufenzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wdb.vqdsnc.cn

TS:   arr.map(String)
来源：http://fla.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lbu.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mmo.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://nfh.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lns.wangshuangyany.cn

[C08] 闭包
来源：http://jzd.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fcq.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sry.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oap.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://juu.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cyx.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pwa.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hzh.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mdw.jianghu66.top

[C09] 递归
来源：http://vzz.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qvi.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yfn.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://esv.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gfd.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tcx.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wfz.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iiq.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wns.pengpengdd.cyou

[C10] 变量作用域
来源：http://mdy.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rck.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ljh.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mtl.cqqwz.cn

TS:   同 JS
来源：http://osq.zhengqikj.top

Java: 方法内为块级作用域
来源：http://dwi.sweek.top

Go:   花括号块级作用域
来源：http://xwu.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tpg.yuanzhike.top

C#:   块级作用域
来源：http://tcs.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://gce.zhongyouzk.top

Py:   from module import func
来源：http://crx.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://isn.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://evr.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ryc.ppjwa.cn

Java: import java.util.List;
来源：http://stz.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cvk.zhengqikj.top


<!-- 参考信息 -->