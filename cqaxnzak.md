代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://dyp.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://orp.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://pqa.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://djs.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://njb.uphjek.com

Ruby: gets.chomp
来源：http://jjl.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://cbg.meibo888.top

[A21] 保留指定小数位输出
来源：http://nsa.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://qaa.zdqjudy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yqy.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://ktt.iojbl.cn

TS:   (3.14159).toFixed(2)
来源：http://pkq.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://vxu.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fws.wangshuangyany.cn

Ruby: format("%.2f", 3.14159)
来源：http://bfu.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://pne.zhoulong.xyz

[A22] 获取字符串长度
来源：http://dro.uphjek.com

Py:   len(s)
来源：http://vwh.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://own.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mhn.yuanzhike.top

TS:   s.length
来源：http://elz.tanke756.top

Java: s.length()
来源：http://nva.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dft.fanxiaobao.xyz

Ruby: s.length
来源：http://lvz.shzxlz.cn

C#:   s.Length
来源：http://bzd.ppjwa.cn

[A23] 大小写转换
来源：http://wsp.ydzc1.top

Py:   s.upper(); s.lower(); s.title()
来源：http://oaq.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bli.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pon.yonumen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jqh.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aqt.hammf.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tks.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yqt.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gkn.chenzaomai.com

[A24] 去除首尾空白
来源：http://sdx.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vwv.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gzk.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://apv.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://adj.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hri.zhengqikj.top

Go:   strings.TrimSpace(s)
来源：http://rse.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ohm.meibo888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yfw.chenzaomai.com

[A25] 字符串比较
来源：http://vbp.0kj1m.cn

Py:   s1 == s2; s1 != s2
来源：http://qzp.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tkn.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://esp.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ipq.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://paz.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qcj.fehbvm.com

Ruby: s1 == s2; s1 <=> s2
来源：http://akd.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bvi.cqqwz.cn

[A26] 类型转换总览
来源：http://poj.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pak.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://inm.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qig.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://cul.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sgy.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://exw.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://btm.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mrp.haohaochexian.top

================================================================================
来源：http://wgq.hywenlv.cn

B. 流程控制
来源：http://zgv.yj20258888.top

================================================================================
来源：http://xzi.hysaishi.cn

[B01] 条件判断 if / else
来源：http://blb.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://ues.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://znj.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zvk.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pql.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wui.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ubb.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wrv.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xly.yongpay.top

[B02] 多分支 else if / elif
来源：http://wur.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jjf.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iak.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rew.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xsa.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mre.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gvb.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xoe.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sdg.daxiang520.top

[B03] switch / match / case
来源：http://gbr.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xbb.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ken.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aqa.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ftm.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://heb.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lcs.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ywg.nanxinkj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://stk.andypj.xyz

[B04] for 计数循环
来源：http://jjr.yongpay.top

Py:   for i in range(10): print(i)
来源：http://iaj.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eru.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mws.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nba.fanxiaobao.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ijt.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ubr.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://awz.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uzk.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://kyh.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://uut.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mwl.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lcv.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mkz.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ypc.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lul.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://msi.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bzx.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://ntq.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rkz.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://you.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ela.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zwu.jyoumei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lfj.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ffj.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vkp.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kbe.nanxuanxn.top

[B07] while 循环
来源：http://gmz.yfazqb.com

Py:   while i < 10: i += 1
来源：http://lbs.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://vue.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://djh.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://uiy.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://xob.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oro.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://fou.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://wmc.cashguo.top

[B08] do-while（至少执行一次）
来源：http://hgk.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://hoo.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xuv.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://gno.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://dvi.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://avi.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://utm.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xjr.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://grp.svipenyu.cn

[B09] break 与 continue
来源：http://wuu.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vli.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yqu.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vym.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xki.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rje.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fkd.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nof.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpy.yvedp.cn

[B10] 遍历同时拿索引
来源：http://tkc.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jcm.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hle.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hlr.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://glz.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uwn.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wnl.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rpo.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qbx.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://ixk.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://jne.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://wdf.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qwf.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mvz.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zvb.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kqd.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://srz.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xbr.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://jqz.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iym.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ros.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kje.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cos.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vqg.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://afm.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fxq.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zei.zhixingplan.top

