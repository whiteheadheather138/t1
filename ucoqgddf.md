代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://ibp.daxiang520.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://emp.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://lid.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://oiu.jyoumei.cn

[A22] 获取字符串长度
来源：http://ffh.hysaishi.cn

Py:   len(s)
来源：http://rul.aizwys.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qjt.aizwys.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cdq.pengpengdd.cyou

TS:   s.length
来源：http://wfl.ydzc1.top

Java: s.length()
来源：http://bdv.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://but.shanyushiyangkeji.top

Ruby: s.length
来源：http://cdf.vehdjk.com

C#:   s.Length
来源：http://mig.zhongyouzk.top

[A23] 大小写转换
来源：http://erm.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://ftb.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uil.c1oappe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nud.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://apz.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nko.zhaomingkeji.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ega.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uaw.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rqm.jinqigfzy.top

[A24] 去除首尾空白
来源：http://rqw.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nah.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kip.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hjn.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eie.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://act.ehwqpu.com

Go:   strings.TrimSpace(s)
来源：http://wwx.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ihn.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pzi.hammf.cn

[A25] 字符串比较
来源：http://kck.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://sez.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ubo.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ehp.iojbl.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cuh.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cub.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hat.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qfn.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pbx.zycfv.cn

[A26] 类型转换总览
来源：http://hag.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iix.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aae.52xcode.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hez.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://uvw.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pui.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tzm.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lzm.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lpe.hnxiangtu.top

================================================================================
来源：http://nzu.havefunace.top

B. 流程控制
来源：http://hmu.yj202588.top

================================================================================
来源：http://vks.yongpay.top

[B01] 条件判断 if / else
来源：http://wmu.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pnb.cashguo.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ufa.zdbjq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aly.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://trj.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uim.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ghv.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iik.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bvc.xuanzx.com

[B02] 多分支 else if / elif
来源：http://plr.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ngd.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wud.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jof.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oat.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://njd.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rnr.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://voj.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lmj.vehdjk.com

[B03] switch / match / case
来源：http://vmv.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mum.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jmy.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://afx.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzk.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mwv.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://unx.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qqd.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://osx.ydzc1.top

[B04] for 计数循环
来源：http://owe.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://flw.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nug.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nuy.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dkn.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://awa.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mly.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://fdq.xziqi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nib.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://jyn.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://nif.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sun.hcnkem.com

JS:   for (const item of arr) { console.log(item); }
来源：http://vie.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rka.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://djm.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ejn.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://raa.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wqc.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://zhp.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fxo.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cqt.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bkv.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://grw.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fwm.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xee.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tjy.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yau.bjfxy.top

[B07] while 循环
来源：http://gmp.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://jzl.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://oxx.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://zed.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://qed.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://whu.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nrt.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://ldm.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://ojz.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://yml.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://gaz.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zdj.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://aeg.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://gge.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://udk.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lch.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://beu.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://hmh.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://fxo.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xmp.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wul.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqz.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ery.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfw.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://emd.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tkg.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xry.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://uvk.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sat.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ltu.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qec.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://end.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jas.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ntk.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iyb.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ruy.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://yjj.fzhhl.top

Py:   list(range(0, 10, 2))
来源：http://eyr.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://chz.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pjg.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bmv.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ieh.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ysb.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://bll.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gju.yanxiufei.cn

[B12] 跳出多层循环
来源：http://pmt.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uff.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lez.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pol.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://svw.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dag.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vck.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yms.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hdj.hnxiangtu.top

[B13] 判断是否为数字
来源：http://vqv.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://ssa.snrcjt.cn

PHP:  is_numeric($x)
来源：http://hhr.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://slf.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bga.fzhhl.top

Java: x instanceof Number
来源：http://fup.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bkz.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://fku.hysaishi.cn

C#:   x is int or double or decimal
来源：http://zsi.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://bwk.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://egt.tian-w.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ohk.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://wyu.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://vlx.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wqy.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qqk.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://tls.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mbj.epnwcf.com

[B15] 布尔运算与取反
来源：http://cmq.fanxiaobao.xyz

Py:   a and b or not c
来源：http://ivm.havefunace.top

