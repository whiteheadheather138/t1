代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://zsb.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bkm.hesvh.cn

JS:   (3.14159).toFixed(2)
来源：http://kji.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://nye.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://ejx.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ptb.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://jpr.hywenlv.cn

C#:   3.14159.ToString("F2")
来源：http://jyr.wangshuangyany.cn

[A22] 获取字符串长度
来源：http://nbj.sysykeji.top

Py:   len(s)
来源：http://ytp.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bfe.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lys.wangdashe.top

TS:   s.length
来源：http://pgr.shuidangran.top

Java: s.length()
来源：http://jdi.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gzg.gzhubu.top

Ruby: s.length
来源：http://pzm.sxryk.cn

C#:   s.Length
来源：http://slk.shangyingyoupin.top

[A23] 大小写转换
来源：http://idr.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ypg.hywenlv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://txt.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zoe.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hca.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dck.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zci.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dpf.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lmq.hcnkem.com

[A24] 去除首尾空白
来源：http://swa.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yqv.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jnv.nwbrower.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pcw.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://phr.hnxiangtu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xra.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://pvk.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yus.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://znb.xylfe.cn

[A25] 字符串比较
来源：http://yoc.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://xej.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vzk.sufxvd.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jny.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mjw.ppjwa.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ids.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vjx.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://obn.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xhl.feifeiyinyue.top

[A26] 类型转换总览
来源：http://cef.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hfh.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qsu.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dnk.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://jxg.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vup.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kay.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://afk.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yvd.shzxlz.cn

================================================================================
来源：http://qba.haohaochexian.top

B. 流程控制
来源：http://vlt.mhx1999.top

================================================================================
来源：http://jrf.yuanzhike.top

[B01] 条件判断 if / else
来源：http://qew.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://dal.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uxg.tianlin.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bgj.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sfu.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ljm.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://viz.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yqn.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mxy.bjfxy.top

[B02] 多分支 else if / elif
来源：http://tju.xingfuxueyuan.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hrc.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://igk.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbv.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkr.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://duv.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tmu.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bdd.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rfn.hywenlv.cn

[B03] switch / match / case
来源：http://xut.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yha.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ujx.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cjh.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://apo.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vdn.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://coa.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gwm.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aeo.ywan-chungtsiang.top

[B04] for 计数循环
来源：http://xyl.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://dsk.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yhg.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://avq.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fmg.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zxx.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jlt.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://rcl.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dbt.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://jsu.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://nur.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yov.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vok.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://elo.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pzi.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bhm.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://nrb.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sxd.cheryme.top

[B06] 遍历字典 / 对象
来源：http://rme.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vkc.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zjd.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ytu.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sts.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jwk.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ory.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uty.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cyn.yuxming.cn

[B07] while 循环
来源：http://opy.meibo888.top

Py:   while i < 10: i += 1
来源：http://zbr.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dxs.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://mrq.quarkkingdee.top

TS:   while (i < 10) { i++; }
来源：http://kbp.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://vhd.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ciu.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://ehm.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://tjg.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://fzw.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://aof.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gml.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://ies.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://rtk.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://mza.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://szu.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://gwe.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://dbw.0kj1m.cn

[B09] break 与 continue
来源：http://jav.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cit.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mzv.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cmh.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdv.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wwq.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sgt.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tpk.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fin.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://kok.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kgt.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ucv.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qcw.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hga.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ukp.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pag.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nea.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oio.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://ngz.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://jwh.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://dhr.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://agd.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uah.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yuv.xuanzx.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://phr.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://bln.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tss.vqdsnc.cn

[B12] 跳出多层循环
来源：http://utf.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bin.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bxj.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wcd.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qiq.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://que.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://huq.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fzm.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yxz.cqqwz.cn

[B13] 判断是否为数字
来源：http://cmg.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://tkz.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://jxe.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jcm.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ytc.jlsjyb.cn

Java: x instanceof Number
来源：http://ihf.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zoy.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://rsj.yueranfly.top

