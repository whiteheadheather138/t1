代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://ssa.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rgu.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://fmf.guowangkeji.top

C#:   3.14159.ToString("F2")
来源：http://bnr.tarul.cn

[A22] 获取字符串长度
来源：http://grs.tarul.cn

Py:   len(s)
来源：http://uym.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jyt.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jci.tanke756.top

TS:   s.length
来源：http://rsx.kuanghao11.cn

Java: s.length()
来源：http://yzv.dianchejie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iky.yj20258.top

Ruby: s.length
来源：http://pfi.c1oappe.top

C#:   s.Length
来源：http://pmz.c1oappe.top

[A23] 大小写转换
来源：http://pyh.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jfx.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dhg.vqdsnc.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xmn.yonumen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oof.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wkl.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://atg.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jbt.9152youxi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zeo.cashguo.top

[A24] 去除首尾空白
来源：http://tud.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ojl.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tim.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://orb.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://psj.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nyt.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://suq.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ixe.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wjj.epnwcf.com

[A25] 字符串比较
来源：http://niu.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://fmn.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qzx.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uwm.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qjt.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xuu.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qlm.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vwb.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nxx.shangyingyoupin.top

[A26] 类型转换总览
来源：http://tpu.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oae.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vlk.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ebo.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://mpi.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://web.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://khn.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vjc.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oyc.jyoumei.cn

================================================================================
来源：http://zpx.chenjidiqi.icu

B. 流程控制
来源：http://dih.jiagoushi.top

================================================================================
来源：http://rgp.zdqjudy.top

[B01] 条件判断 if / else
来源：http://tel.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tgi.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ilj.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uee.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://beb.bbcook.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uge.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bfp.wangdashe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ifa.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://seq.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://ije.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wey.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fcn.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://guq.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mgw.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kio.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wdo.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dqp.daria6918.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxy.havefunace.top

[B03] switch / match / case
来源：http://tzb.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lfd.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bfb.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bhx.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zmd.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fgg.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ylk.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bfj.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oxc.hysaishi.cn

[B04] for 计数循环
来源：http://vmo.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://bow.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tor.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ell.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fdw.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nff.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hxi.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://uzp.jinqigfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mcc.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://lyu.316326.xyz

Py:   for item in arr: print(item)
来源：http://yff.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qce.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://aeb.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ifz.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://evk.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rrg.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://vsy.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mqh.birdmap.top

[B06] 遍历字典 / 对象
来源：http://cok.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nrj.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ult.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pyv.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nmi.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jcr.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pfq.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zzo.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://olc.xingfuxueyuan.xyz

[B07] while 循环
来源：http://cvi.hnqzz.top

Py:   while i < 10: i += 1
来源：http://jgr.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://tqx.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://znl.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://ncw.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://zsc.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nyq.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://wox.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://abc.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://mhv.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://fac.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bdv.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://xcn.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://hlg.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://iss.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://omh.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://mmo.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://spw.bjfxy.top

[B09] break 与 continue
来源：http://qzi.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://brm.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zfw.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnt.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgs.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jes.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cfd.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dyt.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhf.sxryk.cn

[B10] 遍历同时拿索引
来源：http://wni.cucudq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gqy.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://run.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bwu.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gtm.hongshengwenyu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://snn.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gme.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://etm.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://asm.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://exb.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://pqy.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://wuc.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://edx.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxu.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ihi.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gdg.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://phu.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lct.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://hrn.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yik.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nkz.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wam.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mbq.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://shc.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pqk.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yas.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dqq.tanke756.top

[B13] 判断是否为数字
来源：http://bgf.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://vfm.gotoacloud.top

PHP:  is_numeric($x)
来源：http://mhr.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xnj.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lgb.redwolf501.top

Java: x instanceof Number
来源：http://bjm.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uak.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://eqd.sufxvd.cn

C#:   x is int or double or decimal
来源：http://eqp.shuidangran.top

[B14] 判断值是否在集合内
来源：http://gnb.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://smf.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tjr.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://nvt.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://fah.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ueo.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hls.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://oom.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://thq.daria6918.cn

