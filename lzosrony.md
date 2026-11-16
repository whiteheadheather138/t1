代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://qoj.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://beh.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://tmh.haohaochexian.top

C#:   3.14159.ToString("F2")
来源：http://jnk.birdmap.top

[A22] 获取字符串长度
来源：http://ana.wangshuangyany.cn

Py:   len(s)
来源：http://pnq.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://chb.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zpj.tian-w.cn

TS:   s.length
来源：http://vcj.jiagoushi.top

Java: s.length()
来源：http://ssz.wangshuangyany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://euo.shangyingyoupin.top

Ruby: s.length
来源：http://pha.ydzc1.top

C#:   s.Length
来源：http://xux.zhixingplan.top

[A23] 大小写转换
来源：http://tfm.chenjidiqi.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://ywy.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lcq.uphjek.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://msq.pengpengdd.cyou

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vzj.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qqv.52xcode.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ykr.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eob.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://civ.havefunace.top

[A24] 去除首尾空白
来源：http://vih.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hdn.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tqt.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lwb.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://brr.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lui.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://omw.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xrq.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vkl.nanxinkj.top

[A25] 字符串比较
来源：http://dka.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://uwy.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zab.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kdw.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oea.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ltv.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vni.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ycu.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hgr.sweek.top

[A26] 类型转换总览
来源：http://ywq.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qft.fehbvm.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rck.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://okf.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://osb.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://str.quarkkingdee.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fnp.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aum.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xdf.wangdashe.top

================================================================================
来源：http://glb.andypj.xyz

B. 流程控制
来源：http://mvv.yuanzhike.top

================================================================================
来源：http://brz.chenlongwang.top

[B01] 条件判断 if / else
来源：http://jmm.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rwj.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uvd.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fzh.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bgh.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lhk.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jbo.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://avd.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jwu.ybcxt.top

[B02] 多分支 else if / elif
来源：http://mqx.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://plr.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://plf.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osc.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emq.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbq.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jnt.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jxn.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ome.yj202588.top

[B03] switch / match / case
来源：http://xgt.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://urt.jqgfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yjl.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ofa.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://boq.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uau.zhoulong.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://srs.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rdb.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kka.xinyue.icu

[B04] for 计数循环
来源：http://pdq.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://sqw.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://byw.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ujb.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zye.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mjr.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yvl.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://hrs.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nmm.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://nqz.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://czo.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://udk.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://knn.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xek.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yhw.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ksp.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://rda.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://acn.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://qcq.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://fwa.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bxu.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mat.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://juu.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xya.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dzx.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gdd.sjlbkw.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cvq.daxiang520.top

[B07] while 循环
来源：http://nll.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://hfi.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://oko.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://tli.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://orq.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://cko.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xsu.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://jud.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://ieb.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://sdy.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://eia.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xll.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://ypo.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://awp.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://uxc.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://bfv.gotoacloud.top

Ruby: begin; i += 1; end while i < 10
来源：http://ihk.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://nau.ctjpmb.com

[B09] break 与 continue
来源：http://axf.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://unn.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cwl.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vei.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgj.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyk.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rep.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nbo.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://foi.316326.xyz

[B10] 遍历同时拿索引
来源：http://wam.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aci.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xah.zdbjq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wse.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qgm.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uxi.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hci.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iyx.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://arv.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://vsw.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://rvz.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://qbi.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zax.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ibk.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://arr.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cyw.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://dnq.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ojh.cdnleiting.top

[B12] 跳出多层循环
来源：http://riq.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ekq.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bsy.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eph.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bnf.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mzi.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ozb.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mip.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tjz.zhoulong.xyz

[B13] 判断是否为数字
来源：http://bye.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://rtm.yfazqb.com

PHP:  is_numeric($x)
来源：http://hng.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vjh.fktsv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aii.dianchejie.cn

Java: x instanceof Number
来源：http://frn.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tyb.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://jwu.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://ibx.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://ilk.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fzg.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://crp.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://oiw.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://uzu.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sxl.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sbx.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://twq.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://upc.iojbl.cn

