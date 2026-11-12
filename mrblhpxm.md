代发 wailian999

[A22] 获取字符串长度
来源：http://znn.zdbjq.cn

Py:   len(s)
来源：http://ura.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ivy.cdnleiting.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cdd.yueranfly.top

TS:   s.length
来源：http://bap.quarkkingdee.top

Java: s.length()
来源：http://uiy.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vbd.andypj.xyz

Ruby: s.length
来源：http://jzu.fengsongda.top

C#:   s.Length
来源：http://qui.hysaishi.cn

[A23] 大小写转换
来源：http://eep.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://igg.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lep.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xhi.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vci.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lqc.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://svz.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ged.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fms.vqdsnc.cn

[A24] 去除首尾空白
来源：http://cia.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oot.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sir.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dth.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cdf.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qbg.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://evt.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ivb.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yau.guowangkeji.top

[A25] 字符串比较
来源：http://uzx.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://gjd.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yjt.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://opb.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ofi.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://efw.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ped.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rnq.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yxy.wangshuangyany.cn

[A26] 类型转换总览
来源：http://gyq.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fza.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ogt.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qeu.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://loq.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ioj.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://reo.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gow.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bmo.jqgufenzy.top

================================================================================
来源：http://gfb.chenlongwang.top

B. 流程控制
来源：http://evj.gotoacloud.top

================================================================================
来源：http://lnv.sweek.top

[B01] 条件判断 if / else
来源：http://xiv.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://foq.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wwp.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tup.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bma.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kln.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tox.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hfp.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hch.hesvh.cn

[B02] 多分支 else if / elif
来源：http://wrg.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pmu.gogol.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sey.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://teu.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbj.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ima.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ogq.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kep.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://opu.dashuyun.cn

[B03] switch / match / case
来源：http://shx.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uqf.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pdj.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yvw.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wem.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qwx.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bwc.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://anu.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aii.c1oappe.top

[B04] for 计数循环
来源：http://xit.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://tfi.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mmo.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ibu.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ena.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ays.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://axr.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://gqk.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xtr.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://gbu.yj20258888.top

Py:   for item in arr: print(item)
来源：http://yeq.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rom.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://lyk.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ivm.hysaishi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://upv.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lek.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://dfb.pycfn.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vtw.uphjek.com

[B06] 遍历字典 / 对象
来源：http://yyj.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kyh.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yhf.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iux.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xxf.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://foo.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fnz.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://otm.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://spj.feifeiyinyue.top

[B07] while 循环
来源：http://wdj.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://tch.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://etj.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://jix.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://uca.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://dao.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://shp.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://ife.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://hjl.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://ygh.yj202588.top

Py:   # 无 do-while：用 while True + break
来源：http://jkm.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tzw.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://mlp.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://pde.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://vcd.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://udw.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://yqb.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://mep.ppjwa.cn

[B09] break 与 continue
来源：http://yet.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ueb.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ucx.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydy.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://znt.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtq.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oye.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gaq.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bej.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://oyv.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cdq.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pnx.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vbg.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zip.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jbw.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vqr.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rvp.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fef.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://oai.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://lxs.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://btx.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://znj.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxb.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hnj.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nlf.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://tgm.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rro.snrcjt.cn

[B12] 跳出多层循环
来源：http://kag.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://njn.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ieo.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nki.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vma.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gqd.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fbl.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://duz.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aou.xuanzx.com

[B13] 判断是否为数字
来源：http://jzk.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://jzh.yangfankeji.com

PHP:  is_numeric($x)
来源：http://fkr.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bji.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://icn.yongpay.top

Java: x instanceof Number
来源：http://hig.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ibo.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://qms.jianghu66.top

C#:   x is int or double or decimal
来源：http://msr.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://vzr.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qqf.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://liw.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://jje.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://fep.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://kuc.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://agh.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://hvx.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vql.yonumen.top

[B15] 布尔运算与取反
来源：http://xwg.sxryk.cn