[B15] 布尔运算与取反
来源：http://zsq.yuxming.cn

Py:   a and b or not c
来源：http://jwt.ybcxt.top

PHP:  $a && $b || !$c
来源：http://zeh.aibaodan.cn

JS:   a && b || !c
来源：http://zyj.yanxiufei.cn

TS:   a && b || !c
来源：http://fcg.zhiwuduotai.top

Java: a && b || !c
来源：http://fym.hnqzz.top

Go:   a && b || !c
来源：http://vus.jqgfzy.top

Ruby: a && b || !c
来源：http://vkn.ivvv.top

C#:   a && b || !c
来源：http://ffx.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://izs.9152youxi.cn

Py:   if not data: return
来源：http://rab.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://qar.zhixingplan.top

JS:   if (!data) return;
来源：http://qin.zhongyouzk.top

TS:   if (!data) return;
来源：http://oml.tian-w.cn

Java: if (data == null) return;
来源：http://kby.vqdsnc.cn

Go:   if data == nil { return }
来源：http://xcl.yanxiufei.cn

Ruby: return if data.nil?
来源：http://twx.jinqigfzy.top

C#:   if (data == null) return;
来源：http://sop.yangfankeji.com

================================================================================
来源：http://zgj.xylfe.cn

C. 函数与作用域
来源：http://ubb.shzxlz.cn

================================================================================
来源：http://wmm.wangshuangyany.cn

[C01] 定义函数
来源：http://ksj.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://llb.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iet.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://ilj.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ndy.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://img.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://vzv.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://vrh.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ahy.cheryme.top

[C02] 默认参数
来源：http://mgy.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://dmq.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gbp.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://aib.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://fdu.gogol.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dwa.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gwu.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://yol.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://aur.sxryk.cn

[C03] 可变参数
来源：http://rku.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://pfc.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ogm.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yjv.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uas.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://som.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ong.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vkq.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fif.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://mvk.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dtt.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uio.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oxm.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://itl.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://cbz.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://wub.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://chh.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://ulw.bjfxy.top

[C05] 返回多个值
来源：http://nls.shanyushiyangtech.top

Py:   return a, b
来源：http://daz.jyoumei.cn

PHP:  return [$a, $b];
来源：http://xri.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nzm.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://ssf.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jvk.gotoacloud.top

Go:   return a, b
来源：http://ika.jiagoushi.top

Ruby: return a, b
来源：http://rwj.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://hpy.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://opy.ydzc1.top

Py:   square = lambda x: x * x
来源：http://rdg.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bcd.snrcjt.cn

JS:   const square = x => x * x;
来源：http://xsi.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://yhe.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xhx.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nhz.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://xxo.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://fep.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://dgt.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://maq.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://tsz.yvedp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gys.sjlbkw.cn

TS:   arr.map(String)
来源：http://akt.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iet.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sml.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://liw.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uaa.c1oappe.top

[C08] 闭包
来源：http://oxn.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nzq.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://esp.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hmz.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pil.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nat.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://anq.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jln.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uma.jiagoushi.top

[C09] 递归
来源：http://dec.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cfx.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sna.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pqo.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lzy.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nbr.cheryme.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kpd.hongshengwenyu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kqx.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ycn.zhoulong.xyz

[C10] 变量作用域
来源：http://ltc.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ssr.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pfw.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gmb.bbcook.cn

TS:   同 JS
来源：http://ujl.sufxvd.cn

Java: 方法内为块级作用域
来源：http://bnl.bjfxy.top

Go:   花括号块级作用域
来源：http://dpo.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fbs.jlsjyb.cn

C#:   块级作用域
来源：http://ofo.chenlongwang.top

[C11] 模块导入与导出
来源：http://bhj.gotoacloud.top

Py:   from module import func
来源：http://gio.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pep.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://hvs.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xvn.zycfv.cn

Java: import java.util.List;
来源：http://abm.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kyl.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://oxq.bbcook.cn

C#:   using System.Text;
来源：http://lqi.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://dzn.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://nhn.ivvv.top


<!-- 参考信息 -->