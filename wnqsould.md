代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://nid.cashguo.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lwx.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://iin.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://cfe.chenzaomai.com

[A22] 获取字符串长度
来源：http://ncm.ivvv.top

Py:   len(s)
来源：http://yjg.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qgt.ydzc1.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ezq.yueranfly.top

TS:   s.length
来源：http://tsa.zhongyouzk.top

Java: s.length()
来源：http://gzh.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hll.tian-w.cn

Ruby: s.length
来源：http://rqt.daria6918.cn

C#:   s.Length
来源：http://wmo.zhongyouzk.top

[A23] 大小写转换
来源：http://gyg.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oqt.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oyl.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bpg.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pxh.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tzn.zhixingplan.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ybm.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xek.svipenyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jfy.chenlongwang.top

[A24] 去除首尾空白
来源：http://tlq.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://acw.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://puh.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tnk.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://djf.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iqt.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://ghl.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lbv.yuxming.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://paa.yj202588.top

[A25] 字符串比较
来源：http://kdn.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://njs.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oip.jlsjyb.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nkm.zhijiandao.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xbq.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tvn.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vys.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nbw.hnqzz.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://noh.zycfv.cn

[A26] 类型转换总览
来源：http://bcc.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://atn.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hcj.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yvz.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://xxw.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://crg.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fdn.shanyushiyangtech.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vpi.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dzk.dashuyun.cn

================================================================================
来源：http://dnj.chenjidiqi.icu

B. 流程控制
来源：http://iqq.cheryme.top

================================================================================
来源：http://ezw.yonumen.top

[B01] 条件判断 if / else
来源：http://zam.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jos.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yhk.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nzm.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://egg.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://dhj.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ypm.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqk.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oek.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://ffc.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nqg.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ktr.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwt.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibk.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ngy.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xwh.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nxu.daria6918.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aif.epnwcf.com

[B03] switch / match / case
来源：http://beu.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rxf.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wbo.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ohm.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rnr.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wpf.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bvd.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gzf.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lit.gotoacloud.top

[B04] for 计数循环
来源：http://mor.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://lsn.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bea.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ayd.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rpe.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lqf.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://slp.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://lqf.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yeh.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://zzg.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://gfq.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mmn.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://szp.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://byn.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cbp.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vhw.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://lkr.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hfm.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://lgd.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hur.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sde.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ttg.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mlc.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ist.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://voi.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fux.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://prr.fanxiaobao.xyz

[B07] while 循环
来源：http://hog.tarul.cn

Py:   while i < 10: i += 1
来源：http://icv.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://gza.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://reh.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://bsz.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://nrz.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bnh.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://zsj.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://jbb.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://txq.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://gzi.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ewy.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://jkc.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://osx.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://uzx.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mpn.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://boc.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://uit.ivvv.top

[B09] break 与 continue
来源：http://emn.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qbz.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nyq.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixf.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://loo.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pgi.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jeb.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rne.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkl.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://uhq.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivq.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nhv.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jlr.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cbc.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wuw.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qlk.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ljx.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lcy.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://ltx.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://yih.iojbl.cn

PHP:  range(0, 10, 2);
来源：http://smo.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uhg.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kke.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://llu.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://muu.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://csl.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vlr.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://cdk.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://czl.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://rbl.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cej.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pye.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://arg.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rsf.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nzo.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://amm.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://krd.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://sqd.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://nmm.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nsj.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qjg.yangfankeji.com

Java: x instanceof Number
来源：http://cdp.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://itw.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://lgb.zdqjudy.top

C#:   x is int or double or decimal
来源：http://iat.sysykeji.top

[B14] 判断值是否在集合内
来源：http://wmk.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://znm.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://elo.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://wte.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://tft.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uor.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pes.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://oqb.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tlv.redwolf501.top

[B15] 布尔运算与取反
来源：http://hfh.yj20258888.top

Py:   a and b or not c
来源：http://mlv.nwbrower.top

PHP:  $a && $b || !$c
来源：http://nps.chenjidiqi.icu

JS:   a && b || !c
来源：http://xka.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://wum.jyoumei.cn

Java: a && b || !c
来源：http://oiv.hywenlv.cn

Go:   a && b || !c
来源：http://dkd.ydjk.org.cn

Ruby: a && b || !c
来源：http://hsa.zycfv.cn

C#:   a && b || !c
来源：http://eex.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dti.hywenlv.cn

Py:   if not data: return
来源：http://eul.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://joq.haohaochexian.top

JS:   if (!data) return;
来源：http://kxe.xylfe.cn

TS:   if (!data) return;
来源：http://ono.zhixingplan.top

Java: if (data == null) return;
来源：http://krd.cucudq.cn

Go:   if data == nil { return }
来源：http://pco.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://nxf.xuanzx.com

C#:   if (data == null) return;
来源：http://iza.epnwcf.com

================================================================================
来源：http://zwg.ywan-chungtsiang.top

C. 函数与作用域
来源：http://yis.tarul.cn

================================================================================
来源：http://swr.cdnleiting.top

[C01] 定义函数
来源：http://xhz.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://snf.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://czd.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xka.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvj.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://enr.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://tdx.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://lxg.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ugi.nwbrower.top

[C02] 默认参数
来源：http://fox.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://nol.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ull.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://suo.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wjx.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vhy.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mhj.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://roa.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://qel.wangdashe.top

[C03] 可变参数
来源：http://kap.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://xql.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lkf.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cpg.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cuc.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hoy.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qhz.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://byd.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nlb.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://sfs.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ilu.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xin.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tkt.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://znf.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://yyu.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://urf.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://qpy.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://hhn.jyoumei.cn

[C05] 返回多个值
来源：http://uct.cdnleiting.top

Py:   return a, b
来源：http://kao.tianlin.xyz

PHP:  return [$a, $b];
来源：http://say.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://oea.aibaodan.cn

TS:   return { a, b };
来源：http://tpb.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ewg.chenlongwang.top

Go:   return a, b
来源：http://mmy.zdqjudy.top

Ruby: return a, b
来源：http://dyx.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://qzl.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://bta.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://alu.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://qrm.svipenyu.cn

JS:   const square = x => x * x;
来源：http://vco.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://uua.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zro.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://fhh.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://dwq.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ctw.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://sbo.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pbr.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://uga.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fri.zhoulong.xyz

TS:   arr.map(String)
来源：http://lww.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wvs.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ivp.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://mxm.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bin.xingfuxueyuan.xyz

[C08] 闭包
来源：http://fwg.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oja.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://edw.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zgt.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://znv.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gjz.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fja.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rgk.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kgc.jyoumei.cn

[C09] 递归
来源：http://kxu.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qel.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ful.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kcu.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dhd.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jht.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://csb.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ths.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xyu.xuanzx.com

[C10] 变量作用域
来源：http://qth.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dcn.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xsr.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oxp.uphjek.com

TS:   同 JS
来源：http://eyu.hysaishi.cn

Java: 方法内为块级作用域
来源：http://qay.hnqzz.top

Go:   花括号块级作用域
来源：http://oyp.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ozj.tian-w.cn

C#:   块级作用域
来源：http://jkk.ybcxt.top

[C11] 模块导入与导出
来源：http://apy.birdmap.top

Py:   from module import func
来源：http://pxx.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xfe.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://raj.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sxb.haohaochexian.top

Java: import java.util.List;
来源：http://gce.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://art.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://att.guannengcc.top

C#:   using System.Text;
来源：http://caa.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://tuo.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://chn.zhiwuduotai.top


<!-- 参考信息 -->