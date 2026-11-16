代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://fbk.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nei.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://iog.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://svl.hammf.cn

[A22] 获取字符串长度
来源：http://pad.yuxming.cn

Py:   len(s)
来源：http://jsu.jinqigfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xhh.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kfq.smart0.xyz

TS:   s.length
来源：http://gon.yvedp.cn

Java: s.length()
来源：http://aul.zhijiandao.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iyv.shangyingyoupin.top

Ruby: s.length
来源：http://fer.yanxiufei.cn

C#:   s.Length
来源：http://kbl.dianchejie.cn

[A23] 大小写转换
来源：http://wgu.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bgw.hcnkem.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ceb.shzxlz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zdn.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vid.fanxiaobao.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gjq.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mza.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://omb.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://adi.hysaishi.cn

[A24] 去除首尾空白
来源：http://tii.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pnh.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cyf.nwbrower.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kjo.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://juy.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zqn.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://ogw.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rhj.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nyn.jinqigufen.top

[A25] 字符串比较
来源：http://aki.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://wqd.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ysm.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://egz.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://afl.ydjk.org.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aot.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://piv.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kkm.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xtg.quarkkingdee.top

[A26] 类型转换总览
来源：http://lbt.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jzg.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://szo.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xqb.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://fjc.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jey.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://miz.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zzu.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://adl.gaohongyu789.top

================================================================================
来源：http://wmi.mhx1999.top

B. 流程控制
来源：http://zjh.hongshengwenyu.top

================================================================================
来源：http://yrt.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://vst.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ooi.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yfo.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mib.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xkg.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ssf.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zts.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://whb.tianlin.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://igp.epnwcf.com

[B02] 多分支 else if / elif
来源：http://adl.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ihd.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zad.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blg.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rrn.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://som.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tft.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zzk.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tvm.zhongyouzk.top

[B03] switch / match / case
来源：http://ygz.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mhs.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vdi.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lba.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://smy.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xwq.jqgfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jwn.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fau.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://szl.shuidangran.top

[B04] for 计数循环
来源：http://glr.meibo888.top

Py:   for i in range(10): print(i)
来源：http://uyd.gaohongyu789.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dua.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xeo.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cvq.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xyn.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zlz.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://ywy.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eea.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://iod.vehdjk.com

Py:   for item in arr: print(item)
来源：http://rwh.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ujs.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ixn.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tfn.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://she.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://csm.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://wvi.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hfs.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://ufh.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zmq.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://owl.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tbv.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dao.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uec.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hot.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ejy.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gef.smart0.xyz

[B07] while 循环
来源：http://kcl.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://rap.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dlw.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://dqh.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://hcz.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://wxt.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pjl.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://ypx.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://tzy.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://mlf.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://jah.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sym.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://tor.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://tlh.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://uzm.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://rlj.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://czf.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://giv.xuetiantiany.cn

[B09] break 与 continue
来源：http://adg.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blo.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cqp.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nym.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptu.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxp.ehwqpu.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gkd.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ncf.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smr.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://vae.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rmm.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tgh.feifeiyinyue.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ons.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ujq.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qcr.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wst.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blr.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ljx.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://jrs.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://qwa.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://inv.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hqo.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uyn.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eec.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kbd.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://wfc.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://byn.bbcook.cn

[B12] 跳出多层循环
来源：http://fyp.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bdj.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ruz.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ecr.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wsw.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hat.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dqr.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sgd.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ala.gotoacloud.top

[B13] 判断是否为数字
来源：http://plv.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://rla.jiagoushi.top

PHP:  is_numeric($x)
来源：http://ywc.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ijf.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rrn.jyoumei.cn

Java: x instanceof Number
来源：http://day.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ygg.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://auk.yvedp.cn

C#:   x is int or double or decimal
来源：http://ktv.cashguo.top

[B14] 判断值是否在集合内
来源：http://qzp.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://beo.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dzv.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://tcv.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://jzg.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vsl.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tpd.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://rka.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vsf.hnqzz.top

