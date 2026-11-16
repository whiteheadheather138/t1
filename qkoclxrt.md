代发 wailian999

Ruby: a, b = b, a
来源：http://aib.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://gfm.shangyingyoupin.top

[A20] 读取标准输入
来源：http://fnb.gzhubu.top

Py:   name = input("请输入：")
来源：http://qsz.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://fqk.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uvi.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://owl.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://uuh.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vhm.svipenyu.cn

Ruby: gets.chomp
来源：http://vhb.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://wcr.cheryme.top

[A21] 保留指定小数位输出
来源：http://nkf.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://cog.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yhx.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://wyv.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://xfi.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://qji.cdnleiting.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vqo.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://lfx.ybcxt.top

C#:   3.14159.ToString("F2")
来源：http://wki.shanyushiyangkeji.top

[A22] 获取字符串长度
来源：http://ggd.zycfv.cn

Py:   len(s)
来源：http://dgm.wangshuangyany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qiv.dianchejie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zfe.0kj1m.cn

TS:   s.length
来源：http://con.aibaodan.cn

Java: s.length()
来源：http://cxi.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://thi.quarkkingdee.top

Ruby: s.length
来源：http://kdo.gogol.net.cn

C#:   s.Length
来源：http://uio.cucudq.cn

[A23] 大小写转换
来源：http://mik.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zyq.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eao.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jex.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cje.quarkkingdee.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ofa.gogol.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tiq.cheryme.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jsz.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://rei.zhongyouzk.top

[A24] 去除首尾空白
来源：http://cwo.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eqx.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iyc.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xuj.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mxi.fehbvm.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wej.zhixingplan.top

Go:   strings.TrimSpace(s)
来源：http://ixa.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tzk.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xdx.snrcjt.cn

[A25] 字符串比较
来源：http://hdn.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://kar.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tob.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gpy.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ojz.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yeh.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wgl.bjfxy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nag.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yrf.zhijiandao.cn

[A26] 类型转换总览
来源：http://bnh.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fof.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fuh.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xfm.epnwcf.com

TS:   Number() String() Boolean() x as number
来源：http://pxa.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gqi.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uju.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://exq.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xof.redwolf501.top

================================================================================
来源：http://sao.epnwcf.com

B. 流程控制
来源：http://vav.chenlongwang.top

================================================================================
来源：http://sgt.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://noj.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://dbz.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sfz.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://igo.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cxe.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ibx.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fqj.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://owp.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bse.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://cdg.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jvt.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ulw.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eiu.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hyl.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ype.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vcv.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tzb.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ynk.quarkkingdee.top

[B03] switch / match / case
来源：http://vhq.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sfl.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pnq.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://utx.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjq.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hjm.jqgfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jtd.hcnkem.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://axf.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bel.xuanzx.com

[B04] for 计数循环
来源：http://eve.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://jao.gaohongyu789.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rga.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://arm.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qgh.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cnb.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lpi.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://vcc.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yzd.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://hnc.mhx1999.top

Py:   for item in arr: print(item)
来源：http://ive.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qha.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fle.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://evl.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bpv.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gsj.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://erx.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gbr.birdmap.top

[B06] 遍历字典 / 对象
来源：http://yth.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://eiy.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jer.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kso.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qkv.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sxu.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tyl.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://npz.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://byx.andypj.xyz

[B07] while 循环
来源：http://afj.iojbl.cn

Py:   while i < 10: i += 1
来源：http://tgf.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://zyp.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://xjw.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://jub.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://eph.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eih.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://enr.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://nso.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://hgh.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://nxy.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vnj.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://exg.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://uzu.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://pyv.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nnt.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://fam.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://jeq.c1oappe.top

[B09] break 与 continue
来源：http://fcy.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zsb.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jhd.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://poz.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjk.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjt.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://doj.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fnm.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sto.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://doq.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://edj.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://icu.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://idy.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hrl.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rpf.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eyp.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nco.cashguo.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hvw.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://spq.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://gzo.uphjek.com

