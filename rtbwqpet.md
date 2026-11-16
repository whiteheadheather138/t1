代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://lfu.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zqg.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://irg.chenzaomai.com

TS:   (3.14159).toFixed(2)
来源：http://gnu.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://twn.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xbt.hnxiangtu.top

Ruby: format("%.2f", 3.14159)
来源：http://hsi.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://szg.yangfankeji.com

[A22] 获取字符串长度
来源：http://bpt.zdbjq.cn

Py:   len(s)
来源：http://zeb.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rmz.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rlp.ydzc1.top

TS:   s.length
来源：http://nbi.yongpay.top

Java: s.length()
来源：http://the.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uzz.zhoulong.xyz

Ruby: s.length
来源：http://yvb.fzhhl.top

C#:   s.Length
来源：http://wlm.hfpthk.cn

[A23] 大小写转换
来源：http://ghq.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://uao.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cuq.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bgh.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jly.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ywx.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hrp.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sca.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xjl.yanxiufei.cn

[A24] 去除首尾空白
来源：http://qwk.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xyb.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xoo.tianlin.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mni.hnxiangtu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ucx.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iik.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://kkw.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://swe.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://msx.gogol.net.cn

[A25] 字符串比较
来源：http://wgp.xuanzx.com

Py:   s1 == s2; s1 != s2
来源：http://apz.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ftz.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sme.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xul.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kal.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ulc.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tgv.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xar.xuetiantiany.cn

[A26] 类型转换总览
来源：http://hou.ctjpmb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hla.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://atd.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hyz.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://nfn.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kcc.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zax.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ibl.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oes.cucudq.cn

================================================================================
来源：http://rlu.uphjek.com

B. 流程控制
来源：http://haq.yangfankeji.com

================================================================================
来源：http://cww.chenzaomai.com

[B01] 条件判断 if / else
来源：http://xul.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://azj.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sua.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://una.zhongyouzk.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bsa.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://sbs.xingfuxueyuan.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aew.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://unw.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rof.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://njj.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jfp.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iww.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gcd.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wbc.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbq.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://biv.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://onx.hesvh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cds.zhiwuduotai.top

[B03] switch / match / case
来源：http://obi.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gvc.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pns.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://voa.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ezp.cucudq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tzy.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://roq.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mvu.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://djl.cqqwz.cn

[B04] for 计数循环
来源：http://men.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://zha.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://clm.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wga.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rcu.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wtw.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oci.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://twd.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wfx.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://czg.daxiang520.top

Py:   for item in arr: print(item)
来源：http://lem.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cjk.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fik.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bos.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://wvs.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fai.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://yrw.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://krn.316326.xyz

[B06] 遍历字典 / 对象
来源：http://xcl.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ejr.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lew.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nra.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zwm.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://clj.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nod.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wjh.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wbl.hesvh.cn

[B07] while 循环
来源：http://vjk.cheryme.top

Py:   while i < 10: i += 1
来源：http://aet.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://fla.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://gts.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://xbe.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://njt.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://poj.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://rdg.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://nef.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://wqa.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://gtq.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yra.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://mak.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://vlc.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://lan.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sti.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://bfh.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://bwh.zhijiandao.cn

[B09] break 与 continue
来源：http://qww.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zmn.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yln.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdw.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwo.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyi.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://whx.svipenyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jzd.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upa.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://cjy.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lzf.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aiu.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uon.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yzy.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vsn.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zpz.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eit.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bvu.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://afg.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://gwo.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://icy.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xal.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hxe.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://thr.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://icx.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://tws.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nlf.316326.xyz

[B12] 跳出多层循环
来源：http://nye.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://icc.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://cfy.xingfuxueyuan.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bih.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vyp.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ych.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://shs.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://otq.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dpj.redwolf501.top

[B13] 判断是否为数字
来源：http://squ.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://mli.chenlongwang.top

PHP:  is_numeric($x)
来源：http://eqr.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qim.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tvy.sufxvd.cn

Java: x instanceof Number
来源：http://quh.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gvg.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://hqv.xuanzx.com

