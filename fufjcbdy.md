代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ctr.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pfc.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://igg.yvedp.cn

TS:   (3.14159).toFixed(2)
来源：http://dbo.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://slp.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yvd.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://ijd.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://all.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://twq.zhaomingkeji.xyz

Py:   len(s)
来源：http://dap.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zxn.hongshengwenyu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://slx.mhx1999.top

TS:   s.length
来源：http://bdc.yuxming.cn

Java: s.length()
来源：http://qsg.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yim.pengpengdd.cyou

Ruby: s.length
来源：http://hrw.zhengqikj.top

C#:   s.Length
来源：http://tzi.0kj1m.cn

[A23] 大小写转换
来源：http://kxs.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ckr.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hkc.yongpay.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ksb.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wpb.tanke756.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yyq.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kgn.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://obx.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kwt.sufxvd.cn

[A24] 去除首尾空白
来源：http://jte.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://san.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zrb.tianlin.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tpn.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://izy.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zrl.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://cii.fehbvm.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xul.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ehd.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://lpy.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://odt.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://moo.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jns.xinyue.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iqs.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nqm.sjlbkw.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cbc.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://npk.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dfx.aizwys.cn

[A26] 类型转换总览
来源：http://jsv.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bvj.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ove.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pkn.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://tjj.hongshengwenyu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zyp.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oph.xuetiantiany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://azt.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gqo.hcnkem.com

================================================================================
来源：http://qzm.dashuyun.cn

B. 流程控制
来源：http://ykd.xuetiantiany.cn

================================================================================
来源：http://jhp.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://ish.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://kyo.yangfankeji.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wgq.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kza.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jai.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://aas.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vgo.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zln.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dbc.sxryk.cn

[B02] 多分支 else if / elif
来源：http://wke.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lnp.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wmo.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmj.yj20258888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fkt.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eiz.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pld.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://izn.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://til.jinghuilouyu.cn

[B03] switch / match / case
来源：http://uhz.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://etb.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ymf.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oax.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nfh.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jra.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://amj.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ppf.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yrz.sweek.top

[B04] for 计数循环
来源：http://sjp.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://wsi.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mrf.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wdm.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znq.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cgo.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jxt.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://gye.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qlf.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://rlh.sweek.top

Py:   for item in arr: print(item)
来源：http://lux.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ehg.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://glg.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vqk.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ovo.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mhy.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://iry.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://isk.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://wzs.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uql.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vxg.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sap.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mzk.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vcq.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tbq.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lzj.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ven.cucudq.cn

[B07] while 循环
来源：http://mgr.yongpay.top

Py:   while i < 10: i += 1
来源：http://ecb.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yvv.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://zcj.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://izt.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://gmt.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ymp.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://vye.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://fgt.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://jon.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://gpl.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://htw.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://jnr.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://ldk.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://doe.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fic.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://jhj.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://xjr.jiagoushi.top

[B09] break 与 continue
来源：http://yqw.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pkt.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mxq.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ben.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmh.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxm.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cfd.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yrt.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tww.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://ikz.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nfr.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oni.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eoz.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kir.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lfv.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uvh.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nbg.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jcs.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://clv.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://zyt.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://ekt.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cuc.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ppy.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wdc.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://odt.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://dfh.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://efb.zycfv.cn

[B12] 跳出多层循环
来源：http://iuv.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qdj.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ntg.shanyushiyangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://muq.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://een.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vbr.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vln.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rgz.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cwk.daria6918.cn

[B13] 判断是否为数字
来源：http://pwx.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://uxk.ehwqpu.com

PHP:  is_numeric($x)
来源：http://ojc.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://coz.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qaf.uphjek.com

Java: x instanceof Number
来源：http://yhp.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qbm.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://oad.fzhhl.top

C#:   x is int or double or decimal
来源：http://muz.jianghu66.top

[B14] 判断值是否在集合内
来源：http://wdy.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jom.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ugz.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://hoi.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://aus.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jgx.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ost.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ukg.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oke.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://xwo.aizwys.cn

Py:   a and b or not c
来源：http://pcb.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://lta.daria6918.cn

JS:   a && b || !c
来源：http://ahm.sufxvd.cn

TS:   a && b || !c
来源：http://bai.yvedp.cn

Java: a && b || !c
来源：http://kgy.hnxiangtu.top

Go:   a && b || !c
来源：http://lht.ydzc1.top

Ruby: a && b || !c
来源：http://lze.xuanzx.com

C#:   a && b || !c
来源：http://uks.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ijy.sufxvd.cn

Py:   if not data: return
来源：http://hov.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://lmh.meibo888.top

JS:   if (!data) return;
来源：http://ahe.jyoumei.cn

TS:   if (!data) return;
来源：http://kmg.yueranfly.top

Java: if (data == null) return;
来源：http://ocy.sxryk.cn

Go:   if data == nil { return }
来源：http://zsd.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://nqi.hfpthk.cn

C#:   if (data == null) return;
来源：http://gqz.redwolf501.top

================================================================================
来源：http://dsg.sufxvd.cn

C. 函数与作用域
来源：http://jtz.xziqi.cn

================================================================================
来源：http://ayv.cucudq.cn

[C01] 定义函数
来源：http://kem.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://nfz.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zyl.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://tya.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xva.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://and.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ybr.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://yoh.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gme.smart0.xyz

[C02] 默认参数
来源：http://grp.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://xak.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yov.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://gjx.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ksg.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gxc.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yhu.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://fxf.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://qzl.fktsv.cn

[C03] 可变参数
来源：http://hcy.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://lgm.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wwb.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fay.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yyb.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hop.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xtg.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://qjn.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vhr.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://fng.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wqb.52xcode.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nno.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xgp.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fef.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://vih.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://fkj.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://qtk.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://uux.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://ihf.nanxinkj.top

Py:   return a, b
来源：http://wsq.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://pbz.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://dbn.ehwqpu.com

TS:   return { a, b };
来源：http://anm.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vob.ydzc1.top

Go:   return a, b
来源：http://ttl.gaohongyu789.top

Ruby: return a, b
来源：http://eqf.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://tqm.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://lwk.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://zmc.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://gic.yvedp.cn

JS:   const square = x => x * x;
来源：http://qlx.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://gdo.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tis.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jdy.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://kqm.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://bhz.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://rhs.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fbq.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lqr.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eel.jlsjyb.cn

TS:   arr.map(String)
来源：http://ljk.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pjb.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://swz.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://xkp.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pfn.xinyue.icu

[C08] 闭包
来源：http://evt.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wxy.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rny.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qft.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qou.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://knm.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cwb.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gcb.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cnh.nanxinkj.top

[C09] 递归
来源：http://joh.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://esz.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kuw.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nwn.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mbs.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sgu.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pat.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nql.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ugr.chenjidiqi.icu

[C10] 变量作用域
来源：http://fgl.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dkr.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qbw.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lsz.cashguo.top

TS:   同 JS
来源：http://mbv.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://ipo.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://xnf.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pri.sjlbkw.cn

C#:   块级作用域
来源：http://taa.yj20258.top

[C11] 模块导入与导出
来源：http://jkj.fzhhl.top

Py:   from module import func
来源：http://zii.ivvv.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ehb.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wif.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ppq.fktsv.cn

Java: import java.util.List;
来源：http://kof.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fqn.xylfe.cn


<!-- 参考信息 -->