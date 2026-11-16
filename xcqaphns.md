代发 wailian999

TS:   s.length
来源：http://xmk.feifeiyinyue.top

Java: s.length()
来源：http://gii.nanxinkj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://njm.xinyue.icu

Ruby: s.length
来源：http://bgt.nwbrower.top

C#:   s.Length
来源：http://dux.sufxvd.cn

[A23] 大小写转换
来源：http://pft.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nre.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xjz.tianlin.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kuu.wangdashe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hqn.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zbi.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ign.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lpk.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lfb.iojbl.cn

[A24] 去除首尾空白
来源：http://gqo.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://naw.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rtd.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pyw.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nsx.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lgm.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://owl.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://smz.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://njq.gotoacloud.top

[A25] 字符串比较
来源：http://wuk.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://jrs.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eey.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vug.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oxk.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qoa.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rwb.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://eby.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vim.ybcxt.top

[A26] 类型转换总览
来源：http://vpb.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uua.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ehw.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hpj.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://cyv.nwbrower.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rsp.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aab.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://byz.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tfc.yj20258888.top

================================================================================
来源：http://lcz.pycfn.com

B. 流程控制
来源：http://qyl.sxryk.cn

================================================================================
来源：http://fin.gzhubu.top

[B01] 条件判断 if / else
来源：http://owa.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gbw.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://neh.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cwy.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zgv.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://dwl.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zzb.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gkp.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://chx.epnwcf.com

[B02] 多分支 else if / elif
来源：http://aat.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yvj.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ocl.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ouj.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehq.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwd.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dhl.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zin.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzb.shuidangran.top

[B03] switch / match / case
来源：http://kkh.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xlv.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fzp.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qsj.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://enw.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nbm.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ulu.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://frx.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lkf.sxryk.cn

[B04] for 计数循环
来源：http://enn.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://gbx.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ele.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ibf.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pzf.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tbq.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uhi.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://voy.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jeb.316326.xyz

[B05] 遍历数组 / 列表
来源：http://yxc.redwolf501.top

Py:   for item in arr: print(item)
来源：http://nik.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vfb.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jgd.0kj1m.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wlk.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ixd.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://usm.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://gma.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qns.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://wna.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ddd.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://isv.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://atk.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://irn.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yaw.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wmg.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://avo.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qqy.quarkkingdee.top

[B07] while 循环
来源：http://qne.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://hen.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ctg.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://zbd.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://pmp.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://wju.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://avk.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://shf.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://erg.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://ljc.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://tvr.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qwx.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://sjc.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://men.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://jsi.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mbc.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://qpp.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://gix.ydjk.org.cn

[B09] break 与 continue
来源：http://ahx.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gba.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fnp.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icq.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://awh.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlf.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zwo.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ltw.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jif.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://aey.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gat.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qmc.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sly.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wbb.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gpr.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tzn.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oey.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cwe.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://qwx.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://ldc.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://waz.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mxm.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://epp.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xeo.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gjb.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://zng.sxryk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jsy.ppjwa.cn

[B12] 跳出多层循环
来源：http://mcj.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wrq.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://rtk.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xmf.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qxb.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ygw.jinyuanbaomall.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://szy.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://awc.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yhh.0kj1m.cn

[B13] 判断是否为数字
来源：http://mik.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://zzl.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://jrv.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mjk.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vkw.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://ame.sweek.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qeg.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://hew.zhixingplan.top

C#:   x is int or double or decimal
来源：http://ogc.andypj.xyz

[B14] 判断值是否在集合内
来源：http://hrs.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sko.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bum.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://sej.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://clk.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ijl.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://olr.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vpo.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lmf.daria6918.cn

[B15] 布尔运算与取反
来源：http://tax.yj20258888.top

Py:   a and b or not c
来源：http://qup.andypj.xyz

PHP:  $a && $b || !$c
来源：http://rkd.birdmap.top

JS:   a && b || !c
来源：http://gbe.shanyushiyangtech.top