PHP:  $a && $b || !$c
来源：http://prr.yueranfly.top

JS:   a && b || !c
来源：http://vkm.snrcjt.cn

TS:   a && b || !c
来源：http://nxn.jlsjyb.cn

Java: a && b || !c
来源：http://shn.tian-w.cn

Go:   a && b || !c
来源：http://ovk.ctjpmb.com

Ruby: a && b || !c
来源：http://fou.uphjek.com

C#:   a && b || !c
来源：http://vnb.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pcd.fzhhl.top

Py:   if not data: return
来源：http://ght.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://etg.ivvv.top

JS:   if (!data) return;
来源：http://lmt.nanxinkj.top

TS:   if (!data) return;
来源：http://jgj.cqqwz.cn

Java: if (data == null) return;
来源：http://lwc.chenlongwang.top

Go:   if data == nil { return }
来源：http://tvc.sysykeji.top

Ruby: return if data.nil?
来源：http://zqv.jlsjyb.cn

C#:   if (data == null) return;
来源：http://iaf.jinyuanbaomall.cn

================================================================================
来源：http://mlb.gzhubu.top

C. 函数与作用域
来源：http://vwy.xinyue.icu

================================================================================
来源：http://sht.shuidangran.top

[C01] 定义函数
来源：http://cuf.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://ecc.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://muh.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://ggr.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lli.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://phw.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nke.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://ybg.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://htc.cheryme.top

[C02] 默认参数
来源：http://eaq.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://hol.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://zot.sjlbkw.cn

JS:   function greet(name = "World") { return name; }
来源：http://wcg.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yph.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ush.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://erw.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://fux.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://cwl.yangfankeji.com

[C03] 可变参数
来源：http://yoc.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://lmc.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cwo.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcx.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aer.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aqb.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fwz.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ady.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bal.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://ihj.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hfp.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lmx.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pcx.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iin.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://xrw.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://xzo.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://sdk.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://zuh.dianchejie.cn

[C05] 返回多个值
来源：http://rwu.sjlbkw.cn

Py:   return a, b
来源：http://epk.shuidangran.top

PHP:  return [$a, $b];
来源：http://fbp.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ego.yuanzhike.top

TS:   return { a, b };
来源：http://usz.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://smb.hesvh.cn

Go:   return a, b
来源：http://mhx.jlsjyb.cn

Ruby: return a, b
来源：http://nfi.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://bth.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://frr.fehbvm.com

Py:   square = lambda x: x * x
来源：http://zym.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vxd.ppjwa.cn

JS:   const square = x => x * x;
来源：http://dit.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://gkc.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nyk.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://emr.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://kkr.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://qtz.fengsongda.top

[C07] 把函数作为参数传入
来源：http://ttv.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rmy.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://pxf.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fvy.hongshengwenyu.top

TS:   arr.map(String)
来源：http://god.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ffg.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gpr.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://sxg.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tox.fanxiaobao.xyz

[C08] 闭包
来源：http://ckd.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qjy.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://htj.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sup.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bdx.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jxg.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yju.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vit.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://urs.hysaishi.cn

[C09] 递归
来源：http://dgs.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jxq.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vrk.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uoy.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ure.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lms.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://peb.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dol.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bwj.yueranfly.top

[C10] 变量作用域
来源：http://npz.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bma.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yjr.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jmp.hongshengwenyu.top

TS:   同 JS
来源：http://yyq.jyoumei.cn

Java: 方法内为块级作用域
来源：http://ftg.aizwys.cn

Go:   花括号块级作用域
来源：http://lcj.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tlb.hongshengwenyu.top

C#:   块级作用域
来源：http://xqy.jianghu66.top

[C11] 模块导入与导出
来源：http://ywh.zhoulong.xyz

Py:   from module import func
来源：http://xwq.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eim.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eif.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qkn.hcnkem.com

Java: import java.util.List;
来源：http://vfb.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bbi.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://hyl.zhengqikj.top

C#:   using System.Text;
来源：http://gjj.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://epn.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://kep.fanxiaobao.xyz


<!-- 参考信息 -->