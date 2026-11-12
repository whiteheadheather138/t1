代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://xkb.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zde.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://mqt.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://yav.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://apk.yuxming.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kfk.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://yon.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://uaq.jlsjyb.cn

[A22] 获取字符串长度
来源：http://fbb.bbcook.cn

Py:   len(s)
来源：http://dsn.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cac.shuidangran.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pdp.9152youxi.cn

TS:   s.length
来源：http://fwx.gogol.net.cn

Java: s.length()
来源：http://rar.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://izu.zdbjq.cn

Ruby: s.length
来源：http://coh.yj20258.top

C#:   s.Length
来源：http://hav.52xcode.cn

[A23] 大小写转换
来源：http://wpx.jinqigufen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://imw.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://edc.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rla.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vce.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zxg.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dbi.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qxj.tian-w.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nwl.yanxiufei.cn

[A24] 去除首尾空白
来源：http://ivw.yueranfly.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qyz.cheryme.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fwi.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://njr.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lnu.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uvy.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://div.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dpn.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tdd.cucudq.cn

[A25] 字符串比较
来源：http://glm.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://yev.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mps.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nhm.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ksc.hongshengwenyu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://weu.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iat.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mfz.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://siv.havefunace.top

[A26] 类型转换总览
来源：http://rqt.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tjn.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tcx.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fxx.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://cas.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gyy.shzxlz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iuz.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://acb.snrcjt.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://byl.0kj1m.cn

================================================================================
来源：http://mkw.shanyushiyangtech.top

B. 流程控制
来源：http://vnc.wangshuangyany.cn

================================================================================
来源：http://hzj.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://rsg.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://mst.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mgz.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sxr.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://obj.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://oek.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gzt.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jev.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vne.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://nzb.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xar.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cmy.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sim.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kba.bjfxy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udg.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xsc.quarkkingdee.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fes.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icf.wangdashe.top

[B03] switch / match / case
来源：http://aty.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rkc.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gvx.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uwk.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyh.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://npi.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pib.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kov.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ebl.fktsv.cn

[B04] for 计数循环
来源：http://xit.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://xlg.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pwz.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vbr.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tou.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ryh.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yhd.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://lve.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ztx.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://npr.hesvh.cn

Py:   for item in arr: print(item)
来源：http://fcf.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mox.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nnw.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://tur.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://psh.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hcr.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://vad.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zvw.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://zew.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hqi.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bkn.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgg.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://arb.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nkj.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bxk.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://osg.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vzi.smart0.xyz

[B07] while 循环
来源：http://jfu.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://thv.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://faq.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://tcd.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://ecw.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://aoi.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gcr.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://htv.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://reu.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://zme.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://pqp.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dmp.jiagoushi.top

JS:   do { i++; } while (i < 10);
来源：http://mzz.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://ctn.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://ots.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://lij.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rlt.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://osu.ydzc1.top

[B09] break 与 continue
来源：http://ybb.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wzy.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vqx.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zac.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://izh.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ens.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ype.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sud.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqs.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://bmm.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kgd.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nho.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ohy.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://okm.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sle.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://azf.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rkj.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mka.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://rto.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://utm.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://zsl.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yaa.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://chc.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://asl.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kmw.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://cuw.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ivv.andypj.xyz

[B12] 跳出多层循环
来源：http://yai.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://apd.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zek.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://llj.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jbc.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cdn.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fhx.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yyf.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nlv.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://how.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://qha.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://ccv.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vfk.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hkx.vqdsnc.cn

Java: x instanceof Number
来源：http://gkr.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wlt.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://snj.ybcxt.top

C#:   x is int or double or decimal
来源：http://jhc.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://fde.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lwi.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cdf.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://uii.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://tat.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ngd.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kqu.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://qdz.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yxt.aibaodan.cn

[B15] 布尔运算与取反
来源：http://nne.hammf.cn

Py:   a and b or not c
来源：http://fpy.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://xna.vehdjk.com

JS:   a && b || !c
来源：http://aed.feifeiyinyue.top

TS:   a && b || !c
来源：http://epo.ydzc1.top

Java: a && b || !c
来源：http://xiz.snrcjt.cn

Go:   a && b || !c
来源：http://zzt.aizwys.cn

Ruby: a && b || !c
来源：http://ovb.feifeiyinyue.top

C#:   a && b || !c
来源：http://zlt.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://zgv.hfpthk.cn

Py:   if not data: return
来源：http://wvi.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://sap.zhiwuduotai.top

JS:   if (!data) return;
来源：http://izw.dianchejie.cn

TS:   if (!data) return;
来源：http://hzp.yonumen.top

Java: if (data == null) return;
来源：http://fwf.sjlbkw.cn

Go:   if data == nil { return }
来源：http://zmx.hnxiangtu.top

Ruby: return if data.nil?
来源：http://ymd.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://uec.yj20258.top

================================================================================
来源：http://svm.jlsjyb.cn

C. 函数与作用域
来源：http://fob.nanxuanxn.top

================================================================================
来源：http://myi.yanxiufei.cn

[C01] 定义函数
来源：http://cei.uphjek.com

Py:   def add(a, b): return a + b
来源：http://bor.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjs.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://jwp.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xjt.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hne.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://djg.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://wkv.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xtf.zhongyouzk.top

[C02] 默认参数
来源：http://itg.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://gzu.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://xlc.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://ogl.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wfq.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jip.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qct.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://chf.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://eyo.shanyushiyangtech.top

[C03] 可变参数
来源：http://jwi.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://iiu.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ksc.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eqr.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nvd.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qyh.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mka.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://pfc.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zuk.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://jwt.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ylm.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hto.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ecy.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cgj.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://zhh.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://sed.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://otl.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://rxw.sweek.top

[C05] 返回多个值
来源：http://zdr.316326.xyz

Py:   return a, b
来源：http://xbv.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://wwi.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ftg.pengpengdd.cyou

TS:   return { a, b };
来源：http://jcd.hesvh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fbc.xingfuxueyuan.xyz

Go:   return a, b
来源：http://nab.jlsjyb.cn

Ruby: return a, b
来源：http://pbb.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://btg.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://rjl.hcnkem.com

Py:   square = lambda x: x * x
来源：http://umi.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://fmc.tianlin.xyz

JS:   const square = x => x * x;
来源：http://ksf.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ncd.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://idy.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://tsx.hnxiangtu.top

Ruby: square = ->(x) { x * x }
来源：http://ldz.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://pld.epnwcf.com

[C07] 把函数作为参数传入
来源：http://xwk.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jrf.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ijd.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qfn.tanke756.top

TS:   arr.map(String)
来源：http://kgg.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://log.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hpq.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://nmo.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dvd.jianghu66.top

[C08] 闭包
来源：http://mbu.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wnk.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://faq.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yyi.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ami.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oxk.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://biw.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wab.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tfl.sjlbkw.cn

[C09] 递归
来源：http://jww.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kvd.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ydv.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nlq.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ayk.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ilk.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xod.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bes.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mrx.yonumen.top

[C10] 变量作用域
来源：http://hsf.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zro.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pil.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://azl.zdqjudy.top

TS:   同 JS
来源：http://ygq.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://aum.jqgufenzy.top

Go:   花括号块级作用域
来源：http://etr.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://urk.mhx1999.top

C#:   块级作用域
来源：http://uiv.aibaodan.cn

[C11] 模块导入与导出
来源：http://ias.chenjidiqi.icu

Py:   from module import func
来源：http://bdh.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qpk.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zhc.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tcu.havefunace.top

Java: import java.util.List;
来源：http://iag.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dil.ctjpmb.com


<!-- 参考信息 -->