代发 wailian999

Ruby: a, b = b, a
来源：http://edq.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://ihf.cdnleiting.top

[A20] 读取标准输入
来源：http://xip.xziqi.cn

Py:   name = input("请输入：")
来源：http://lnh.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vfi.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kwn.gaohongyu789.top

TS:   // Node.js：readline 模块
来源：http://adq.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://dzo.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gbd.tanke756.top

Ruby: gets.chomp
来源：http://gbc.yj20258888.top

C#:   Console.ReadLine();
来源：http://wsr.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://scn.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://tjk.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vbd.shanyushiyangtech.top

JS:   (3.14159).toFixed(2)
来源：http://fhu.hcnkem.com

TS:   (3.14159).toFixed(2)
来源：http://uff.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://owx.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bwe.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://spm.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://cme.sxryk.cn

[A22] 获取字符串长度
来源：http://izw.daria6918.cn

Py:   len(s)
来源：http://tzz.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lsa.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mri.svipenyu.cn

TS:   s.length
来源：http://ujb.svipenyu.cn

Java: s.length()
来源：http://yee.cqqwz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rty.gaohongyu789.top

Ruby: s.length
来源：http://uft.redwolf501.top

C#:   s.Length
来源：http://fxo.yueranfly.top

[A23] 大小写转换
来源：http://wow.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vzx.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zxm.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kuu.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rdp.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sxp.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pbx.shanyushiyangtech.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ofb.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mcq.zhongyouzk.top

[A24] 去除首尾空白
来源：http://rkp.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xmx.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ryd.hfpthk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eph.tanke756.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wed.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mdw.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://eou.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fom.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bny.xuanzx.com

[A25] 字符串比较
来源：http://zuq.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://pdx.tanke756.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://szd.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fjr.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cjj.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kat.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://juf.jqgufenzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hjy.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cky.cqqwz.cn

[A26] 类型转换总览
来源：http://cgk.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xan.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oaq.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uid.316326.xyz

TS:   Number() String() Boolean() x as number
来源：http://fye.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rqx.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pbj.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yzu.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vhq.gotoacloud.top

================================================================================
来源：http://gen.haohaochexian.top

B. 流程控制
来源：http://frj.jinqigfzy.top

================================================================================
来源：http://dkb.fengsongda.top

[B01] 条件判断 if / else
来源：http://hxq.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://eck.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://urt.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bqa.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sls.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jbp.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cic.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hyk.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gei.uphjek.com

[B02] 多分支 else if / elif
来源：http://mfy.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ppf.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qac.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://afr.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oiy.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdy.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dau.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bbh.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdp.zhijiandao.cn

[B03] switch / match / case
来源：http://ffi.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cid.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lpx.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://igj.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xjt.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://agz.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://utu.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xya.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pbj.zhaomingkeji.xyz

[B04] for 计数循环
来源：http://qym.uphjek.com

Py:   for i in range(10): print(i)
来源：http://fyd.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jdp.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gew.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://obw.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fss.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://efb.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://kvb.xingfuxueyuan.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jqj.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://gjd.uphjek.com

Py:   for item in arr: print(item)
来源：http://hsj.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ybr.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jye.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://itl.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mvh.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nvf.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://bmu.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uuq.yj20258.top

[B06] 遍历字典 / 对象
来源：http://azw.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://hjd.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mnl.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qah.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://szp.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mgv.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://opq.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hpu.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sqh.xylfe.cn

[B07] while 循环
来源：http://dws.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://erz.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://fze.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://avx.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://ohd.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://uvr.shzxlz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sif.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://wwt.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://bgo.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://woj.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://evu.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jvv.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://wpp.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://dfk.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://ksj.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vxj.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://nbf.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://umv.zdqjudy.top

[B09] break 与 continue
来源：http://zzn.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zgd.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gdp.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qed.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://efd.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yiz.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oqj.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lsd.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywi.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://oge.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gbp.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cqq.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xbd.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zio.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vwi.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hbj.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ggv.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nha.smart0.xyz

