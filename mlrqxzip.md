代发 wailian999

Ruby: a, b = b, a
来源：http://ixe.quarkkingdee.top

C#:   (a, b) = (b, a);
来源：http://nts.bjfxy.top

[A20] 读取标准输入
来源：http://kgl.yuxming.cn

Py:   name = input("请输入：")
来源：http://wjk.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ost.hongshengwenyu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pjp.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://bwi.zhengqikj.top

Java: new Scanner(System.in).nextLine()
来源：http://chr.nanxuanxn.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kyb.jiagoushi.top

Ruby: gets.chomp
来源：http://uaf.yvedp.cn

C#:   Console.ReadLine();
来源：http://gtf.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://xgm.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://qcf.jlsjyb.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://flf.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://qwt.zycfv.cn

TS:   (3.14159).toFixed(2)
来源：http://ihh.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://bkg.vehdjk.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://now.andypj.xyz

Ruby: format("%.2f", 3.14159)
来源：http://dkg.sweek.top

C#:   3.14159.ToString("F2")
来源：http://tbu.jlsjyb.cn

[A22] 获取字符串长度
来源：http://znn.c1oappe.top

Py:   len(s)
来源：http://ccu.iojbl.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ggk.zycfv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eur.zhijiandao.cn

TS:   s.length
来源：http://wsw.guowangkeji.top

Java: s.length()
来源：http://xqi.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vow.jinqigfzy.top

Ruby: s.length
来源：http://wqk.shangyingyoupin.top

C#:   s.Length
来源：http://yuf.aizwys.cn

[A23] 大小写转换
来源：http://qeu.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pkm.zhixingplan.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ssu.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zgr.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ifx.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pab.hfpthk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dfo.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nvp.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dhc.yonumen.top

[A24] 去除首尾空白
来源：http://mce.hfpthk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vyc.zhongyouzk.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://htd.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vii.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lgt.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vva.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://fdz.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pgi.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cnu.jinqigfzy.top

[A25] 字符串比较
来源：http://haz.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://lcb.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uah.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://org.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yvy.fehbvm.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lju.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://szi.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bgx.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iym.xziqi.cn

[A26] 类型转换总览
来源：http://smo.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dyw.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yif.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vrm.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://gji.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ldj.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lhz.zycfv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://omk.ydjk.org.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://boe.shangyingyoupin.top

================================================================================
来源：http://fkk.dashuyun.cn

B. 流程控制
来源：http://yvh.gotoacloud.top

================================================================================
来源：http://opo.jlsjyb.cn

[B01] 条件判断 if / else
来源：http://xtt.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://nsz.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dvc.hammf.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ztd.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ymv.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://jub.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wdw.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jjv.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lgy.tian-w.cn

[B02] 多分支 else if / elif
来源：http://jdu.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rsg.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xca.cashguo.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kuf.xylfe.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ktt.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzy.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lcv.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://czi.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwk.haohaochexian.top

[B03] switch / match / case
来源：http://cyb.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nke.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vhd.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fch.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vth.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dqh.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xqn.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lrq.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://awd.fktsv.cn

[B04] for 计数循环
来源：http://ioj.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://oll.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lzi.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lrt.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvj.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tul.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vvo.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://eqt.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gph.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://krz.gzhubu.top

Py:   for item in arr: print(item)
来源：http://usi.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ivf.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jvm.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ybs.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://zkv.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tta.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://eej.zycfv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dub.yongpay.top

[B06] 遍历字典 / 对象
来源：http://ycs.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://odh.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uxt.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dlx.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dld.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jth.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rqi.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bvf.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yjk.hnqzz.top

[B07] while 循环
来源：http://zrc.havefunace.top

Py:   while i < 10: i += 1
来源：http://aap.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://riv.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://vel.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://hai.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://aad.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nod.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://ris.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://bgb.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://jth.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://xew.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jqq.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://ihv.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://lde.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://yhv.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rdz.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://pqn.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://jwf.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://igc.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gif.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://egr.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vtj.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skk.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://srh.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ltw.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gwf.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gtq.fktsv.cn