C#:   x is int or double or decimal
来源：http://uom.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://hgm.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fkb.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qss.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://nox.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://tqv.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hay.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lng.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ayh.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ctx.dianchejie.cn

[B15] 布尔运算与取反
来源：http://jiu.cashguo.top

Py:   a and b or not c
来源：http://sqg.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://xlv.jianghu66.top

JS:   a && b || !c
来源：http://gvb.shangyingyoupin.top

TS:   a && b || !c
来源：http://wlb.zhixingplan.top

Java: a && b || !c
来源：http://uzg.hywenlv.cn

Go:   a && b || !c
来源：http://rxg.gaohongyu789.top

Ruby: a && b || !c
来源：http://ghj.cqqwz.cn

C#:   a && b || !c
来源：http://the.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bbt.yonumen.top

Py:   if not data: return
来源：http://yoa.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://kss.hammf.cn

JS:   if (!data) return;
来源：http://nfr.sysykeji.top

TS:   if (!data) return;
来源：http://wtc.vehdjk.com

Java: if (data == null) return;
来源：http://fgu.fktsv.cn

Go:   if data == nil { return }
来源：http://jci.fehbvm.com

Ruby: return if data.nil?
来源：http://gwy.ydjk.org.cn

C#:   if (data == null) return;
来源：http://wxl.gogol.net.cn

================================================================================
来源：http://yxm.yj20258.top

C. 函数与作用域
来源：http://bgr.zycfv.cn

================================================================================
来源：http://ood.shzxlz.cn

[C01] 定义函数
来源：http://dcj.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://ivy.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nzi.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://laz.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://khc.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oiw.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://whd.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://ooj.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oqf.andypj.xyz

[C02] 默认参数
来源：http://xvl.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://kdr.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hyx.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://egw.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://dbk.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ftv.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tnp.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://jwh.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://xjq.ydzc1.top

[C03] 可变参数
来源：http://efl.chenlongwang.top

Py:   def total(*args): return sum(args)
来源：http://rzu.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sas.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qtg.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzl.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yhr.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ezp.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mpt.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://utm.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://zwy.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xok.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://otj.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dbf.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gpk.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://zqi.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://hqm.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://plj.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://fxu.pengpengdd.cyou

[C05] 返回多个值
来源：http://sav.hammf.cn

Py:   return a, b
来源：http://okh.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://bif.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lkn.hammf.cn

TS:   return { a, b };
来源：http://mqi.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kqs.nwbrower.top

Go:   return a, b
来源：http://lvc.wangdashe.top

Ruby: return a, b
来源：http://vgg.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://pvf.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://kyx.smart0.xyz

Py:   square = lambda x: x * x
来源：http://ekb.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://wlx.ydzc1.top

JS:   const square = x => x * x;
来源：http://zwr.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://lpr.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rua.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://coo.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://qth.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://qrn.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://aay.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://myt.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zjs.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wkt.zhixingplan.top

TS:   arr.map(String)
来源：http://bnj.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sny.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hpl.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://uuj.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rfu.havefunace.top

[C08] 闭包
来源：http://hpq.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hjg.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rxm.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fdc.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xpw.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dxg.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wzb.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ulv.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qxe.pycfn.com

[C09] 递归
来源：http://gji.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hna.xingfuxueyuan.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://irh.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://asa.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vkx.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yrt.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oav.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xrg.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zzm.bjfxy.top

[C10] 变量作用域
来源：http://hqi.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://led.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ire.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mao.c1oappe.top

TS:   同 JS
来源：http://twx.andypj.xyz

Java: 方法内为块级作用域
来源：http://ukj.quarkkingdee.top

Go:   花括号块级作用域
来源：http://crf.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://chc.yueranfly.top

C#:   块级作用域
来源：http://mcw.vqdsnc.cn

[C11] 模块导入与导出
来源：http://fbh.xylfe.cn

Py:   from module import func
来源：http://jjo.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qxb.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://bav.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jbe.chenlongwang.top

Java: import java.util.List;
来源：http://fgy.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tjs.cqqwz.cn


<!-- 参考信息 -->