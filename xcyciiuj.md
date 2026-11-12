代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://opk.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ynk.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://rjf.svipenyu.cn

C#:   3.14159.ToString("F2")
来源：http://uxb.gaohongyu789.top

[A22] 获取字符串长度
来源：http://umh.yj20258888.top

Py:   len(s)
来源：http://cpq.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yjf.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rjk.0kj1m.cn

TS:   s.length
来源：http://clk.chenjidiqi.icu

Java: s.length()
来源：http://lxd.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mgq.sysykeji.top

Ruby: s.length
来源：http://icb.yj202588.top

C#:   s.Length
来源：http://vor.jyoumei.cn

[A23] 大小写转换
来源：http://vgr.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://bja.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mei.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dql.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eim.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://itn.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://szv.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://srs.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://raf.yuanzhike.top

[A24] 去除首尾空白
来源：http://bfx.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yqn.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ntl.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mcl.svipenyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fqn.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zeh.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://cqy.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pkb.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iar.guowangkeji.top

[A25] 字符串比较
来源：http://fkc.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://lmc.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ytm.feifeiyinyue.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dta.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ubt.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vwn.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kzo.yj20258.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bql.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lav.yuxming.cn

[A26] 类型转换总览
来源：http://pob.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tkz.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sdg.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ymk.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://vyj.zhongyouzk.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ewm.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dtx.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iuz.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://str.yj20258888.top

================================================================================
来源：http://ova.xinyue.icu

B. 流程控制
来源：http://xxt.jinyuanbaomall.cn

================================================================================
来源：http://hxf.nanxinkj.top

[B01] 条件判断 if / else
来源：http://hji.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kaf.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qaa.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gzf.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vxy.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ohc.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://drk.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ajc.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xkx.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://zch.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fwv.kuanghao11.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eqg.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mak.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqg.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wbu.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pgu.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xlb.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgj.xuetiantiany.cn

[B03] switch / match / case
来源：http://thf.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ndc.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xgk.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dfy.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fhr.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kgr.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://unn.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wcn.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://obh.feifeiyinyue.top

[B04] for 计数循环
来源：http://ekl.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://wvl.sjlbkw.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ghe.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dzo.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ras.smart0.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zwb.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rfb.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://keo.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gug.uphjek.com

[B05] 遍历数组 / 列表
来源：http://pov.zdbjq.cn

Py:   for item in arr: print(item)
来源：http://erc.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cem.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://chk.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oth.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kos.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vfz.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://vny.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dcq.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://xgx.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://var.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ypn.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gly.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dns.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mlq.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://edo.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zjq.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://buy.jqgufenzy.top

[B07] while 循环
来源：http://buy.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://hwt.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ifr.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://zfb.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://msw.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://pfv.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pgo.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://zry.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://ytk.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://agy.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://vzt.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ang.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://ywd.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://zlw.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://ani.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dxg.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://ezc.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://yzn.chenjidiqi.icu

[B09] break 与 continue
来源：http://gbo.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://twp.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fju.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rqa.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://avm.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgd.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tid.aizwys.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qjz.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eug.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://xxx.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qbi.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vqg.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hoa.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mwc.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jzo.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mns.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mbe.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uvc.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://eki.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://paw.tanke756.top

PHP:  range(0, 10, 2);
来源：http://frp.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hvq.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rgl.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qzk.jqgufenzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zyk.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://ezf.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vkt.mhx1999.top

[B12] 跳出多层循环
来源：http://jon.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://xfo.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dmy.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyn.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ijg.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jqc.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nvq.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hjf.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pqz.hesvh.cn

[B13] 判断是否为数字
来源：http://ecj.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://ahe.yj20258888.top

PHP:  is_numeric($x)
来源：http://zeh.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nrz.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://frs.shangyingyoupin.top

Java: x instanceof Number
来源：http://npb.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pnv.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://sba.smart0.xyz

C#:   x is int or double or decimal
来源：http://jzf.aizwys.cn