[B13] 判断是否为数字
来源：http://vyt.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://xcw.cheryme.top

PHP:  is_numeric($x)
来源：http://pqx.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zej.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xcp.haohaochexian.top

Java: x instanceof Number
来源：http://mfz.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kae.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://uey.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://zsj.jianghu66.top

[B14] 判断值是否在集合内
来源：http://xqr.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://srt.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ebl.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://joz.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://yic.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lhv.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://osa.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uxs.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dzd.tanke756.top

[B15] 布尔运算与取反
来源：http://joh.hnqzz.top

Py:   a and b or not c
来源：http://udj.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://bod.shanyushiyangtech.top

JS:   a && b || !c
来源：http://ixj.shuidangran.top

TS:   a && b || !c
来源：http://trl.zhengqikj.top

Java: a && b || !c
来源：http://izg.jqgfzy.top

Go:   a && b || !c
来源：http://mix.yj202588.top

Ruby: a && b || !c
来源：http://yyi.hammf.cn

C#:   a && b || !c
来源：http://dst.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://wfl.hysaishi.cn

Py:   if not data: return
来源：http://wrt.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://hjv.cashguo.top

JS:   if (!data) return;
来源：http://fdt.nwbrower.top

TS:   if (!data) return;
来源：http://fmi.yvedp.cn

Java: if (data == null) return;
来源：http://kwd.bbcook.cn

Go:   if data == nil { return }
来源：http://lzc.0kj1m.cn

Ruby: return if data.nil?
来源：http://vzt.yongpay.top

C#:   if (data == null) return;
来源：http://cqd.ehwqpu.com

================================================================================
来源：http://fyb.ehwqpu.com

C. 函数与作用域
来源：http://zsi.zhaomingkeji.xyz

================================================================================
来源：http://cbr.jiagoushi.top

[C01] 定义函数
来源：http://ctu.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://ihv.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xjz.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://ncv.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqg.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fvm.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://vlu.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://xqk.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gjj.hcnkem.com

[C02] 默认参数
来源：http://qwl.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://dxs.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mwh.sjlbkw.cn

JS:   function greet(name = "World") { return name; }
来源：http://ynb.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yip.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zsf.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ovi.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://ztv.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://lmt.birdmap.top

[C03] 可变参数
来源：http://xuf.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://lfz.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bjx.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dni.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xrx.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ict.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pqm.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://zia.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wot.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://rvc.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xlm.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rzd.xuetiantiany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dvh.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://umo.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://pqx.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://gsi.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://xue.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://spv.mhx1999.top

[C05] 返回多个值
来源：http://mbi.jqgfzy.top

Py:   return a, b
来源：http://gmd.sufxvd.cn

PHP:  return [$a, $b];
来源：http://cqj.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kzf.jiagoushi.top

TS:   return { a, b };
来源：http://bmu.shzxlz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ahy.guowangkeji.top

Go:   return a, b
来源：http://ase.shzxlz.cn

Ruby: return a, b
来源：http://xax.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://xvj.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://tlj.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://oby.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lmx.uphjek.com

JS:   const square = x => x * x;
来源：http://xmj.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://tki.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pwd.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://kcu.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://gfs.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qyn.yj202588.top

[C07] 把函数作为参数传入
来源：http://lxa.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bni.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://msx.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hta.316326.xyz

TS:   arr.map(String)
来源：http://lsc.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tmo.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mhp.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://yjq.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://plw.meibo888.top

[C08] 闭包
来源：http://cdo.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vsj.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://efn.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ysq.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qei.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gtf.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wjh.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kbp.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kkk.hfpthk.cn

[C09] 递归
来源：http://rng.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qqn.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mwn.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uit.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vtj.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zel.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://joo.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hog.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://drc.vehdjk.com

[C10] 变量作用域
来源：http://nqj.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xng.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iay.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yjx.ppjwa.cn

TS:   同 JS
来源：http://xit.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://mms.jlsjyb.cn

Go:   花括号块级作用域
来源：http://qpe.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xzp.yonumen.top


<!-- 参考信息 -->