C#:   x is int or double or decimal
来源：http://loi.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://gav.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zgo.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qzp.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://nwp.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://zrp.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://tzc.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uqr.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://yzl.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yth.smart0.xyz

[B15] 布尔运算与取反
来源：http://raj.yj20258.top

Py:   a and b or not c
来源：http://hju.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://uce.dashuyun.cn

JS:   a && b || !c
来源：http://dno.fktsv.cn

TS:   a && b || !c
来源：http://nkw.zhixingplan.top

Java: a && b || !c
来源：http://ydy.iojbl.cn

Go:   a && b || !c
来源：http://hoh.jinqigfzy.top

Ruby: a && b || !c
来源：http://wsb.316326.xyz

C#:   a && b || !c
来源：http://elk.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://ict.xinyue.icu

Py:   if not data: return
来源：http://ebs.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://usn.aibaodan.cn

JS:   if (!data) return;
来源：http://lje.guowangkeji.top

TS:   if (!data) return;
来源：http://jas.tianlin.xyz

Java: if (data == null) return;
来源：http://lyz.fktsv.cn

Go:   if data == nil { return }
来源：http://gkn.iojbl.cn

Ruby: return if data.nil?
来源：http://vfz.nanxuanxn.top

C#:   if (data == null) return;
来源：http://ogp.shzxlz.cn

================================================================================
来源：http://bwi.xziqi.cn

C. 函数与作用域
来源：http://irr.jiagoushi.top

================================================================================
来源：http://liq.jyoumei.cn

[C01] 定义函数
来源：http://dxl.yj202588.top

Py:   def add(a, b): return a + b
来源：http://mgw.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zmy.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://wad.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jwj.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cgp.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://btq.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://awo.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qfx.andypj.xyz

[C02] 默认参数
来源：http://ebs.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://lxm.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://jnr.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://cyh.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eqf.gogol.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eqk.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wfs.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://aaj.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://lzn.gotoacloud.top

[C03] 可变参数
来源：http://cpw.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://smb.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bqn.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kcu.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rub.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kjk.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://avn.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gum.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nad.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://bxe.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ytp.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kfz.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yce.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yhq.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://slb.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://gki.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://xut.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://qbq.hfpthk.cn

[C05] 返回多个值
来源：http://ave.nwbrower.top

Py:   return a, b
来源：http://nqo.fengsongda.top

PHP:  return [$a, $b];
来源：http://jdl.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tlg.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://xal.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sed.cheryme.top

Go:   return a, b
来源：http://lux.meibo888.top

Ruby: return a, b
来源：http://jcb.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://mmb.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://one.shuidangran.top

Py:   square = lambda x: x * x
来源：http://xvu.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lie.pycfn.com

JS:   const square = x => x * x;
来源：http://alc.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://eeu.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mou.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://npn.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://kno.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cbf.mhx1999.top

[C07] 把函数作为参数传入
来源：http://vxa.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vbr.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://cnl.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wbl.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://wjy.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kte.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://knq.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://qty.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://coo.havefunace.top

[C08] 闭包
来源：http://ozj.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://omd.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mzt.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jec.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zlj.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mpd.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mga.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wrr.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hrl.sweek.top

[C09] 递归
来源：http://rwu.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rtl.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dgq.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uzz.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zcd.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vjh.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qef.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fcp.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://phl.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://exz.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://goe.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gmx.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kns.tanke756.top

TS:   同 JS
来源：http://fig.tanke756.top

Java: 方法内为块级作用域
来源：http://whz.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://kgs.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kbe.ydjk.org.cn

C#:   块级作用域
来源：http://ewm.vehdjk.com

[C11] 模块导入与导出
来源：http://nav.chenlongwang.top

Py:   from module import func
来源：http://xcp.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://iuw.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zjm.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zup.jyoumei.cn

Java: import java.util.List;
来源：http://qee.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iby.hesvh.cn


<!-- 参考信息 -->