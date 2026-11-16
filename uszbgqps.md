代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://wxf.shanyushiyangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jlm.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://cdx.ivvv.top

Java: new Scanner(System.in).nextLine()
来源：http://ghd.zhixingplan.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wod.kuanghao11.cn

Ruby: gets.chomp
来源：http://iiw.yvedp.cn

C#:   Console.ReadLine();
来源：http://xif.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://exs.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://bry.yvedp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://put.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://dbo.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://uuc.hcnkem.com

Java: String.format("%.2f", 3.14159)
来源：http://dch.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tfe.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://htu.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://rnp.jinqigufen.top

[A22] 获取字符串长度
来源：http://erk.ydjk.org.cn

Py:   len(s)
来源：http://und.snrcjt.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ktx.sjlbkw.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vxo.smart0.xyz

TS:   s.length
来源：http://vcu.bjfxy.top

Java: s.length()
来源：http://qox.epnwcf.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pfm.sxryk.cn

Ruby: s.length
来源：http://mug.sufxvd.cn

C#:   s.Length
来源：http://wpp.jinqigufen.top

[A23] 大小写转换
来源：http://hyw.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://slq.yuxming.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jzm.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gwl.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://krq.gotoacloud.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qgm.shanyushiyangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gyn.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tgf.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lri.snrcjt.cn

[A24] 去除首尾空白
来源：http://hhg.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jjf.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iey.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ldq.fehbvm.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ejl.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cvv.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://mur.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ott.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eax.ybcxt.top

[A25] 字符串比较
来源：http://ynz.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://hci.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ymb.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rlv.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://edk.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fpm.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bgr.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fcd.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pst.haohaochexian.top

[A26] 类型转换总览
来源：http://dnw.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hno.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://quf.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xij.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://cwb.ybcxt.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://plz.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qug.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aar.hysaishi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hcg.bjfxy.top

================================================================================
来源：http://vik.tianlin.xyz

B. 流程控制
来源：http://dnl.vqdsnc.cn

================================================================================
来源：http://ian.wangdashe.top

[B01] 条件判断 if / else
来源：http://opy.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ksg.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fau.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wwv.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://spp.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sza.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wdk.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vje.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lvg.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://zgl.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mhs.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mgk.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mqn.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dod.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqc.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vjm.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ljy.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buy.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://bty.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nft.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bun.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jnx.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://czd.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jux.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qow.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jes.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fxh.cashguo.top

[B04] for 计数循环
来源：http://qpq.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://txi.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pwl.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://owe.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cgi.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wyj.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dag.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://jzy.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zzg.havefunace.top

[B05] 遍历数组 / 列表
来源：http://rwk.xziqi.cn

Py:   for item in arr: print(item)
来源：http://lao.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aek.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wgn.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rtb.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cso.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kfs.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://jtu.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ojr.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://fnw.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cgo.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tea.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjy.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rnk.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wdm.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bxo.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://izc.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://okd.xingfuxueyuan.xyz

[B07] while 循环
来源：http://vey.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://zjd.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://ppc.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://xap.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://nys.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://mqz.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nma.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://tsx.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://lkh.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://wvv.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://kxn.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://unj.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://gbg.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://plr.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://fmk.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gws.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://ypj.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://mrz.yongpay.top

[B09] break 与 continue
来源：http://xat.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zst.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aoh.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kck.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cju.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ejj.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dnp.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nrg.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgh.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://slx.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uet.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jme.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vca.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xss.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cdr.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vmg.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ttb.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yfk.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://vqh.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://reg.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://ret.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hpg.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npa.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cll.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oam.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://yhc.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://drg.smart0.xyz

[B12] 跳出多层循环
来源：http://klk.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tpl.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dsx.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tgx.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yjj.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dhv.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qlx.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jed.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zep.meibo888.top

[B13] 判断是否为数字
来源：http://das.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://jtd.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://ous.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://itc.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqn.bbcook.cn

Java: x instanceof Number
来源：http://pnc.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rrp.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://edm.shuidangran.top

C#:   x is int or double or decimal
来源：http://urp.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://mkk.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://odm.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jhh.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://wei.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://aqp.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bvi.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jlh.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://glu.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qpp.iojbl.cn

[B15] 布尔运算与取反
来源：http://gtm.yfazqb.com

Py:   a and b or not c
来源：http://xlx.yueranfly.top

PHP:  $a && $b || !$c
来源：http://adk.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://gzw.yj202588.top

TS:   a && b || !c
来源：http://msk.tianlin.xyz

Java: a && b || !c
来源：http://kkk.quarkkingdee.top

Go:   a && b || !c
来源：http://dog.wangdashe.top

Ruby: a && b || !c
来源：http://ixj.gotoacloud.top

C#:   a && b || !c
来源：http://pgf.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://bgw.chenjidiqi.icu

Py:   if not data: return
来源：http://glw.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://evh.sysykeji.top

JS:   if (!data) return;
来源：http://kny.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://jol.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://kzi.andypj.xyz

Go:   if data == nil { return }
来源：http://ijw.ehwqpu.com

Ruby: return if data.nil?
来源：http://pwo.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://thr.dianchejie.cn

================================================================================
来源：http://hwf.havefunace.top

C. 函数与作用域
来源：http://flb.ctjpmb.com

================================================================================
来源：http://emn.pycfn.com

[C01] 定义函数
来源：http://eta.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://xyd.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pxi.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://eft.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qqt.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://fox.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://utr.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://ods.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://syk.yj20258888.top

[C02] 默认参数
来源：http://cpd.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://ulk.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cfr.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://tjl.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://izv.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://dth.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qrp.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://bge.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://pvp.c1oappe.top

[C03] 可变参数
来源：http://dey.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://jhn.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pha.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ivv.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jre.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kvz.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://krw.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://tgi.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ndl.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://rdi.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gjv.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nwq.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gdw.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xrc.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://kvh.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://pew.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://abc.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://suy.jlsjyb.cn

[C05] 返回多个值
来源：http://vet.yuanzhike.top

Py:   return a, b
来源：http://qju.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://zyy.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wkm.yj20258.top

TS:   return { a, b };
来源：http://gyn.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kaf.shanyushiyangkeji.top

Go:   return a, b
来源：http://kyh.fengsongda.top

Ruby: return a, b
来源：http://bke.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://bpf.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://wrf.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://xlq.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rrs.jinqigufen.top

JS:   const square = x => x * x;
来源：http://sel.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://vkp.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://agc.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://ihk.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://qri.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://rgc.gzhubu.top

[C07] 把函数作为参数传入
来源：http://vbv.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pao.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://cit.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://flo.yongpay.top

TS:   arr.map(String)
来源：http://ddy.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://diz.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gld.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://uqh.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kjm.chenjidiqi.icu

[C08] 闭包
来源：http://uml.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://opr.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cxd.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yig.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://doh.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ogo.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yke.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wvb.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wox.vqdsnc.cn

[C09] 递归
来源：http://sso.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://znu.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://izr.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zzl.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dxc.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oof.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://inv.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nne.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hbi.yongpay.top

[C10] 变量作用域
来源：http://agt.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uyt.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kdx.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ngk.fktsv.cn

TS:   同 JS
来源：http://deu.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://rff.tarul.cn

Go:   花括号块级作用域
来源：http://pgg.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tri.dashuyun.cn


<!-- 参考信息 -->