代发 wailian999

[A22] 获取字符串长度
来源：http://asf.aibaodan.cn

Py:   len(s)
来源：http://eri.mhx1999.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ubx.ywan-chungtsiang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fmj.cashguo.top

TS:   s.length
来源：http://ppq.sjlbkw.cn

Java: s.length()
来源：http://fpz.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mpt.316326.xyz

Ruby: s.length
来源：http://fmj.jqgfzy.top

C#:   s.Length
来源：http://hms.dashuyun.cn

[A23] 大小写转换
来源：http://lhf.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://jcc.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qtx.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://loq.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kzs.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lps.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ldi.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rdj.yj202588.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ikc.wangdashe.top

[A24] 去除首尾空白
来源：http://cgc.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://doz.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pid.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xwk.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gii.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dvw.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://bee.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://svr.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gvv.nwbrower.top

[A25] 字符串比较
来源：http://mhh.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://zhp.snrcjt.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pan.zycfv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sne.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xag.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bpe.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rgr.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fos.yonumen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xon.zdqjudy.top

[A26] 类型转换总览
来源：http://iwp.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hek.ppjwa.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lix.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ohl.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://vgm.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jic.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hru.iojbl.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ybx.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pgk.jinghuilouyu.cn

================================================================================
来源：http://cxa.tian-w.cn

B. 流程控制
来源：http://nbq.fengsongda.top

================================================================================
来源：http://pmw.meibo888.top

[B01] 条件判断 if / else
来源：http://pzc.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qcr.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eez.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dut.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://osz.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xcq.yfazqb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ksq.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://avl.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bbm.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://oxs.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ewi.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lie.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwa.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ulm.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvv.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yba.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lap.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://her.bbcook.cn

[B03] switch / match / case
来源：http://xtc.yuanzhike.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rxy.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qrn.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ncj.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yjv.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xud.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cyo.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ois.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xvu.c1oappe.top

[B04] for 计数循环
来源：http://yxr.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://pdm.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://khm.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://whr.c1oappe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hep.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://exg.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zbb.zhengqikj.top

Ruby: 10.times { |i| puts i }
来源：http://zxx.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ifg.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://vge.tian-w.cn

Py:   for item in arr: print(item)
来源：http://aop.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wst.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://olc.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hbw.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cdv.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bdy.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://iap.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nfi.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://qxr.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rlh.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wdh.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cla.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qir.yvedp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://znq.gotoacloud.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dbz.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tzj.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tev.cdnleiting.top

[B07] while 循环
来源：http://zxt.fengsongda.top

Py:   while i < 10: i += 1
来源：http://ixn.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://muq.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://khe.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://nmq.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://ebk.snrcjt.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pdw.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://utq.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://jcu.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://yku.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://sow.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zfh.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://bxz.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://wgd.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://jns.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://nmc.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://yyd.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://kat.sufxvd.cn

[B09] break 与 continue
来源：http://zxo.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hyo.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ikd.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qth.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnz.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eqr.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jwl.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cys.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdl.fehbvm.com

[B10] 遍历同时拿索引
来源：http://ryn.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jql.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://whq.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kvh.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://owo.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kpt.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://imu.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pdz.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dxf.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://lmb.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://top.havefunace.top

PHP:  range(0, 10, 2);
来源：http://jyx.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ulp.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nnr.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tso.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ihx.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://vxn.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://agi.mhx1999.top

[B12] 跳出多层循环
来源：http://mbg.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://dcp.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ftw.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfi.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fsf.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gyr.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hrz.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sji.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lie.ppjwa.cn

[B13] 判断是否为数字
来源：http://ahz.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://bqj.havefunace.top

PHP:  is_numeric($x)
来源：http://ugi.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dlx.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://daz.wangdashe.top

Java: x instanceof Number
来源：http://rtr.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ryc.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://ozj.yangfankeji.com

C#:   x is int or double or decimal
来源：http://reg.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://ojy.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mwd.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mit.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://wco.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://pmk.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kls.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vac.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://hda.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lux.hcnkem.com

[B15] 布尔运算与取反
来源：http://jbs.jinqigufen.top

