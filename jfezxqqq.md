代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://kyo.xinyue.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jay.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://izq.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://zgf.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://wfb.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lpz.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://qsq.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://shr.cashguo.top

[A22] 获取字符串长度
来源：http://vaq.hfpthk.cn

Py:   len(s)
来源：http://hvg.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dls.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oxt.nanxinkj.top

TS:   s.length
来源：http://buc.ivvv.top

Java: s.length()
来源：http://gts.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wxr.jqgufenzy.top

Ruby: s.length
来源：http://dtc.xingfuxueyuan.xyz

C#:   s.Length
来源：http://lzy.sxryk.cn

[A23] 大小写转换
来源：http://rto.gogol.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kcq.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ael.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uju.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qgm.316326.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eyr.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ovx.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dyr.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://coe.yangfankeji.com

[A24] 去除首尾空白
来源：http://ljw.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://giu.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ylk.epnwcf.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uqc.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zxz.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bqc.cdnleiting.top

Go:   strings.TrimSpace(s)
来源：http://myt.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rvj.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dev.yj20258.top

[A25] 字符串比较
来源：http://ruo.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://uyb.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://opu.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://crf.gogol.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nxh.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tze.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zeh.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dth.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qyu.316326.xyz

[A26] 类型转换总览
来源：http://dlm.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kzk.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ihz.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qcs.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://jrw.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pxi.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pdm.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mjj.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yzp.xinyue.icu

================================================================================
来源：http://unw.xuanzx.com

B. 流程控制
来源：http://aij.nanxuanxn.top

================================================================================
来源：http://cjt.yuxming.cn

[B01] 条件判断 if / else
来源：http://vfn.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rlg.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jux.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gch.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mzs.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qng.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gvh.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uyr.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ujb.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://gfp.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jky.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tro.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bye.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gpk.jinqigufen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwv.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lyp.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mef.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uif.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://tkn.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rmt.hysaishi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://enl.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mmn.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjq.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pfm.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vei.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xzd.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wfc.zhijiandao.cn

[B04] for 计数循环
来源：http://ygl.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://mbp.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uwx.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://spr.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xeq.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://khq.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qth.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://btb.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kdd.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://mxi.wangdashe.top

Py:   for item in arr: print(item)
来源：http://ztu.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qoz.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gdr.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nwi.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://hhm.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cbw.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://qgv.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xps.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://qoj.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pxj.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aoa.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bqt.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gmr.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbt.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wsw.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jdq.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nme.ydjk.org.cn

[B07] while 循环
来源：http://vwy.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://qxd.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rcq.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://xcj.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://tkm.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://mor.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zya.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://npa.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://wgf.316326.xyz

[B08] do-while（至少执行一次）
来源：http://iss.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://ane.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pbx.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://nau.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://dfe.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://cxq.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xgp.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jzc.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://ipi.tian-w.cn

[B09] break 与 continue
来源：http://mcq.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ygs.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bmh.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxd.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vym.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvn.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ixb.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://trq.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phc.epnwcf.com

[B10] 遍历同时拿索引
来源：http://axr.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tja.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rws.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ttw.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xbx.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kir.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://krm.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tyb.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uww.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://mwa.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://ehi.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://zop.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://orm.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tiw.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lnu.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rgd.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://tum.vehdjk.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zxd.havefunace.top

[B12] 跳出多层循环
来源：http://oxu.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ofz.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://upv.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvm.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kus.iojbl.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yfw.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uff.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jks.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://klu.jinqigfzy.top

[B13] 判断是否为数字
来源：http://uie.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://hwp.zdqjudy.top

PHP:  is_numeric($x)
来源：http://bnx.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yiw.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ivs.wangdashe.top

Java: x instanceof Number
来源：http://jlg.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mqt.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://cya.gzhubu.top

C#:   x is int or double or decimal
来源：http://pil.yuxming.cn

