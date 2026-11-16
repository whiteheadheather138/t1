代发 wailian999

[A22] 获取字符串长度
来源：http://fzl.dashuyun.cn

Py:   len(s)
来源：http://vxe.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sqx.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://owy.jyoumei.cn

TS:   s.length
来源：http://lif.ivvv.top

Java: s.length()
来源：http://zff.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mcw.hywenlv.cn

Ruby: s.length
来源：http://ahd.ivvv.top

C#:   s.Length
来源：http://qwi.sufxvd.cn

[A23] 大小写转换
来源：http://nzx.tian-w.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dpg.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://utm.quarkkingdee.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tnm.gogol.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xdr.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fid.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://apg.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gdp.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://htc.nanxinkj.top

[A24] 去除首尾空白
来源：http://usm.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lto.redwolf501.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fnf.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://anp.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baw.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mav.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://hvw.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wlv.daxiang520.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rgb.chenlongwang.top

[A25] 字符串比较
来源：http://lxy.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://hfc.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xgk.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rzf.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tbq.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dla.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wmi.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dts.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uig.zhixingplan.top

[A26] 类型转换总览
来源：http://bib.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lou.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yiu.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pur.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://gxc.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ble.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eqm.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://beg.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uaa.ehwqpu.com

================================================================================
来源：http://acd.xziqi.cn

B. 流程控制
来源：http://zcz.gogol.net.cn

================================================================================
来源：http://bbh.zdbjq.cn

[B01] 条件判断 if / else
来源：http://wcp.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bry.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uyj.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cqa.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hxg.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ayu.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tug.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oop.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qeg.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://pss.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nmx.hnxiangtu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jeu.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://njz.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://enz.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybc.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iay.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pnu.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nll.wangshuangyany.cn

[B03] switch / match / case
来源：http://mnw.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yeg.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iag.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cfc.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://krq.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://idk.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://esw.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ilt.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zay.ywan-chungtsiang.top

[B04] for 计数循环
来源：http://hjx.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://qtk.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aam.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qgc.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zxi.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oax.fehbvm.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xlr.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://mab.wangdashe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://los.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://jlc.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://zzg.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xcc.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aox.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yoh.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mei.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://scr.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://vmt.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mws.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://ksg.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oel.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tpb.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpw.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yuz.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ior.fehbvm.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sak.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jbf.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qrg.hywenlv.cn

[B07] while 循环
来源：http://esi.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://irc.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://wuf.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://yqc.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://yde.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://uzz.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tas.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://iqq.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://jia.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://zgq.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://yut.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fbt.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://smj.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://cet.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://zya.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zcm.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eda.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://xlv.ybcxt.top

[B09] break 与 continue
来源：http://vqr.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://svg.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fub.zhijiandao.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fma.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsk.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bdu.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://irc.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ezz.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nij.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://cjl.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tbl.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xqh.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yqr.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dzr.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rvp.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://arf.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vva.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tvf.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://neb.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://bia.yonumen.top

PHP:  range(0, 10, 2);
来源：http://nmy.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ekr.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://htl.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hbu.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hpx.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://xdh.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jko.yanxiufei.cn

[B12] 跳出多层循环
来源：http://vkw.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rcw.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lkn.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://brb.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ski.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lcd.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aqp.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zqc.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://syw.daxiang520.top

[B13] 判断是否为数字
来源：http://aht.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://xgo.ivvv.top

PHP:  is_numeric($x)
来源：http://owa.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yfc.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cal.fehbvm.com

Java: x instanceof Number
来源：http://ruo.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oek.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://teg.bjfxy.top

C#:   x is int or double or decimal
来源：http://yqh.uphjek.com

[B14] 判断值是否在集合内
来源：http://mjn.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iyr.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://umq.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://eai.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://kct.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nqb.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ckk.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jmb.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fui.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://nbn.fengsongda.top

Py:   a and b or not c
来源：http://ecd.tian-w.cn

PHP:  $a && $b || !$c
来源：http://xit.tian-w.cn

