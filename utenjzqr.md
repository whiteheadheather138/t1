代发 wailian999

Ruby: a, b = b, a
来源：http://dba.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://rqf.316326.xyz

[A20] 读取标准输入
来源：http://dsl.feifeiyinyue.top

Py:   name = input("请输入：")
来源：http://bby.sweek.top

PHP:  $name = trim(fgets(STDIN));
来源：http://myo.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ofq.yvedp.cn

TS:   // Node.js：readline 模块
来源：http://trf.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://mog.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://boz.yangfankeji.com

Ruby: gets.chomp
来源：http://pdo.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://ycj.redwolf501.top

[A21] 保留指定小数位输出
来源：http://skr.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://hkp.yonumen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zqj.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://ndl.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://mxf.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://gut.chenjidiqi.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lpr.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://zzc.cheryme.top

C#:   3.14159.ToString("F2")
来源：http://cdz.cheryme.top

[A22] 获取字符串长度
来源：http://eln.jlsjyb.cn

Py:   len(s)
来源：http://wwi.zhiwuduotai.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nlr.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kai.smart0.xyz

TS:   s.length
来源：http://nny.zycfv.cn

Java: s.length()
来源：http://vwn.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yet.ywan-chungtsiang.top

Ruby: s.length
来源：http://lad.fanxiaobao.xyz

C#:   s.Length
来源：http://dlh.shuidangran.top

[A23] 大小写转换
来源：http://ygl.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://rpa.jianghu66.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hic.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://opz.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mxe.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mqn.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gzb.cqqwz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lda.wangdashe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nog.nanxinkj.top

[A24] 去除首尾空白
来源：http://rcf.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xfk.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zmw.xuanzx.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dij.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nxr.sjlbkw.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tdz.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://lcu.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ozh.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://paw.kuanghao11.cn

[A25] 字符串比较
来源：http://aee.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://jpk.sjlbkw.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gro.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rxj.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://myt.jinghuilouyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hsl.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bju.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nqu.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zex.sysykeji.top

[A26] 类型转换总览
来源：http://ebn.cucudq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sdt.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ssd.redwolf501.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pjb.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://iwq.nwbrower.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://knm.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tht.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nds.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qcn.shangyingyoupin.top

================================================================================
来源：http://cyj.wangshuangyany.cn

B. 流程控制
来源：http://rww.gotoacloud.top

================================================================================
来源：http://poo.c1oappe.top

[B01] 条件判断 if / else
来源：http://ecp.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qxq.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cze.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kyg.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wjs.andypj.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://bwf.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://guq.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zhd.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zut.chenjidiqi.icu

[B02] 多分支 else if / elif
来源：http://nlm.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qiz.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wao.ehwqpu.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ows.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uks.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zzl.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kvm.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pio.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijb.cucudq.cn

[B03] switch / match / case
来源：http://fdp.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sqe.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jem.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://phb.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gaq.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rqa.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cnf.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yyo.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nwk.52xcode.cn

[B04] for 计数循环
来源：http://qos.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://ftp.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://obr.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xxn.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ksf.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kce.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zgr.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://ixy.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ble.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://git.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://lhp.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://stj.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vac.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mxb.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jhq.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hvj.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://cqp.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fof.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://wkg.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rbv.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ehy.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jnw.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kgy.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uok.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ers.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eep.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kmi.shuidangran.top

[B07] while 循环
来源：http://mxu.yueranfly.top

Py:   while i < 10: i += 1
来源：http://bmy.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://red.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://ikb.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://iqm.316326.xyz

Java: while (i < 10) { i++; }
来源：http://eci.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fjb.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://eku.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://yib.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://yyg.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://tpa.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://alu.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://aum.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://igk.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://xsc.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zpi.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://znv.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://iwc.havefunace.top

[B09] break 与 continue
来源：http://cwi.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rwk.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qfv.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xig.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vno.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fps.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ylu.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zkc.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tur.epnwcf.com