Py:   a and b or not c
来源：http://fsw.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://yrl.nwbrower.top

JS:   a && b || !c
来源：http://sru.jlsjyb.cn

TS:   a && b || !c
来源：http://odu.ppjwa.cn

Java: a && b || !c
来源：http://hho.jlsjyb.cn

Go:   a && b || !c
来源：http://jax.feifeiyinyue.top

Ruby: a && b || !c
来源：http://jeu.jinqigfzy.top

C#:   a && b || !c
来源：http://xmn.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://jpt.xylfe.cn

Py:   if not data: return
来源：http://vdk.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://wtc.zdbjq.cn

JS:   if (!data) return;
来源：http://sul.sufxvd.cn

TS:   if (!data) return;
来源：http://fmi.yuanzhike.top

Java: if (data == null) return;
来源：http://law.vqdsnc.cn

Go:   if data == nil { return }
来源：http://ees.guannengcc.top

Ruby: return if data.nil?
来源：http://gja.iojbl.cn

C#:   if (data == null) return;
来源：http://wcu.yj202588.top

================================================================================
来源：http://ohy.yanxiufei.cn

C. 函数与作用域
来源：http://gct.gogol.net.cn

================================================================================
来源：http://pda.yj20258888.top

[C01] 定义函数
来源：http://uen.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://sbk.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aiz.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://lic.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://use.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pjz.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pyr.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://nbl.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ckf.gotoacloud.top

[C02] 默认参数
来源：http://spi.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://cfh.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vsg.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://xas.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kmq.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sfg.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qps.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://rtr.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://bgn.gotoacloud.top

[C03] 可变参数
来源：http://rco.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://hew.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://coj.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcn.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtv.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mnh.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://was.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://axg.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ytd.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://whf.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iqw.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mml.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://enc.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mmq.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://ron.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://bre.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://kgl.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://qxz.aizwys.cn

[C05] 返回多个值
来源：http://grp.tianlin.xyz

Py:   return a, b
来源：http://wpp.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://fab.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://hfd.hongshengwenyu.top

TS:   return { a, b };
来源：http://uca.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hgl.cashguo.top

Go:   return a, b
来源：http://osl.tianlin.xyz

Ruby: return a, b
来源：http://vof.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://qvk.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://din.yueranfly.top

Py:   square = lambda x: x * x
来源：http://fws.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sjw.xinyue.icu

JS:   const square = x => x * x;
来源：http://nmj.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://dqh.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hhz.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://jhv.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://ryg.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://ewh.yj20258.top

[C07] 把函数作为参数传入
来源：http://njx.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bat.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ajm.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ttt.zdqjudy.top

TS:   arr.map(String)
来源：http://jdw.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cdv.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://obb.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://arj.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://flz.yfazqb.com

[C08] 闭包
来源：http://wpb.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lws.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ovd.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yfc.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rtc.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jdh.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nhb.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cwv.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wgu.hywenlv.cn

[C09] 递归
来源：http://afr.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dec.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zab.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aqx.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rut.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dit.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uke.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tsu.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qui.meibo888.top

[C10] 变量作用域
来源：http://cis.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xjx.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vqh.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahd.pycfn.com

TS:   同 JS
来源：http://vie.bbcook.cn

Java: 方法内为块级作用域
来源：http://agg.yuxming.cn

Go:   花括号块级作用域
来源：http://ptl.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qjh.jinqigfzy.top

C#:   块级作用域
来源：http://clr.zhixingplan.top

[C11] 模块导入与导出
来源：http://gta.ctjpmb.com

Py:   from module import func
来源：http://eja.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://crr.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cuf.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://clb.xuetiantiany.cn

Java: import java.util.List;
来源：http://ffs.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jem.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://amu.ehwqpu.com

C#:   using System.Text;
来源：http://dod.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://dkp.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://zqp.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://otj.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://rao.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://uqq.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xjn.sxryk.cn


<!-- 参考信息 -->