[B11] 生成数字序列 / 区间
来源：http://qkm.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://vgb.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://vsv.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rnn.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aoo.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://chv.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ich.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://ywz.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://okq.kuanghao11.cn

[B12] 跳出多层循环
来源：http://rcv.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hty.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://phg.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://izp.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uty.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fcr.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pse.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tqt.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hjr.uphjek.com

[B13] 判断是否为数字
来源：http://snc.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://qkn.bbcook.cn

PHP:  is_numeric($x)
来源：http://ydf.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://krg.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ngs.yanxiufei.cn

Java: x instanceof Number
来源：http://hei.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://exg.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://grp.mhx1999.top

C#:   x is int or double or decimal
来源：http://zso.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://qez.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iln.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kwi.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://htn.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://jqd.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://csc.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fti.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://xok.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lpm.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://iqk.yvedp.cn

Py:   a and b or not c
来源：http://sud.yj20258888.top

PHP:  $a && $b || !$c
来源：http://ejj.gzhubu.top

JS:   a && b || !c
来源：http://rer.tian-w.cn

TS:   a && b || !c
来源：http://jtl.zhixingplan.top

Java: a && b || !c
来源：http://xys.nanxinkj.top

Go:   a && b || !c
来源：http://scl.haohaochexian.top

Ruby: a && b || !c
来源：http://bhg.vehdjk.com

C#:   a && b || !c
来源：http://qzv.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mwp.jianghu66.top

Py:   if not data: return
来源：http://irm.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://ecp.sufxvd.cn

JS:   if (!data) return;
来源：http://kug.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://evt.zhixingplan.top

Java: if (data == null) return;
来源：http://ghn.yongpay.top

Go:   if data == nil { return }
来源：http://suw.mhx1999.top

Ruby: return if data.nil?
来源：http://evn.fengsongda.top

C#:   if (data == null) return;
来源：http://ckf.hnxiangtu.top

================================================================================
来源：http://zic.zhixingplan.top

C. 函数与作用域
来源：http://tpz.nwbrower.top

================================================================================
来源：http://vrj.yongpay.top

[C01] 定义函数
来源：http://pyu.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://nkx.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ost.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://nhh.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cuz.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lqg.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://hvw.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://pnv.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nsf.iojbl.cn

[C02] 默认参数
来源：http://bjm.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://bor.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xrp.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://enk.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mgl.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://abz.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://emn.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://bkq.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://tqv.yuxming.cn

[C03] 可变参数
来源：http://pmd.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://zro.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ttq.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bvl.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dti.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://axz.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ezb.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kxa.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pcl.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://wqs.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vzi.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nbm.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ggj.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gge.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://avs.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://iuq.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://xle.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://lyd.wangshuangyany.cn

[C05] 返回多个值
来源：http://ilz.ppjwa.cn

Py:   return a, b
来源：http://vut.smart0.xyz

PHP:  return [$a, $b];
来源：http://hgg.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://chb.yj20258888.top

TS:   return { a, b };
来源：http://rto.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qpu.hcnkem.com

Go:   return a, b
来源：http://lfc.jinqigufen.top

Ruby: return a, b
来源：http://gam.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://mug.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://uor.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://gwb.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yqb.cdnleiting.top

JS:   const square = x => x * x;
来源：http://ccw.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://zpn.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rwg.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://ams.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://qhs.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://wdq.yueranfly.top

[C07] 把函数作为参数传入
来源：http://rjy.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zcy.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kro.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lrg.tanke756.top

TS:   arr.map(String)
来源：http://peh.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bcw.redwolf501.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qcx.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://ajb.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://guk.fehbvm.com

[C08] 闭包
来源：http://xtf.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dqs.jqgufenzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qbf.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ylo.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fvp.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eye.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cwt.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tqb.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wbu.jqgfzy.top

[C09] 递归
来源：http://yfz.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blp.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pyr.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xkf.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vou.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jpt.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ttm.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xgg.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uro.52xcode.cn

[C10] 变量作用域
来源：http://moh.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wbv.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fne.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rxz.guowangkeji.top


<!-- 参考信息 -->