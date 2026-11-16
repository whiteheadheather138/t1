代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://xzy.aizwys.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kfj.yongpay.top

Ruby: format("%.2f", 3.14159)
来源：http://oaa.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://pae.xuetiantiany.cn

[A22] 获取字符串长度
来源：http://byg.cashguo.top

Py:   len(s)
来源：http://cfi.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vwg.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://asw.shangyingyoupin.top

TS:   s.length
来源：http://mpn.nanxinkj.top

Java: s.length()
来源：http://iyl.dianchejie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mpo.bjfxy.top

Ruby: s.length
来源：http://gri.pycfn.com

C#:   s.Length
来源：http://hbn.jinqigufen.top

[A23] 大小写转换
来源：http://iox.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zqz.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yya.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ozo.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://acm.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kos.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://viy.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qfl.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nco.epnwcf.com

[A24] 去除首尾空白
来源：http://zzj.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fpe.shuidangran.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rld.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dqb.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wck.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ryl.hywenlv.cn

Go:   strings.TrimSpace(s)
来源：http://tkj.yuanzhike.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zef.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rpc.fengsongda.top

[A25] 字符串比较
来源：http://bbh.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://xwa.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xoq.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ymk.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rsg.vqdsnc.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://otj.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rjm.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://dfl.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ebn.sufxvd.cn

[A26] 类型转换总览
来源：http://vlh.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qgd.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pnt.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zrh.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://amu.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mzp.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vik.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://taw.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zfc.gogol.net.cn

================================================================================
来源：http://ocb.sysykeji.top

B. 流程控制
来源：http://wma.wangshuangyany.cn

================================================================================
来源：http://zyp.daxiang520.top

[B01] 条件判断 if / else
来源：http://lnq.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gmg.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ieg.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blm.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nde.yvedp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ivf.yfazqb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vrn.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rhc.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://flx.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://byc.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qvb.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://spp.fengsongda.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfo.chenlongwang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbb.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wkv.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mdw.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ysu.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sww.xylfe.cn

[B03] switch / match / case
来源：http://gkq.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cne.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qga.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mbe.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ckv.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tep.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://izk.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gyc.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sxd.zhoulong.xyz

[B04] for 计数循环
来源：http://saj.birdmap.top

Py:   for i in range(10): print(i)
来源：http://rwo.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ifp.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ztc.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wzu.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gmv.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yjd.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://yxs.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wtq.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://sxm.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://zjb.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cbb.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zpt.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sxl.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lct.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hvo.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://zcj.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://som.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://siy.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kwb.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nbj.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blp.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cuz.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vxc.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gmk.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zac.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gzu.gaohongyu789.top

[B07] while 循环
来源：http://mqx.fktsv.cn

Py:   while i < 10: i += 1
来源：http://ugi.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://mws.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://goi.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://jss.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://qav.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mha.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://ukk.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://xik.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://wex.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://sbc.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://gei.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://bhc.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://qrs.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://eqn.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bqu.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://wgh.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://ckf.hnqzz.top

[B09] break 与 continue
来源：http://ror.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hfd.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jep.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sfx.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idp.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkd.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qzp.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kfk.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gjt.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://hya.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ifq.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ozd.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qfn.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yrv.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ydj.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fof.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://izf.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://npy.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://yog.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://bow.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://zbb.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wdd.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lio.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nta.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lpj.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://wpd.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rgr.fktsv.cn

[B12] 跳出多层循环
来源：http://ehv.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://onk.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ipc.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://puf.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jmr.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oie.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vur.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rih.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eqy.gzhubu.top

[B13] 判断是否为数字
来源：http://emx.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://uyf.cheryme.top

PHP:  is_numeric($x)
来源：http://snt.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pnu.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qps.pengpengdd.cyou

Java: x instanceof Number
来源：http://zra.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sdi.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://uix.hnqzz.top

C#:   x is int or double or decimal
来源：http://adl.sxryk.cn

[B14] 判断值是否在集合内
来源：http://iyr.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hfl.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nxz.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://mob.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://lms.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://zbw.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fhl.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xge.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://umx.jianghu66.top

