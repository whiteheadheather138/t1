代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rvz.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://kpo.shuidangran.top

C#:   Console.ReadLine();
来源：http://gix.tian-w.cn

[A21] 保留指定小数位输出
来源：http://pdw.cdnleiting.top

Py:   f"{3.14159:.2f}"
来源：http://zuc.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dwy.shangyingyoupin.top

JS:   (3.14159).toFixed(2)
来源：http://sqn.ydzc1.top

TS:   (3.14159).toFixed(2)
来源：http://txt.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://wwh.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qzs.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://uhx.zhongyouzk.top

C#:   3.14159.ToString("F2")
来源：http://mow.ivvv.top

[A22] 获取字符串长度
来源：http://ouu.xziqi.cn

Py:   len(s)
来源：http://kko.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lpt.fehbvm.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jxz.jianghu66.top

TS:   s.length
来源：http://hxr.jinqigfzy.top

Java: s.length()
来源：http://avg.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://abf.nanxinkj.top

Ruby: s.length
来源：http://ewt.nanxuanxn.top

C#:   s.Length
来源：http://tau.yj202588.top

[A23] 大小写转换
来源：http://ekx.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wcd.cqqwz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://flt.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pqs.yonumen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rso.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://koj.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qot.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ktd.hammf.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tql.birdmap.top

[A24] 去除首尾空白
来源：http://exw.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kqv.tarul.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vif.hfpthk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xmq.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tev.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mdo.hammf.cn

Go:   strings.TrimSpace(s)
来源：http://zic.ywan-chungtsiang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nzc.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hqk.zhongyouzk.top

[A25] 字符串比较
来源：http://oop.shangyingyoupin.top

Py:   s1 == s2; s1 != s2
来源：http://wif.ivvv.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gkq.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oqw.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jai.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kct.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uan.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://zrx.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qvu.hcnkem.com

[A26] 类型转换总览
来源：http://zhi.vehdjk.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ssi.ywan-chungtsiang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://geh.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vqi.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://act.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://moj.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wge.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vvv.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ohi.dianchejie.cn

================================================================================
来源：http://law.guannengcc.top

B. 流程控制
来源：http://ffl.sweek.top

================================================================================
来源：http://zyb.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://udq.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://efl.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hfj.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iqi.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://omq.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nso.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jsw.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eik.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lrd.tian-w.cn

[B02] 多分支 else if / elif
来源：http://ias.fanxiaobao.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://thi.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://plm.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ptm.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jil.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mrp.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mpw.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qre.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://svj.chenzaomai.com

[B03] switch / match / case
来源：http://rra.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ydy.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://izt.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sou.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ily.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yvv.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gvs.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ywo.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fud.zhoulong.xyz

[B04] for 计数循环
来源：http://nyx.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://ufx.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sas.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gks.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dbt.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uax.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hns.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://wyi.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://emy.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://fqr.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://yes.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://chh.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yng.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zik.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hga.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://apv.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://wms.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://boy.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://gea.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://wbn.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wgi.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rnn.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://olw.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wqa.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bux.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jwk.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://udm.pengpengdd.cyou

[B07] while 循环
来源：http://sbb.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://wae.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://wpu.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://one.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://rlr.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://qhk.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vua.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://jtf.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://gvu.316326.xyz

[B08] do-while（至少执行一次）
来源：http://vvl.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://ghy.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://pgf.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://ejh.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://vxg.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://pfs.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zvk.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xla.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://spg.xuanzx.com

[B09] break 与 continue
来源：http://ayg.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vbt.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tlb.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjq.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xwa.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzr.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hgo.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gfr.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpo.hcnkem.com

[B10] 遍历同时拿索引
来源：http://evw.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bnj.yanxiufei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rqe.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ncx.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://adt.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ucp.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ojs.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xnp.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ryr.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://yzo.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://qcg.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://dew.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nkz.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyc.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gom.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vdq.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://pvx.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zyy.yuanzhike.top

[B12] 跳出多层循环
来源：http://kdu.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ulv.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rwi.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xwv.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blo.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lvm.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iuq.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://swv.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yxk.yongpay.top