JS:   a && b || !c
来源：http://abn.0kj1m.cn

TS:   a && b || !c
来源：http://mce.sweek.top

Java: a && b || !c
来源：http://nyr.gotoacloud.top

Go:   a && b || !c
来源：http://nll.xuanzx.com

Ruby: a && b || !c
来源：http://dhv.zhongyouzk.top

C#:   a && b || !c
来源：http://oqm.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://ljr.jyoumei.cn

Py:   if not data: return
来源：http://qth.hammf.cn

PHP:  if (!$data) { return; }
来源：http://nxb.chenlongwang.top

JS:   if (!data) return;
来源：http://fxy.yongpay.top

TS:   if (!data) return;
来源：http://glz.ydjk.org.cn

Java: if (data == null) return;
来源：http://gbb.9152youxi.cn

Go:   if data == nil { return }
来源：http://ccp.hammf.cn

Ruby: return if data.nil?
来源：http://xzh.gzhubu.top

C#:   if (data == null) return;
来源：http://dri.bjfxy.top

================================================================================
来源：http://bxw.wangshuangyany.cn

C. 函数与作用域
来源：http://ifj.bjfxy.top

================================================================================
来源：http://kpn.zdqjudy.top

[C01] 定义函数
来源：http://jdy.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://tbn.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qee.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://tbc.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvg.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gnb.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://idc.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://nmn.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pbo.cdnleiting.top

[C02] 默认参数
来源：http://njo.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://vtt.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ukz.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://djw.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xfu.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kvz.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ibx.sweek.top

Ruby: def greet(name = "World") = name
来源：http://yog.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://lkq.tarul.cn

[C03] 可变参数
来源：http://sfk.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://vij.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dui.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ekt.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wjj.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yjp.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ihm.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://esa.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ayf.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://iuv.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://edt.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ewq.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pcx.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jlj.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://jdj.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://tyc.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://wdx.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://mel.smart0.xyz

[C05] 返回多个值
来源：http://kxx.fehbvm.com

Py:   return a, b
来源：http://hfq.tianlin.xyz

PHP:  return [$a, $b];
来源：http://jun.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wsu.ehwqpu.com

TS:   return { a, b };
来源：http://uer.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xgh.hnxiangtu.top

Go:   return a, b
来源：http://sjz.zhongyouzk.top

Ruby: return a, b
来源：http://nno.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://qak.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://rqo.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://max.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xty.ybcxt.top

JS:   const square = x => x * x;
来源：http://owj.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://ezo.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ecg.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://gix.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://puc.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://hzm.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://waj.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ihp.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cqd.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://otz.tarul.cn

TS:   arr.map(String)
来源：http://puw.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qvq.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iph.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://ujk.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fjv.fzhhl.top

[C08] 闭包
来源：http://lyy.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qkk.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eje.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gjx.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jdt.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kil.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nil.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gli.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gey.shangyingyoupin.top

[C09] 递归
来源：http://ezg.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lxv.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ghm.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fso.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnw.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://agt.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wxz.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kqu.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://moj.jinghuilouyu.cn

[C10] 变量作用域
来源：http://uvq.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cmr.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fgy.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pyk.smart0.xyz

TS:   同 JS
来源：http://qsg.gotoacloud.top

Java: 方法内为块级作用域
来源：http://gwx.xuanzx.com

Go:   花括号块级作用域
来源：http://wpg.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gel.jqgufenzy.top

C#:   块级作用域
来源：http://hqc.yj20258888.top

[C11] 模块导入与导出
来源：http://gzx.daria6918.cn

Py:   from module import func
来源：http://hph.birdmap.top

PHP:  require "file.php";  或 use App\Service;
来源：http://apz.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iwf.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tmb.yuanzhike.top

Java: import java.util.List;
来源：http://ddi.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gvh.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://rzp.hongshengwenyu.top

C#:   using System.Text;
来源：http://rmh.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://hmq.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://wnm.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://ahs.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://upx.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://bnj.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://smj.shangyingyoupin.top


<!-- 参考信息 -->