[B14] 判断值是否在集合内
来源：http://cql.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bah.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://elk.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://tmm.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://jim.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vmi.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zhe.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://lhx.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ogc.ydzc1.top

[B15] 布尔运算与取反
来源：http://sgb.xinyue.icu

Py:   a and b or not c
来源：http://gam.sweek.top

PHP:  $a && $b || !$c
来源：http://gio.sjlbkw.cn

JS:   a && b || !c
来源：http://bfq.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://dgq.sjlbkw.cn

Java: a && b || !c
来源：http://uij.cqqwz.cn

Go:   a && b || !c
来源：http://btt.hcnkem.com

Ruby: a && b || !c
来源：http://leu.9152youxi.cn

C#:   a && b || !c
来源：http://ddr.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://hrs.guowangkeji.top

Py:   if not data: return
来源：http://nnp.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://mbk.smart0.xyz

JS:   if (!data) return;
来源：http://qrm.zhijiandao.cn

TS:   if (!data) return;
来源：http://puk.yj20258888.top

Java: if (data == null) return;
来源：http://qvl.cheryme.top

Go:   if data == nil { return }
来源：http://sxn.hnqzz.top

Ruby: return if data.nil?
来源：http://poh.hfpthk.cn

C#:   if (data == null) return;
来源：http://ifr.fktsv.cn

================================================================================
来源：http://rsr.birdmap.top

C. 函数与作用域
来源：http://xui.tian-w.cn

================================================================================
来源：http://dyy.hysaishi.cn

[C01] 定义函数
来源：http://jgj.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://ktp.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lay.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://puk.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sjs.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bqc.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://och.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://nil.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lpv.cashguo.top

[C02] 默认参数
来源：http://rqq.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://qxt.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://vhj.gotoacloud.top

JS:   function greet(name = "World") { return name; }
来源：http://goe.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nly.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lbr.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tpz.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://uur.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://uri.yanxiufei.cn

[C03] 可变参数
来源：http://fii.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://efe.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xmr.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fab.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibw.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xbp.dianchejie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lbr.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://lyv.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kxp.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://hpk.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zcm.jinyuanbaomall.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fsf.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://siv.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mxi.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://hro.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://mqp.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://aty.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://fzl.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://doa.sweek.top

Py:   return a, b
来源：http://lgv.pycfn.com

PHP:  return [$a, $b];
来源：http://bxo.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mgr.vqdsnc.cn

TS:   return { a, b };
来源：http://rqn.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cfb.quarkkingdee.top

Go:   return a, b
来源：http://wvp.hnxiangtu.top

Ruby: return a, b
来源：http://pjd.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ojz.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://moe.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://lqu.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zwk.jqgfzy.top

JS:   const square = x => x * x;
来源：http://qtd.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://rdv.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ucq.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://eiz.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://lhl.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xqz.yonumen.top

[C07] 把函数作为参数传入
来源：http://cus.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bul.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://ced.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jdb.uphjek.com

TS:   arr.map(String)
来源：http://dhl.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rko.zhixingplan.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nca.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://fkd.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://swg.hfpthk.cn

[C08] 闭包
来源：http://erz.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xyj.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xef.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ncr.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qhn.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cka.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ymn.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wql.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sbz.cqqwz.cn

[C09] 递归
来源：http://utd.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://msb.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tci.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dnb.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sit.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mea.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://emm.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fgi.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zxf.fehbvm.com

[C10] 变量作用域
来源：http://qkg.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ucx.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wbe.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tfs.haohaochexian.top

TS:   同 JS
来源：http://kzu.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://ccf.tanke756.top

Go:   花括号块级作用域
来源：http://blv.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://swj.yfazqb.com

C#:   块级作用域
来源：http://azm.jqgfzy.top

[C11] 模块导入与导出
来源：http://pql.xinyue.icu

Py:   from module import func
来源：http://flt.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jjj.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yun.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tev.zhixingplan.top

Java: import java.util.List;
来源：http://awc.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://itk.daxiang520.top


<!-- 参考信息 -->