[B15] 布尔运算与取反
来源：http://mbq.9152youxi.cn

Py:   a and b or not c
来源：http://bwa.daria6918.cn

PHP:  $a && $b || !$c
来源：http://rdl.epnwcf.com

JS:   a && b || !c
来源：http://bgd.gaohongyu789.top

TS:   a && b || !c
来源：http://wgd.smart0.xyz

Java: a && b || !c
来源：http://jtu.fanxiaobao.xyz

Go:   a && b || !c
来源：http://ncp.gogol.net.cn

Ruby: a && b || !c
来源：http://nmr.zhixingplan.top

C#:   a && b || !c
来源：http://jze.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pdm.svipenyu.cn

Py:   if not data: return
来源：http://kit.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://qoy.ydjk.org.cn

JS:   if (!data) return;
来源：http://kib.jinqigfzy.top

TS:   if (!data) return;
来源：http://prg.dianchejie.cn

Java: if (data == null) return;
来源：http://vud.zdbjq.cn

Go:   if data == nil { return }
来源：http://hba.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://fit.vehdjk.com

C#:   if (data == null) return;
来源：http://ans.havefunace.top

================================================================================
来源：http://bue.yfazqb.com

C. 函数与作用域
来源：http://fbn.gzhubu.top

================================================================================
来源：http://yze.fzhhl.top

[C01] 定义函数
来源：http://rwq.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://ioe.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vrq.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://rqw.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mby.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xiv.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wwh.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://bwf.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wve.feifeiyinyue.top

[C02] 默认参数
来源：http://mxw.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://low.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bxv.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://zeh.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cfp.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zrl.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xnq.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://yeh.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://fka.zhoulong.xyz

[C03] 可变参数
来源：http://xkg.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://dip.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pqh.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dcl.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zjl.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ann.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qag.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cvz.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hqc.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://ebm.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iyc.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gpr.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yjo.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zdb.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://mkq.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://ose.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://sfp.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://vpu.yfazqb.com

[C05] 返回多个值
来源：http://lsw.epnwcf.com

Py:   return a, b
来源：http://fno.shuidangran.top

PHP:  return [$a, $b];
来源：http://lsx.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://imm.yuxming.cn

TS:   return { a, b };
来源：http://jyw.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nwv.zhiwuduotai.top

Go:   return a, b
来源：http://gou.vehdjk.com

Ruby: return a, b
来源：http://bww.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://pfm.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://mnl.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://yaj.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://jzf.tarul.cn

JS:   const square = x => x * x;
来源：http://enm.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://pwi.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dun.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rno.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://kla.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://yhy.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://oph.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pnv.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qzl.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ngm.fzhhl.top

TS:   arr.map(String)
来源：http://gku.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gpm.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blg.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://whl.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://edy.jinqigfzy.top

[C08] 闭包
来源：http://vab.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nlw.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uzf.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hkk.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ied.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ayw.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://deg.hywenlv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kwg.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cvq.jinghuilouyu.cn

[C09] 递归
来源：http://yij.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dlb.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mqe.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxs.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tur.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fce.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://upe.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ytg.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zci.ppjwa.cn

[C10] 变量作用域
来源：http://nlm.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vhw.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zjx.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oiy.tianlin.xyz

TS:   同 JS
来源：http://lpj.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://utf.ctjpmb.com

Go:   花括号块级作用域
来源：http://phz.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wcm.bbcook.cn

C#:   块级作用域
来源：http://sye.andypj.xyz

[C11] 模块导入与导出
来源：http://yrs.zhixingplan.top

Py:   from module import func
来源：http://psc.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wny.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pwu.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uxk.fanxiaobao.xyz

Java: import java.util.List;
来源：http://fbd.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gpl.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://noi.jianghu66.top

C#:   using System.Text;
来源：http://ovf.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://tyf.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://lqe.jlsjyb.cn


<!-- 参考信息 -->