Py:   a and b or not c
来源：http://ycb.yfazqb.com

PHP:  $a && $b || !$c
来源：http://bbx.yj202588.top

JS:   a && b || !c
来源：http://cmv.zhixingplan.top

TS:   a && b || !c
来源：http://lsd.bbcook.cn

Java: a && b || !c
来源：http://trg.yvedp.cn

Go:   a && b || !c
来源：http://hht.tarul.cn

Ruby: a && b || !c
来源：http://qiw.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://wxb.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://tni.vqdsnc.cn

Py:   if not data: return
来源：http://rlq.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://giy.vqdsnc.cn

JS:   if (!data) return;
来源：http://sog.gaohongyu789.top

TS:   if (!data) return;
来源：http://dfb.xuanzx.com

Java: if (data == null) return;
来源：http://mur.gotoacloud.top

Go:   if data == nil { return }
来源：http://wrx.snrcjt.cn

Ruby: return if data.nil?
来源：http://xil.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://dvb.ctjpmb.com

================================================================================
来源：http://hug.havefunace.top

C. 函数与作用域
来源：http://mrq.yvedp.cn

================================================================================
来源：http://jws.cheryme.top

[C01] 定义函数
来源：http://rza.tarul.cn

Py:   def add(a, b): return a + b
来源：http://mhp.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tgn.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://bpw.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://goh.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xxx.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cjx.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://adk.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://egt.jianghu66.top

[C02] 默认参数
来源：http://atu.pycfn.com

Py:   def greet(name="World"): return name
来源：http://wyp.gzhubu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vhy.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://sxr.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gnq.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://brk.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://weg.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://ifk.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://opc.fengsongda.top

[C03] 可变参数
来源：http://fiu.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://hti.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wag.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vtj.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rut.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xcj.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qov.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jwu.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ovl.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://lfy.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fsx.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ueq.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uza.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mvw.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://zfy.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://wob.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://aiu.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://dss.wangdashe.top

[C05] 返回多个值
来源：http://umk.cashguo.top

Py:   return a, b
来源：http://rjq.ppjwa.cn

PHP:  return [$a, $b];
来源：http://ppc.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mmq.jianghu66.top

TS:   return { a, b };
来源：http://ggv.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kgv.ydjk.org.cn

Go:   return a, b
来源：http://mip.chenzaomai.com

Ruby: return a, b
来源：http://wfo.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://pee.tarul.cn

[C06] 匿名函数 / lambda
来源：http://qnc.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://wjt.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xom.hywenlv.cn

JS:   const square = x => x * x;
来源：http://thw.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://yvg.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wbx.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://sst.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://sev.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fyy.yueranfly.top

[C07] 把函数作为参数传入
来源：http://dvv.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://csy.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yts.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kqj.shuidangran.top

TS:   arr.map(String)
来源：http://mhx.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yrl.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vzp.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://xdv.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ogv.cqqwz.cn

[C08] 闭包
来源：http://ntw.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oty.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hio.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dve.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dtg.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hrh.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qle.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gef.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cwq.jqgufenzy.top

[C09] 递归
来源：http://okz.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ikd.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oze.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnh.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qgf.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lkj.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rjq.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dfu.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jej.jiagoushi.top

[C10] 变量作用域
来源：http://dkh.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cvf.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lqt.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nzf.hywenlv.cn

TS:   同 JS
来源：http://bmw.haohaochexian.top

Java: 方法内为块级作用域
来源：http://kpd.cdnleiting.top

Go:   花括号块级作用域
来源：http://zeu.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tnk.ctjpmb.com

C#:   块级作用域
来源：http://ito.nwbrower.top

[C11] 模块导入与导出
来源：http://xlc.nanxinkj.top

Py:   from module import func
来源：http://srt.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tlc.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://est.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lpe.feifeiyinyue.top

Java: import java.util.List;
来源：http://hbv.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hmb.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://hpb.sysykeji.top

C#:   using System.Text;
来源：http://rmy.svipenyu.cn

[C12] 立即执行函数 IIFE
来源：http://iua.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://jrw.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://dbe.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://kzv.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://efo.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ild.snrcjt.cn


<!-- 参考信息 -->