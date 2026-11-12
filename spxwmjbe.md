代发 wailian999

TS:   s.length
来源：http://gcp.yanxiufei.cn

Java: s.length()
来源：http://ltp.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dru.jqgfzy.top

Ruby: s.length
来源：http://obe.jianghu66.top

C#:   s.Length
来源：http://rdi.shanyushiyangtech.top

[A23] 大小写转换
来源：http://tua.hysaishi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oqw.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pzd.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uez.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hkp.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nkc.jinghuilouyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pyq.c1oappe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bil.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://swk.tianlin.xyz

[A24] 去除首尾空白
来源：http://nfd.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bch.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vdp.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fmm.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qqz.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://efw.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://mnx.bjfxy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hsx.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rgl.fengsongda.top

[A25] 字符串比较
来源：http://czs.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://yhi.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qbg.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://doh.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bwj.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lgy.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uaq.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aue.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xdl.zdbjq.cn

[A26] 类型转换总览
来源：http://sjv.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lza.9152youxi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://evs.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lbw.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://zoj.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gcd.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iiv.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bjz.xinyue.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://psx.xziqi.cn

================================================================================
来源：http://cml.haohaochexian.top

B. 流程控制
来源：http://myr.guowangkeji.top

================================================================================
来源：http://jjk.xziqi.cn

[B01] 条件判断 if / else
来源：http://zxk.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zle.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://myc.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bls.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cud.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bpt.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rpi.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uye.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qtn.316326.xyz

[B02] 多分支 else if / elif
来源：http://hlt.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dpy.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gck.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybb.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gag.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://usf.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pni.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dnz.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ypt.aizwys.cn

[B03] switch / match / case
来源：http://brk.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gkv.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qjl.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hum.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hqr.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sob.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yxz.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vzd.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gnd.hesvh.cn

[B04] for 计数循环
来源：http://tby.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://zin.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kqt.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kiu.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://atb.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://alc.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yjh.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://bau.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://euy.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://qse.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://zpv.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nxp.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fdb.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ncp.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://mnb.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wxm.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://qrn.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://obd.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://kkt.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kny.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sxc.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zub.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://boa.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jqx.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ouy.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://byt.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zxt.zhoulong.xyz

[B07] while 循环
来源：http://czn.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://fgz.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qrs.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://rbg.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://tnd.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://ahb.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mlt.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://dwo.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://ric.sweek.top

[B08] do-while（至少执行一次）
来源：http://tko.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://blq.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gls.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://lfn.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://rvg.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://biy.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://axw.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://sup.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://lrz.pengpengdd.cyou

[B09] break 与 continue
来源：http://jkp.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iao.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ndb.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rau.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnj.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nuh.dianchejie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ddk.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jet.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xse.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://lqr.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://boc.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gjs.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://geq.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lvd.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nuv.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xll.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jhm.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pev.cheryme.top

[B11] 生成数字序列 / 区间
来源：http://nkc.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://prw.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://qps.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwy.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qyn.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lly.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://did.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://glb.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wqp.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://svl.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zkz.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yqx.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nhp.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cnf.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wlv.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pmi.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgc.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uia.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://rzx.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://lyy.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://mjm.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xaq.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wvp.yj20258888.top

Java: x instanceof Number
来源：http://oml.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://exh.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://pvw.tanke756.top

C#:   x is int or double or decimal
来源：http://sez.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://zkm.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fck.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xsl.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://dtt.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://xne.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qjg.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lhr.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://aep.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xox.yangfankeji.com

[B15] 布尔运算与取反
来源：http://bgk.xuanzx.com

Py:   a and b or not c
来源：http://uei.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://zuu.jinqigufen.top

JS:   a && b || !c
来源：http://ekm.tian-w.cn

TS:   a && b || !c
来源：http://pkl.gogol.net.cn

Java: a && b || !c
来源：http://qpq.hongshengwenyu.top

Go:   a && b || !c
来源：http://umx.yj20258888.top

Ruby: a && b || !c
来源：http://hrp.vqdsnc.cn

C#:   a && b || !c
来源：http://cja.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jve.vqdsnc.cn

Py:   if not data: return
来源：http://iwa.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://azu.ivvv.top

JS:   if (!data) return;
来源：http://bgs.quarkkingdee.top

TS:   if (!data) return;
来源：http://spq.gaohongyu789.top

Java: if (data == null) return;
来源：http://wzm.quarkkingdee.top

Go:   if data == nil { return }
来源：http://avx.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://keu.zhoulong.xyz

C#:   if (data == null) return;
来源：http://rwi.xinyue.icu

================================================================================
来源：http://ieq.daria6918.cn

C. 函数与作用域
来源：http://rgb.hnxiangtu.top

================================================================================
来源：http://ccq.nanxuanxn.top

[C01] 定义函数
来源：http://prg.yj20258.top

Py:   def add(a, b): return a + b
来源：http://wgq.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eot.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://paz.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqu.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bhm.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://zzp.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://xlc.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gsf.iojbl.cn

[C02] 默认参数
来源：http://zft.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://whz.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bmh.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://bof.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xwy.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xva.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bhl.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://rrz.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://lqo.yongpay.top

[C03] 可变参数
来源：http://lfb.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://afx.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wcg.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jvm.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ayu.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://avh.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xse.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wya.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ciw.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://ywi.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ksk.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fcv.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://myo.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yeg.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://sbo.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://kbv.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://plm.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://kho.yonumen.top

[C05] 返回多个值
来源：http://nnn.gotoacloud.top

Py:   return a, b
来源：http://ojg.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://srw.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wph.hywenlv.cn

TS:   return { a, b };
来源：http://mlh.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mlj.redwolf501.top

Go:   return a, b
来源：http://fjs.vehdjk.com

Ruby: return a, b
来源：http://uyd.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://tyw.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://xwr.fehbvm.com

Py:   square = lambda x: x * x
来源：http://qpg.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yyw.daxiang520.top

JS:   const square = x => x * x;
来源：http://rfr.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://zzw.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://svv.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hmo.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://qgy.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://xlo.316326.xyz

[C07] 把函数作为参数传入
来源：http://hsi.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zjz.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vqt.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nle.316326.xyz

TS:   arr.map(String)
来源：http://bhp.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://msz.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qvv.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://wjt.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uvl.yongpay.top

[C08] 闭包
来源：http://aqe.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cso.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xxl.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://npr.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fuj.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vod.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wbn.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qku.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bkk.0kj1m.cn

[C09] 递归
来源：http://lbc.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bfa.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fey.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vag.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hin.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wvj.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://txu.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iie.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lew.zdbjq.cn

[C10] 变量作用域
来源：http://cbr.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mgo.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hrm.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zsf.xingfuxueyuan.xyz

TS:   同 JS
来源：http://nxg.yj202588.top

Java: 方法内为块级作用域
来源：http://fdh.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://qhc.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wvf.zhixingplan.top

C#:   块级作用域
来源：http://cec.fzhhl.top

[C11] 模块导入与导出
来源：http://gzt.shzxlz.cn

Py:   from module import func
来源：http://evk.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cog.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kug.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sqb.xylfe.cn

Java: import java.util.List;
来源：http://aft.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mvj.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://mdy.pengpengdd.cyou

C#:   using System.Text;
来源：http://djm.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://jhe.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://ovp.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://boi.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://lkw.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://rch.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zdf.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://xtu.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://fzt.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lqb.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://nal.jyoumei.cn


<!-- 参考信息 -->