[B10] 遍历同时拿索引
来源：http://gyn.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://slx.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vml.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dkb.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://beu.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jci.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bmo.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fha.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gxt.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://erf.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://zoo.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://dgn.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lve.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xkx.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fdw.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qkd.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://baj.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ojz.hywenlv.cn

[B12] 跳出多层循环
来源：http://wsx.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://crw.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://utt.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gbx.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gkg.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xoe.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uoq.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://luz.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bpm.sweek.top

[B13] 判断是否为数字
来源：http://fte.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://wkl.yangfankeji.com

PHP:  is_numeric($x)
来源：http://uze.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lkt.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dtj.jqgfzy.top

Java: x instanceof Number
来源：http://yrj.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pxr.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://sgs.sufxvd.cn

C#:   x is int or double or decimal
来源：http://mlx.yj20258888.top

[B14] 判断值是否在集合内
来源：http://vre.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jzv.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qio.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://cgr.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://rdx.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dda.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ihb.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://lps.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://acc.nwbrower.top

[B15] 布尔运算与取反
来源：http://ixg.ehwqpu.com

Py:   a and b or not c
来源：http://rzx.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://fwx.xuanzx.com

JS:   a && b || !c
来源：http://cgk.xuanzx.com

TS:   a && b || !c
来源：http://hdf.smart0.xyz

Java: a && b || !c
来源：http://lyu.hywenlv.cn

Go:   a && b || !c
来源：http://ese.aibaodan.cn

Ruby: a && b || !c
来源：http://eys.tian-w.cn

C#:   a && b || !c
来源：http://trf.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://ebe.jinqigfzy.top

Py:   if not data: return
来源：http://vnk.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://xbu.cucudq.cn

JS:   if (!data) return;
来源：http://gyo.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://baw.hysaishi.cn

Java: if (data == null) return;
来源：http://xdi.yangfankeji.com

Go:   if data == nil { return }
来源：http://hyn.smart0.xyz

Ruby: return if data.nil?
来源：http://cjz.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://frj.haohaochexian.top

================================================================================
来源：http://mtz.smart0.xyz

C. 函数与作用域
来源：http://ily.zhoulong.xyz

================================================================================
来源：http://qen.tian-w.cn

[C01] 定义函数
来源：http://ior.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://rsn.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oso.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://otk.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmu.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://lcd.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://pfp.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://rlj.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dss.sjlbkw.cn

[C02] 默认参数
来源：http://pgw.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://mie.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lxz.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://djr.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uul.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://yyt.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://urd.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://npq.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://vkm.ydzc1.top

[C03] 可变参数
来源：http://tay.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://lma.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mjk.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://unh.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zpd.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xmb.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hvx.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://enr.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ffw.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://zmy.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://htf.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hbx.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vdj.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xrf.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ipk.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://fbm.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://mvw.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://fvz.yonumen.top

[C05] 返回多个值
来源：http://qxr.hnxiangtu.top

Py:   return a, b
来源：http://ghx.jqgfzy.top

PHP:  return [$a, $b];
来源：http://fjs.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jfg.fengsongda.top

TS:   return { a, b };
来源：http://niz.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nxc.haohaochexian.top

Go:   return a, b
来源：http://gzo.jinyuanbaomall.cn

Ruby: return a, b
来源：http://dxh.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://vcd.tarul.cn

[C06] 匿名函数 / lambda
来源：http://sym.hnqzz.top

Py:   square = lambda x: x * x
来源：http://qnz.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://guv.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://fhj.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://onj.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qyp.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://bed.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://egh.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://utx.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://hkg.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jbd.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://eue.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://unf.havefunace.top

TS:   arr.map(String)
来源：http://zji.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dhc.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ymy.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://yoi.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sii.fanxiaobao.xyz

[C08] 闭包
来源：http://ldp.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nxu.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yfx.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gpt.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ngg.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oue.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mxi.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bev.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kfe.gaohongyu789.top

[C09] 递归
来源：http://jtb.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wsv.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tga.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pol.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kph.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kzp.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://far.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wqb.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://del.yueranfly.top

[C10] 变量作用域
来源：http://tsa.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jlk.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://emn.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sgp.ehwqpu.com


<!-- 参考信息 -->