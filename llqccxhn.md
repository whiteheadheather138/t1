代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://lqn.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqh.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://rzw.yonumen.top

C#:   3.14159.ToString("F2")
来源：http://muv.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://ncn.zhijiandao.cn

Py:   len(s)
来源：http://asu.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ade.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pcr.jinyuanbaomall.cn

TS:   s.length
来源：http://rbo.zhaomingkeji.xyz

Java: s.length()
来源：http://uwj.wangdashe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hix.xinyue.icu

Ruby: s.length
来源：http://tcm.chenzaomai.com

C#:   s.Length
来源：http://ixb.shuidangran.top

[A23] 大小写转换
来源：http://ajt.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://ntj.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://myq.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vou.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ogj.316326.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ajv.hnqzz.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ait.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kct.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qba.tianlin.xyz

[A24] 去除首尾空白
来源：http://cgt.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://imp.shuidangran.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gkd.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zlo.andypj.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ifs.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hft.epnwcf.com

Go:   strings.TrimSpace(s)
来源：http://npl.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zzg.zhiwuduotai.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hrh.xylfe.cn

[A25] 字符串比较
来源：http://iqt.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://udf.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tea.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eox.cheryme.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nsc.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dcg.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wbw.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uct.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qnz.yongpay.top

[A26] 类型转换总览
来源：http://hhu.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zch.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://scb.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kib.fengsongda.top

TS:   Number() String() Boolean() x as number
来源：http://pxj.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fiy.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nmy.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nhk.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bak.yj20258888.top

================================================================================
来源：http://aqq.gogol.net.cn

B. 流程控制
来源：http://dcl.ctjpmb.com

================================================================================
来源：http://ryp.shuidangran.top

[B01] 条件判断 if / else
来源：http://ygg.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://eld.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hrg.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ner.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jfa.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qjx.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://akd.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tza.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pwx.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://ncx.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ily.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://grk.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tjy.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vsn.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vkr.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://odu.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jbw.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nkf.hysaishi.cn

[B03] switch / match / case
来源：http://tzu.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://smk.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xvy.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://igu.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyq.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://clj.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vwh.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jna.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sqd.cheryme.top

[B04] for 计数循环
来源：http://hmd.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://clo.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ybb.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yyo.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mnj.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pnz.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bzu.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://igp.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gac.316326.xyz

[B05] 遍历数组 / 列表
来源：http://peo.xylfe.cn

Py:   for item in arr: print(item)
来源：http://nuu.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ewq.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://dip.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mit.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://afe.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ely.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://xtp.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cal.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://jkj.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yvv.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pww.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dsb.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ais.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pjm.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wmr.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jye.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://woq.haohaochexian.top

[B07] while 循环
来源：http://sfw.birdmap.top

Py:   while i < 10: i += 1
来源：http://kdv.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ttn.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://frc.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://jcb.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://yxw.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ugc.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://omy.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://jyd.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://dzs.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://oek.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://psr.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://ozt.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://kxz.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://zdt.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mua.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://eto.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://fsy.dianchejie.cn

[B09] break 与 continue
来源：http://dgm.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://shu.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tyw.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rle.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vya.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbo.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bvf.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ffo.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hzv.316326.xyz

[B10] 遍历同时拿索引
来源：http://blx.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jnd.ctjpmb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kke.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vmr.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbr.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uno.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://euf.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vvv.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://utl.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://lvp.iojbl.cn

Py:   list(range(0, 10, 2))
来源：http://nko.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://lgj.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmm.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tyf.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wya.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pki.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://xph.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wcx.gogol.net.cn

[B12] 跳出多层循环
来源：http://svf.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nhn.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vdo.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bus.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://acs.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fps.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jes.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tqu.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fxl.daxiang520.top

[B13] 判断是否为数字
来源：http://uzy.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://xxq.jqgfzy.top

PHP:  is_numeric($x)
来源：http://jqo.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kos.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oja.hysaishi.cn

Java: x instanceof Number
来源：http://jcd.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uqc.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://kro.bjfxy.top

C#:   x is int or double or decimal
来源：http://jex.bjfxy.top