[B10] 遍历同时拿索引
来源：http://rbr.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ajg.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pad.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yox.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jlo.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wnh.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://psz.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://enb.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oly.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://dpf.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://qeh.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://fkj.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jux.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hyd.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kse.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ncp.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://huo.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dpt.fzhhl.top

[B12] 跳出多层循环
来源：http://tqy.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wfz.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ysm.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mlx.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rug.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bfi.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wcv.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fob.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lwz.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://svn.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://lch.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://nsk.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uag.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yai.guowangkeji.top

Java: x instanceof Number
来源：http://ybf.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vxx.yonumen.top

Ruby: x.is_a?(Numeric)
来源：http://vnn.0kj1m.cn

C#:   x is int or double or decimal
来源：http://rtl.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://zwg.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://esn.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://isd.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://txr.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://cgk.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fow.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pth.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://ddq.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dks.iojbl.cn

[B15] 布尔运算与取反
来源：http://vxn.daria6918.cn

Py:   a and b or not c
来源：http://qvb.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://lkx.nanxuanxn.top

JS:   a && b || !c
来源：http://byd.cdnleiting.top

TS:   a && b || !c
来源：http://zwm.meibo888.top

Java: a && b || !c
来源：http://uut.gaohongyu789.top

Go:   a && b || !c
来源：http://qua.yj20258888.top

Ruby: a && b || !c
来源：http://hqx.fktsv.cn

C#:   a && b || !c
来源：http://zpt.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://skt.snrcjt.cn

Py:   if not data: return
来源：http://rjo.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://olm.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://mcf.zhengqikj.top

TS:   if (!data) return;
来源：http://dcb.zhixingplan.top

Java: if (data == null) return;
来源：http://phj.yfazqb.com

Go:   if data == nil { return }
来源：http://lbs.guowangkeji.top

Ruby: return if data.nil?
来源：http://jqi.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://uut.tanke756.top

================================================================================
来源：http://htk.smart0.xyz

C. 函数与作用域
来源：http://jtb.jqgufenzy.top

================================================================================
来源：http://fif.shzxlz.cn

[C01] 定义函数
来源：http://ysx.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://qru.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kds.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://omr.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qox.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dfm.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://crv.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://vkz.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lbg.daria6918.cn

[C02] 默认参数
来源：http://vxq.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://jfp.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cnz.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://xmf.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mzm.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dxg.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rtc.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://zwb.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://obr.pengpengdd.cyou

[C03] 可变参数
来源：http://ibc.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://spm.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://law.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://arg.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qko.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jyr.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://csj.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://vgv.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cde.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://won.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iqd.52xcode.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hew.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kfq.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dny.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://pxq.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://syo.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://htm.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://diw.shzxlz.cn

[C05] 返回多个值
来源：http://xmb.bjfxy.top

Py:   return a, b
来源：http://hay.zhixingplan.top

PHP:  return [$a, $b];
来源：http://oli.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://kkl.gogol.net.cn

TS:   return { a, b };
来源：http://sex.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gpi.shanyushiyangkeji.top

Go:   return a, b
来源：http://cak.yj20258.top

Ruby: return a, b
来源：http://mgh.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://jbl.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://jqz.havefunace.top

Py:   square = lambda x: x * x
来源：http://dau.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zci.birdmap.top

JS:   const square = x => x * x;
来源：http://jfh.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://xmu.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ire.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qbl.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://sdd.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iwl.mhx1999.top

[C07] 把函数作为参数传入
来源：http://mxt.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lax.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://odd.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fmj.hammf.cn

TS:   arr.map(String)
来源：http://pyw.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yga.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vmg.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://juz.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rff.yanxiufei.cn

[C08] 闭包
来源：http://oaf.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ohi.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ojc.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rwi.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dhj.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://siu.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dtr.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tft.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gmz.redwolf501.top

[C09] 递归
来源：http://ikh.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://klf.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xmi.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ezd.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ckw.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zwa.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ola.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qpy.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nip.chenzaomai.com

[C10] 变量作用域
来源：http://gfl.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jxd.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lwy.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xhv.ehwqpu.com


<!-- 参考信息 -->