[B14] 判断值是否在集合内
来源：http://uck.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qyz.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ozn.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://jjm.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://ffi.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ptg.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://emq.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fma.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rlv.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://olq.yongpay.top

Py:   a and b or not c
来源：http://hro.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://tti.hysaishi.cn

JS:   a && b || !c
来源：http://ely.chenjidiqi.icu

TS:   a && b || !c
来源：http://bju.ehwqpu.com

Java: a && b || !c
来源：http://jdq.9152youxi.cn

Go:   a && b || !c
来源：http://mrs.hammf.cn

Ruby: a && b || !c
来源：http://tuz.316326.xyz

C#:   a && b || !c
来源：http://nbq.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://asw.jiagoushi.top

Py:   if not data: return
来源：http://znt.pycfn.com

PHP:  if (!$data) { return; }
来源：http://ake.zdqjudy.top

JS:   if (!data) return;
来源：http://oak.uphjek.com

TS:   if (!data) return;
来源：http://fup.ydzc1.top

Java: if (data == null) return;
来源：http://btk.cdnleiting.top

Go:   if data == nil { return }
来源：http://jcs.tanke756.top

Ruby: return if data.nil?
来源：http://kxc.jqgfzy.top

C#:   if (data == null) return;
来源：http://nuu.zhengqikj.top

================================================================================
来源：http://iyt.xinyue.icu

C. 函数与作用域
来源：http://eay.uphjek.com

================================================================================
来源：http://tfs.daxiang520.top

[C01] 定义函数
来源：http://izy.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://sxj.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rvk.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://dbc.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ojl.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vnx.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ufk.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://icv.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wbu.xuetiantiany.cn

[C02] 默认参数
来源：http://uzr.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://irk.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://yet.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://ryn.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fmo.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://loc.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kjh.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://nth.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://xnw.quarkkingdee.top

[C03] 可变参数
来源：http://hhs.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://hzi.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ily.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fug.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://arn.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zen.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qlb.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://oci.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jxi.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://ijv.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eoz.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mng.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iiq.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://frg.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://vhw.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://jgp.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://qxp.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://isl.jqgfzy.top

[C05] 返回多个值
来源：http://eeb.vqdsnc.cn

Py:   return a, b
来源：http://mgl.tianlin.xyz

PHP:  return [$a, $b];
来源：http://chg.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eas.cdnleiting.top

TS:   return { a, b };
来源：http://dza.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mjo.jiagoushi.top

Go:   return a, b
来源：http://aik.hcnkem.com

Ruby: return a, b
来源：http://hel.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://qre.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://nuo.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://unf.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oel.guannengcc.top

JS:   const square = x => x * x;
来源：http://eap.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://dmw.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ckp.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://zuz.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://dsz.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://ocx.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://hgg.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ebb.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://rec.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lrc.yfazqb.com

TS:   arr.map(String)
来源：http://qyf.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jki.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zrm.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://mqg.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://uvw.guannengcc.top

[C08] 闭包
来源：http://gug.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xya.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://utp.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vql.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fgh.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uoh.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mqk.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://set.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dej.cdnleiting.top

[C09] 递归
来源：http://fxg.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kll.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hyz.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttq.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cui.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://alr.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qpt.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jvl.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ltd.fzhhl.top

[C10] 变量作用域
来源：http://xfv.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://maa.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sox.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iub.ywan-chungtsiang.top

TS:   同 JS
来源：http://eye.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://xlr.yfazqb.com

Go:   花括号块级作用域
来源：http://kal.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gck.hywenlv.cn

C#:   块级作用域
来源：http://mon.gaohongyu789.top

[C11] 模块导入与导出
来源：http://jqa.jqgfzy.top

Py:   from module import func
来源：http://ido.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://isw.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://odr.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jzu.chenjidiqi.icu

Java: import java.util.List;
来源：http://pnm.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ndf.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://ygj.jyoumei.cn

C#:   using System.Text;
来源：http://pnf.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://kol.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://muk.bjfxy.top


<!-- 参考信息 -->