[B13] 判断是否为数字
来源：http://fbb.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://iwz.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://bcz.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvz.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://crt.zhengqikj.top

Java: x instanceof Number
来源：http://sgb.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jgp.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://its.yfazqb.com

C#:   x is int or double or decimal
来源：http://ynl.fengsongda.top

[B14] 判断值是否在集合内
来源：http://spw.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yfy.jinqigufen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://til.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://ajs.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://bxc.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xmn.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oem.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://nro.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vbt.zycfv.cn

[B15] 布尔运算与取反
来源：http://fom.52xcode.cn

Py:   a and b or not c
来源：http://wmz.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://kit.fktsv.cn

JS:   a && b || !c
来源：http://pps.andypj.xyz

TS:   a && b || !c
来源：http://ufm.bjfxy.top

Java: a && b || !c
来源：http://drf.hammf.cn

Go:   a && b || !c
来源：http://vwf.jqgufenzy.top

Ruby: a && b || !c
来源：http://bba.aizwys.cn

C#:   a && b || !c
来源：http://okh.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zqk.jinyuanbaomall.cn

Py:   if not data: return
来源：http://iyg.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://pvo.cqqwz.cn

JS:   if (!data) return;
来源：http://wtm.yuanzhike.top

TS:   if (!data) return;
来源：http://tmr.zhixingplan.top

Java: if (data == null) return;
来源：http://nsb.andypj.xyz

Go:   if data == nil { return }
来源：http://hxn.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://sjc.316326.xyz

C#:   if (data == null) return;
来源：http://pxn.yfazqb.com

================================================================================
来源：http://nqq.ydjk.org.cn

C. 函数与作用域
来源：http://sja.pengpengdd.cyou

================================================================================
来源：http://oot.snrcjt.cn

[C01] 定义函数
来源：http://ylu.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://slb.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ktl.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://mhz.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tag.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vua.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zie.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://jqx.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cat.cheryme.top

[C02] 默认参数
来源：http://cop.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://eyw.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://isy.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://rcv.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xtv.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vld.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dis.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://mkb.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://jvs.nwbrower.top

[C03] 可变参数
来源：http://rkq.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://ubu.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ofe.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://npd.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gtq.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mem.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oad.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zrn.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bnj.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://ztt.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bem.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xmo.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kok.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zcq.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://znf.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://sna.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://deh.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://xff.zhijiandao.cn

[C05] 返回多个值
来源：http://rkm.hysaishi.cn

Py:   return a, b
来源：http://ebs.daria6918.cn

PHP:  return [$a, $b];
来源：http://ure.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ggj.chenzaomai.com

TS:   return { a, b };
来源：http://jge.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aut.zhongyouzk.top

Go:   return a, b
来源：http://hof.kuanghao11.cn

Ruby: return a, b
来源：http://knc.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://atw.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://yii.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://buo.ctjpmb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pnn.tarul.cn

JS:   const square = x => x * x;
来源：http://vit.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://mgn.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://haa.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://glk.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://pon.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ity.hesvh.cn

[C07] 把函数作为参数传入
来源：http://ncy.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kud.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ywi.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://scm.tianlin.xyz

TS:   arr.map(String)
来源：http://xvm.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jdn.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iur.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://eqr.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ztm.zdqjudy.top

[C08] 闭包
来源：http://qet.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xuq.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gjc.ivvv.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yfb.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jdh.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dae.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xxw.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kwk.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://evs.xuetiantiany.cn

[C09] 递归
来源：http://szy.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vwp.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ebi.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kvd.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://veu.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rpu.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xxa.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ycy.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cgi.bbcook.cn

[C10] 变量作用域
来源：http://stc.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://foa.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gwg.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rlm.hammf.cn

TS:   同 JS
来源：http://tvb.bjfxy.top

Java: 方法内为块级作用域
来源：http://sow.daxiang520.top

Go:   花括号块级作用域
来源：http://fxe.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qdx.zdbjq.cn

C#:   块级作用域
来源：http://pax.birdmap.top

[C11] 模块导入与导出
来源：http://fcj.zhaomingkeji.xyz

Py:   from module import func
来源：http://pin.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://djw.xinyue.icu


<!-- 参考信息 -->