[B15] 布尔运算与取反
来源：http://dmb.hcnkem.com

Py:   a and b or not c
来源：http://kwk.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://pnd.jinqigfzy.top

JS:   a && b || !c
来源：http://gxd.jyoumei.cn

TS:   a && b || !c
来源：http://bot.nanxinkj.top

Java: a && b || !c
来源：http://nof.sufxvd.cn

Go:   a && b || !c
来源：http://uct.ydjk.org.cn

Ruby: a && b || !c
来源：http://laf.fktsv.cn

C#:   a && b || !c
来源：http://fbz.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://vqf.cucudq.cn

Py:   if not data: return
来源：http://lhh.hammf.cn

PHP:  if (!$data) { return; }
来源：http://mob.hcnkem.com

JS:   if (!data) return;
来源：http://feq.fengsongda.top

TS:   if (!data) return;
来源：http://brz.xinyue.icu

Java: if (data == null) return;
来源：http://kzy.yuxming.cn

Go:   if data == nil { return }
来源：http://qyu.guowangkeji.top

Ruby: return if data.nil?
来源：http://dca.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://syk.wangdashe.top

================================================================================
来源：http://foy.hfpthk.cn

C. 函数与作用域
来源：http://oct.ydjk.org.cn

================================================================================
来源：http://frm.tianlin.xyz

[C01] 定义函数
来源：http://cip.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://osu.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://scc.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://kxt.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yio.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ygo.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://lrf.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://jac.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://prp.zhijiandao.cn

[C02] 默认参数
来源：http://efy.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://nui.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gov.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vme.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vpf.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ymh.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sfn.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://beq.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://skz.kuanghao11.cn

[C03] 可变参数
来源：http://klj.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://zwy.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rte.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cnu.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dil.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zfx.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://joh.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://gmn.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bow.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://vrg.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uuu.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://coi.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uly.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jry.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://yec.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://wsg.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://vmh.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://lqs.fehbvm.com

[C05] 返回多个值
来源：http://wdd.gogol.net.cn

Py:   return a, b
来源：http://hlu.jyoumei.cn

PHP:  return [$a, $b];
来源：http://dxn.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zmg.ppjwa.cn

TS:   return { a, b };
来源：http://hzw.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://htd.ydjk.org.cn

Go:   return a, b
来源：http://pnf.jinqigufen.top

Ruby: return a, b
来源：http://wpb.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://ypq.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://zuf.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://kka.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gpv.daria6918.cn

JS:   const square = x => x * x;
来源：http://vmv.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://khr.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wmz.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://cfr.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://qeo.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://ikg.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://hde.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://arj.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://eqz.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lmh.nanxuanxn.top

TS:   arr.map(String)
来源：http://swq.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rzy.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jzy.sweek.top

Ruby: arr.map(&:upcase)
来源：http://gtc.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vmi.gaohongyu789.top

[C08] 闭包
来源：http://phe.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lfg.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://luo.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xqr.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zhs.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ayu.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://egj.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ofk.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sdh.0kj1m.cn

[C09] 递归
来源：http://kbf.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nvo.ydjk.org.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lgf.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zmt.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qxc.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fuu.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zku.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzv.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://edn.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://alo.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://shh.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ehf.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zwb.gogol.net.cn

TS:   同 JS
来源：http://thn.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://elc.havefunace.top

Go:   花括号块级作用域
来源：http://sut.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uuv.ybcxt.top

C#:   块级作用域
来源：http://zqh.quarkkingdee.top

[C11] 模块导入与导出
来源：http://kbn.ivvv.top

Py:   from module import func
来源：http://cwm.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xso.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://iot.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jbq.tarul.cn

Java: import java.util.List;
来源：http://xug.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://liq.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://rhp.hesvh.cn

C#:   using System.Text;
来源：http://ijy.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://fds.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://vmo.kuanghao11.cn


<!-- 参考信息 -->