PHP:  range(0, 10, 2);
来源：http://hzv.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mrx.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gbe.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ner.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zpp.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://vuj.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ode.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://sps.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://ltg.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oyp.shanyushiyangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mwr.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgx.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ciu.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qpw.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://miz.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wbt.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://ahb.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://ekp.shzxlz.cn

PHP:  is_numeric($x)
来源：http://brx.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ryl.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uug.pycfn.com

Java: x instanceof Number
来源：http://dfr.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://avu.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://jhe.fzhhl.top

C#:   x is int or double or decimal
来源：http://gbw.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://pjw.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eka.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lxk.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://rcu.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://aoe.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://auz.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://idc.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://wiu.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fgd.bbcook.cn

[B15] 布尔运算与取反
来源：http://paa.gotoacloud.top

Py:   a and b or not c
来源：http://nvu.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://iuy.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://wjq.zhoulong.xyz

TS:   a && b || !c
来源：http://eun.bjfxy.top

Java: a && b || !c
来源：http://wzk.ppjwa.cn

Go:   a && b || !c
来源：http://brc.sjlbkw.cn

Ruby: a && b || !c
来源：http://wdu.havefunace.top

C#:   a && b || !c
来源：http://zjj.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://uul.gaohongyu789.top

Py:   if not data: return
来源：http://yrb.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://mwr.cucudq.cn

JS:   if (!data) return;
来源：http://pje.snrcjt.cn

TS:   if (!data) return;
来源：http://dno.52xcode.cn

Java: if (data == null) return;
来源：http://whe.kuanghao11.cn

Go:   if data == nil { return }
来源：http://qtg.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://yim.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://hix.guowangkeji.top

================================================================================
来源：http://rdo.zhiwuduotai.top

C. 函数与作用域
来源：http://tak.feifeiyinyue.top

================================================================================
来源：http://mmg.0kj1m.cn

[C01] 定义函数
来源：http://jce.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://fzl.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ifs.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://iiu.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ffq.zdbjq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nap.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://viq.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://ndn.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://muu.chenjidiqi.icu

[C02] 默认参数
来源：http://chd.cashguo.top

Py:   def greet(name="World"): return name
来源：http://hmk.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mrj.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wxy.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://maj.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ybw.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rii.sweek.top

Ruby: def greet(name = "World") = name
来源：http://imk.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://yzp.pycfn.com

[C03] 可变参数
来源：http://vhl.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://pdz.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fnk.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nqc.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://krg.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://buy.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://prl.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://vzo.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://znk.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://vrj.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ywk.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fam.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oor.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xsn.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://rgi.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://bdi.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://mlx.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://kqm.nanxinkj.top

[C05] 返回多个值
来源：http://kqu.shangyingyoupin.top

Py:   return a, b
来源：http://fot.fehbvm.com

PHP:  return [$a, $b];
来源：http://dmx.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ynf.gotoacloud.top

TS:   return { a, b };
来源：http://mpr.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zrs.xuetiantiany.cn

Go:   return a, b
来源：http://pzi.zdbjq.cn

Ruby: return a, b
来源：http://yzt.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://ocj.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://nyk.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://ycm.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yzc.zdqjudy.top

JS:   const square = x => x * x;
来源：http://qwj.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://aap.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oqj.yongpay.top

Go:   sq := func(x int) int { return x * x }
来源：http://jog.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://ycu.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://taz.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://btk.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oad.xylfe.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tce.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hhj.iojbl.cn

TS:   arr.map(String)
来源：http://ogo.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fux.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gxx.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://uzj.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jaw.ywan-chungtsiang.top

[C08] 闭包
来源：http://nvi.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aia.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ogn.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mkw.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nts.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mxm.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tvi.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xhp.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fgi.meibo888.top

[C09] 递归
来源：http://shu.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://voi.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ige.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fzx.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwl.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yci.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mkv.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fwv.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cto.vehdjk.com

[C10] 变量作用域
来源：http://xgo.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mao.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yne.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cpc.daxiang520.top


<!-- 参考信息 -->