[B15] 布尔运算与取反
来源：http://sbr.jqgufenzy.top

Py:   a and b or not c
来源：http://ynh.cucudq.cn

PHP:  $a && $b || !$c
来源：http://qtc.redwolf501.top

JS:   a && b || !c
来源：http://mjq.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://rvj.guannengcc.top

Java: a && b || !c
来源：http://eqp.tanke756.top

Go:   a && b || !c
来源：http://kzx.yangfankeji.com

Ruby: a && b || !c
来源：http://xnj.hfpthk.cn

C#:   a && b || !c
来源：http://ftp.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://rks.hcnkem.com

Py:   if not data: return
来源：http://muu.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://koo.xuetiantiany.cn

JS:   if (!data) return;
来源：http://hix.dashuyun.cn

TS:   if (!data) return;
来源：http://apt.ctjpmb.com

Java: if (data == null) return;
来源：http://pbl.hywenlv.cn

Go:   if data == nil { return }
来源：http://ery.gaohongyu789.top

Ruby: return if data.nil?
来源：http://pzy.aizwys.cn

C#:   if (data == null) return;
来源：http://spe.chenjidiqi.icu

================================================================================
来源：http://kxg.yuxming.cn

C. 函数与作用域
来源：http://hyb.zdqjudy.top

================================================================================
来源：http://fvz.epnwcf.com

[C01] 定义函数
来源：http://bvv.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://krg.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://otq.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://xwt.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zri.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tel.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://aao.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://cbt.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uov.yvedp.cn

[C02] 默认参数
来源：http://cho.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://wfu.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hdw.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://gpk.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nul.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://evu.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vzt.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://xzz.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://vtl.yuxming.cn

[C03] 可变参数
来源：http://mhe.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://zae.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rzs.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zry.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrr.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://azj.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uio.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://rtz.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jxj.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://nss.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ndg.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jxn.xuetiantiany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wiv.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gnc.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://whi.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://jbj.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://nnc.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://qrq.epnwcf.com

[C05] 返回多个值
来源：http://emr.yj20258.top

Py:   return a, b
来源：http://gch.iojbl.cn

PHP:  return [$a, $b];
来源：http://nkv.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xsw.daxiang520.top

TS:   return { a, b };
来源：http://cad.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yir.pengpengdd.cyou

Go:   return a, b
来源：http://hgm.uphjek.com

Ruby: return a, b
来源：http://oju.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://mln.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://xfd.yj202588.top

Py:   square = lambda x: x * x
来源：http://vir.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zyp.c1oappe.top

JS:   const square = x => x * x;
来源：http://lon.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://cml.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://naq.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://roh.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://gnc.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://cya.ybcxt.top

[C07] 把函数作为参数传入
来源：http://vzb.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rlg.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ihe.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pck.316326.xyz

TS:   arr.map(String)
来源：http://cey.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hai.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uik.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://ypy.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iez.jiagoushi.top

[C08] 闭包
来源：http://nwy.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yby.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ahf.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gwx.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ybl.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tec.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lry.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ufp.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ead.jyoumei.cn

[C09] 递归
来源：http://mov.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lua.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rcw.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dca.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jfu.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sjt.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xwr.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hrf.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ghr.gotoacloud.top

[C10] 变量作用域
来源：http://weq.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ctl.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qmf.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://obb.gotoacloud.top

TS:   同 JS
来源：http://wcm.sufxvd.cn

Java: 方法内为块级作用域
来源：http://ydt.fehbvm.com

Go:   花括号块级作用域
来源：http://xco.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fjs.zhixingplan.top

C#:   块级作用域
来源：http://joj.sweek.top

[C11] 模块导入与导出
来源：http://rcb.yvedp.cn

Py:   from module import func
来源：http://ega.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hii.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nbl.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rim.52xcode.cn

Java: import java.util.List;
来源：http://ucz.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qlx.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://hfn.meibo888.top

C#:   using System.Text;
来源：http://drr.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://zyv.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://aml.tianlin.xyz


<!-- 参考信息 -->