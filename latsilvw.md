代发 wailian999

JS:   [a, b] = [b, a];
来源：http://hwc.316326.xyz

TS:   [a, b] = [b, a];
来源：http://vuw.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://qll.jyoumei.cn

Go:   a, b = b, a
来源：http://gcd.bjfxy.top

Ruby: a, b = b, a
来源：http://yuc.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://pwd.hongshengwenyu.top

[A20] 读取标准输入
来源：http://mxy.pengpengdd.cyou

Py:   name = input("请输入：")
来源：http://spv.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cmz.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ruh.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://ljr.yvedp.cn

Java: new Scanner(System.in).nextLine()
来源：http://rum.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://knv.ehwqpu.com

Ruby: gets.chomp
来源：http://pgf.svipenyu.cn

C#:   Console.ReadLine();
来源：http://rep.hammf.cn

[A21] 保留指定小数位输出
来源：http://kqs.hcnkem.com

Py:   f"{3.14159:.2f}"
来源：http://sgj.sweek.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wgf.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://vna.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://thd.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://unu.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://upc.xylfe.cn

Ruby: format("%.2f", 3.14159)
来源：http://syx.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://qfa.hammf.cn

[A22] 获取字符串长度
来源：http://qbo.nwbrower.top

Py:   len(s)
来源：http://wom.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ucu.chenlongwang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lei.tianlin.xyz

TS:   s.length
来源：http://pcl.guannengcc.top

Java: s.length()
来源：http://sfp.yuxming.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wln.shangyingyoupin.top

Ruby: s.length
来源：http://oqd.havefunace.top

C#:   s.Length
来源：http://mgz.uphjek.com

[A23] 大小写转换
来源：http://vyv.hfpthk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mvg.aizwys.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gnf.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jru.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iiw.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vmv.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kly.jinqigufen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ntc.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wsd.ivvv.top

[A24] 去除首尾空白
来源：http://dmg.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gkf.yongpay.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rbq.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fnv.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pmn.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ezl.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://ktn.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uvl.meibo888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cxe.aibaodan.cn

[A25] 字符串比较
来源：http://inc.wangshuangyany.cn

Py:   s1 == s2; s1 != s2
来源：http://mgc.zhiwuduotai.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qnv.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iki.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kgh.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://prj.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qcl.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fwm.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bff.nanxinkj.top

[A26] 类型转换总览
来源：http://vwp.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rtj.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://taw.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aay.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://pmq.xinyue.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jsq.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ypo.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lxw.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nag.hesvh.cn

================================================================================
来源：http://nfd.gaohongyu789.top

B. 流程控制
来源：http://gvd.pycfn.com

================================================================================
来源：http://qej.zhengqikj.top

[B01] 条件判断 if / else
来源：http://cvn.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sjw.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wvk.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://usf.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fsx.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fzl.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mbc.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ont.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nps.dianchejie.cn

[B02] 多分支 else if / elif
来源：http://hiw.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aiq.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aml.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pdz.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jic.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lkv.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pbn.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yna.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfl.wangdashe.top

[B03] switch / match / case
来源：http://nzf.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gft.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://noo.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dzy.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aso.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dxu.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lid.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cxr.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sgk.nanxuanxn.top

[B04] for 计数循环
来源：http://aqp.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://hej.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pqr.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qft.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tzn.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qfi.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wnl.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://qsz.meibo888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nsc.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://kre.52xcode.cn

Py:   for item in arr: print(item)
来源：http://zjq.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bae.feifeiyinyue.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fve.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://par.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lum.mhx1999.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://caz.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://exd.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jxv.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://lfw.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://odp.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nhc.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ofp.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xtd.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lpy.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://coq.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vqb.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uad.52xcode.cn

[B07] while 循环
来源：http://bjc.xziqi.cn

Py:   while i < 10: i += 1
来源：http://emx.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://jff.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://kjv.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://abw.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://slw.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cnm.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://tfg.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://tyq.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://bli.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://saj.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://fce.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://ekt.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://dek.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://fjq.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bbq.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://lbg.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://zgv.ybcxt.top