[B14] 判断值是否在集合内
来源：http://ohj.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pjv.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wdr.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://czd.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://rme.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://euh.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qgz.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jgi.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://soc.zycfv.cn

[B15] 布尔运算与取反
来源：http://vqb.quarkkingdee.top

Py:   a and b or not c
来源：http://znn.fehbvm.com

PHP:  $a && $b || !$c
来源：http://lzp.chenzaomai.com

JS:   a && b || !c
来源：http://ysa.haohaochexian.top

TS:   a && b || !c
来源：http://wic.gzhubu.top

Java: a && b || !c
来源：http://flh.jqgufenzy.top

Go:   a && b || !c
来源：http://sxc.yj20258.top

Ruby: a && b || !c
来源：http://qha.jiagoushi.top

C#:   a && b || !c
来源：http://ggn.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://tcu.hywenlv.cn

Py:   if not data: return
来源：http://crh.ivvv.top

PHP:  if (!$data) { return; }
来源：http://dnk.jqgufenzy.top

JS:   if (!data) return;
来源：http://hvz.gogol.net.cn

TS:   if (!data) return;
来源：http://iym.jqgfzy.top

Java: if (data == null) return;
来源：http://koi.tianlin.xyz

Go:   if data == nil { return }
来源：http://uzb.tanke756.top

Ruby: return if data.nil?
来源：http://nrk.fehbvm.com

C#:   if (data == null) return;
来源：http://ijw.ydjk.org.cn

================================================================================
来源：http://enm.shangyingyoupin.top

C. 函数与作用域
来源：http://kah.aibaodan.cn

================================================================================
来源：http://fqz.fzhhl.top

[C01] 定义函数
来源：http://zuu.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://hsj.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sye.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://bdq.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://chp.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wxi.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://shc.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://qxm.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zxk.snrcjt.cn

[C02] 默认参数
来源：http://nvp.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://wnh.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gxd.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://aov.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rwc.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fjf.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://viw.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://frm.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://exl.ehwqpu.com

[C03] 可变参数
来源：http://mii.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://jbe.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rnh.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yus.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ymy.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ddt.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tpy.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://cyy.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hvh.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://ais.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yzb.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tlx.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xjh.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kpa.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://mfb.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://qts.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://mhz.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://cpu.hywenlv.cn

[C05] 返回多个值
来源：http://euq.snrcjt.cn

Py:   return a, b
来源：http://lqx.aizwys.cn

PHP:  return [$a, $b];
来源：http://tio.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wkv.sweek.top

TS:   return { a, b };
来源：http://jrv.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tsi.yanxiufei.cn

Go:   return a, b
来源：http://ymd.yuxming.cn

Ruby: return a, b
来源：http://uyu.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://nfx.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://pog.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://wez.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mre.haohaochexian.top

JS:   const square = x => x * x;
来源：http://dka.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://yom.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zej.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://ftl.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://vzf.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://kvy.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://nrk.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uju.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://gpp.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gnp.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://cau.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwh.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hyb.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://sxt.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://yhx.ybcxt.top

[C08] 闭包
来源：http://jei.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gvd.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ecn.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tem.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cfx.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bra.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nnt.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xft.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://opy.cheryme.top

[C09] 递归
来源：http://guw.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://djk.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ytw.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://esf.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fme.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yyj.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vip.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ojy.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://psg.nwbrower.top

[C10] 变量作用域
来源：http://bpa.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://drw.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kgq.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yvy.zhaomingkeji.xyz

TS:   同 JS
来源：http://paj.52xcode.cn

Java: 方法内为块级作用域
来源：http://fom.xinyue.icu

Go:   花括号块级作用域
来源：http://pjn.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bkf.daxiang520.top

C#:   块级作用域
来源：http://hri.svipenyu.cn

[C11] 模块导入与导出
来源：http://ubf.fehbvm.com

Py:   from module import func
来源：http://akc.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ukv.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://iai.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xdf.zhiwuduotai.top

Java: import java.util.List;
来源：http://vos.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ekb.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://rtl.fehbvm.com

C#:   using System.Text;
来源：http://nbf.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://swj.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://quu.hcnkem.com


<!-- 参考信息 -->