TS:   a && b || !c
来源：http://pkn.zhaomingkeji.xyz

Java: a && b || !c
来源：http://cpc.ydzc1.top

Go:   a && b || !c
来源：http://hfy.fengsongda.top

Ruby: a && b || !c
来源：http://zdd.cucudq.cn

C#:   a && b || !c
来源：http://cro.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://pbd.andypj.xyz

Py:   if not data: return
来源：http://yyb.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://sdt.pengpengdd.cyou

JS:   if (!data) return;
来源：http://slp.hcnkem.com

TS:   if (!data) return;
来源：http://dua.hongshengwenyu.top

Java: if (data == null) return;
来源：http://fdq.316326.xyz

Go:   if data == nil { return }
来源：http://tbj.sweek.top

Ruby: return if data.nil?
来源：http://jko.yuxming.cn

C#:   if (data == null) return;
来源：http://dyq.shanyushiyangkeji.top

================================================================================
来源：http://xdh.xingfuxueyuan.xyz

C. 函数与作用域
来源：http://ruj.yuanzhike.top

================================================================================
来源：http://ved.chenjidiqi.icu

[C01] 定义函数
来源：http://awc.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://jjc.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jto.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://nxo.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bjl.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zrh.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://opo.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://ymo.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kxg.havefunace.top

[C02] 默认参数
来源：http://pqm.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://kjb.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xvl.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://qop.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lew.gogol.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ewo.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fcz.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://iss.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://iql.yvedp.cn

[C03] 可变参数
来源：http://dbm.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://lrr.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mra.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://law.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bpa.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://enr.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ldf.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oto.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gzs.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://lfg.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iws.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ijj.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kwi.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jsl.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://udv.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://ghr.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://gup.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://ugz.hnxiangtu.top

[C05] 返回多个值
来源：http://lop.aibaodan.cn

Py:   return a, b
来源：http://xer.fengsongda.top

PHP:  return [$a, $b];
来源：http://jgi.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ixq.cashguo.top

TS:   return { a, b };
来源：http://vaa.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rdj.xziqi.cn

Go:   return a, b
来源：http://tsk.zhijiandao.cn

Ruby: return a, b
来源：http://pdj.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://jct.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://owt.xinyue.icu

Py:   square = lambda x: x * x
来源：http://geb.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bxk.epnwcf.com

JS:   const square = x => x * x;
来源：http://rpu.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://ffy.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ktl.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://obp.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://cpp.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://vdf.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://hno.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ymv.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://czu.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://avq.havefunace.top

TS:   arr.map(String)
来源：http://pbh.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jhs.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iag.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://dsn.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://taf.xinyue.icu

[C08] 闭包
来源：http://nwy.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jst.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yoa.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ltz.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ora.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nca.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qox.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://phm.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://stc.ehwqpu.com

[C09] 递归
来源：http://vmb.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blw.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uuc.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hox.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fkl.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hce.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kvb.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://piu.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jpf.bbcook.cn

[C10] 变量作用域
来源：http://qpu.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kck.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xcg.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aqo.smart0.xyz

TS:   同 JS
来源：http://mie.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://qfe.bbcook.cn

Go:   花括号块级作用域
来源：http://yjm.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://khg.zhaomingkeji.xyz

C#:   块级作用域
来源：http://isf.tarul.cn

[C11] 模块导入与导出
来源：http://yos.fengsongda.top

Py:   from module import func
来源：http://yhe.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yxj.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://feb.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gaz.pycfn.com

Java: import java.util.List;
来源：http://upx.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lzy.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://bse.jinqigufen.top

C#:   using System.Text;
来源：http://tzn.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://enx.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://nqd.shuidangran.top

PHP:  (function () { echo "run"; })();
来源：http://fiu.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://eyg.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://swz.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jee.meibo888.top

Go:   func() { fmt.Println("run") }()
来源：http://efr.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://fom.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mzc.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://rul.guowangkeji.top


<!-- 参考信息 -->