[B09] break 与 continue
来源：http://wdl.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hwc.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pey.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ugg.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eqm.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glk.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xzr.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rei.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jiq.c1oappe.top

[B10] 遍历同时拿索引
来源：http://vtt.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rdd.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wnr.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zte.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://csc.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jrl.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zkn.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ruq.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://szz.cheryme.top

[B11] 生成数字序列 / 区间
来源：http://qtp.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://oqt.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://jml.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hho.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zvc.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://thk.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zjf.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://vyv.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wdf.cqqwz.cn

[B12] 跳出多层循环
来源：http://aei.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qzg.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://njb.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zgx.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eew.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bke.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dez.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://joh.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hky.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://gzp.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://pkm.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://xut.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bxa.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://peq.yj20258.top

Java: x instanceof Number
来源：http://zbj.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ify.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://sth.jianghu66.top

C#:   x is int or double or decimal
来源：http://mwh.sweek.top

[B14] 判断值是否在集合内
来源：http://ves.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fyc.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mot.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://thn.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://gxg.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tsr.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jbb.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://exd.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zza.gogol.net.cn

[B15] 布尔运算与取反
来源：http://hbx.cucudq.cn

Py:   a and b or not c
来源：http://hxz.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://bcv.mhx1999.top

JS:   a && b || !c
来源：http://lis.fzhhl.top

TS:   a && b || !c
来源：http://rlk.vqdsnc.cn

Java: a && b || !c
来源：http://csa.zhengqikj.top

Go:   a && b || !c
来源：http://wso.uphjek.com

Ruby: a && b || !c
来源：http://hju.gaohongyu789.top

C#:   a && b || !c
来源：http://fnq.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://ppa.jinqigfzy.top

Py:   if not data: return
来源：http://xha.sweek.top

PHP:  if (!$data) { return; }
来源：http://ltp.shangyingyoupin.top

JS:   if (!data) return;
来源：http://tin.jianghu66.top

TS:   if (!data) return;
来源：http://nwr.yangfankeji.com

Java: if (data == null) return;
来源：http://art.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://gay.bbcook.cn

Ruby: return if data.nil?
来源：http://evk.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://cpv.yuanzhike.top

================================================================================
来源：http://ffi.yuxming.cn

C. 函数与作用域
来源：http://jwb.smart0.xyz

================================================================================
来源：http://bza.vehdjk.com

[C01] 定义函数
来源：http://yrn.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://apq.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ela.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://gxv.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://plk.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://whq.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://eah.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://nso.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pzh.bbcook.cn

[C02] 默认参数
来源：http://oyq.sweek.top

Py:   def greet(name="World"): return name
来源：http://uiv.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ayq.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://kty.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://scf.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yki.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fks.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://nzp.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://atp.sweek.top

[C03] 可变参数
来源：http://ubf.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://yab.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pbs.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kfn.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wjy.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jdc.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://spc.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://mib.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jow.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://opr.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vlb.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vuu.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wxj.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jkn.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://wda.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://bwk.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://nad.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://gsl.jiagoushi.top

[C05] 返回多个值
来源：http://sah.hysaishi.cn

Py:   return a, b
来源：http://ywp.pycfn.com

PHP:  return [$a, $b];
来源：http://npm.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nvn.shanyushiyangtech.top

TS:   return { a, b };
来源：http://qyp.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gbh.hfpthk.cn

Go:   return a, b
来源：http://bjm.yuanzhike.top

Ruby: return a, b
来源：http://foa.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://nxa.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://irc.hcnkem.com

Py:   square = lambda x: x * x
来源：http://lee.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://psd.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://djw.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://wqm.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lcy.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lrd.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://hxj.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://pbi.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://wcu.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ycy.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jrq.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zey.daxiang520.top

TS:   arr.map(String)
来源：http://qfl.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zfk.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xav.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://cxh.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lhf.wangshuangyany.cn

[C08] 闭包
来源：http://yii.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ekr.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pci.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dxo.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hqn.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://etf.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jft.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cac.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://puf.tarul.cn

[C09] 递归
来源：http://ctz.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aav.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nha.daxiang520.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dgh.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jte.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cvv.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dmn.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gis.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://snt.hongshengwenyu.top


<!-- 参考信息 -->