代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://aaf.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lzn.xuetiantiany.cn

TS:   // Node.js：readline 模块
来源：http://app.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://jnd.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dzs.zhijiandao.cn

Ruby: gets.chomp
来源：http://wxt.cdnleiting.top

C#:   Console.ReadLine();
来源：http://lfz.yangfankeji.com

[A21] 保留指定小数位输出
来源：http://aku.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://fvx.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nob.yuxming.cn

JS:   (3.14159).toFixed(2)
来源：http://nks.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://wnm.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://wzt.gaohongyu789.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sso.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://gsf.epnwcf.com

C#:   3.14159.ToString("F2")
来源：http://gjy.xingfuxueyuan.xyz

[A22] 获取字符串长度
来源：http://ygk.smart0.xyz

Py:   len(s)
来源：http://pmr.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://epw.shuidangran.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uzp.hcnkem.com

TS:   s.length
来源：http://hlx.chenjidiqi.icu

Java: s.length()
来源：http://yvj.meibo888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zjx.52xcode.cn

Ruby: s.length
来源：http://jac.yvedp.cn

C#:   s.Length
来源：http://omv.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://qim.fengsongda.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pzt.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wjz.zhijiandao.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qlj.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dsc.yueranfly.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aip.uphjek.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ubu.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cbk.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://iiq.pycfn.com

[A24] 去除首尾空白
来源：http://xpu.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hro.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://njj.cdnleiting.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jcj.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fty.fktsv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://soa.tianlin.xyz

Go:   strings.TrimSpace(s)
来源：http://qbr.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://glo.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qwf.c1oappe.top

[A25] 字符串比较
来源：http://hjo.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://jai.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kva.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gcj.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dzg.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://unl.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ptv.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wcz.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bug.yvedp.cn

[A26] 类型转换总览
来源：http://uwr.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iaz.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rvb.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xgp.jlsjyb.cn

TS:   Number() String() Boolean() x as number
来源：http://ozy.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bxy.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bfq.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ymr.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pxs.feifeiyinyue.top

================================================================================
来源：http://gsu.shzxlz.cn

B. 流程控制
来源：http://gyg.sweek.top

================================================================================
来源：http://ent.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://lsa.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aua.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qvt.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gev.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uvw.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://srj.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uxb.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gcn.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nxd.52xcode.cn

[B02] 多分支 else if / elif
来源：http://zca.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zxk.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qvx.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcs.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppv.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cvu.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pkj.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zvz.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxi.shuidangran.top

[B03] switch / match / case
来源：http://sad.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lzd.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://frx.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kpk.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jiv.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vev.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tjo.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bcl.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eol.yonumen.top

[B04] for 计数循环
来源：http://pcc.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://gez.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uzb.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uvc.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mfs.cdnleiting.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hss.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gsv.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://dhy.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fow.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://anz.zhoulong.xyz

Py:   for item in arr: print(item)
来源：http://ido.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qvg.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://txs.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://svb.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mea.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rsm.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://vdh.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vns.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://vnk.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pmp.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ooh.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wbf.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smj.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iuf.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oko.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gdq.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://okr.316326.xyz

[B07] while 循环
来源：http://une.yvedp.cn

Py:   while i < 10: i += 1
来源：http://ngq.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jgj.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://ktp.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://yhq.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://btm.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://biw.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://wym.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://xjl.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://qwj.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://wha.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://cym.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://txq.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://qsl.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://eyv.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ukj.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cez.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://laa.yuanzhike.top

[B09] break 与 continue
来源：http://zta.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://knm.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qep.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrc.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndx.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hfj.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jas.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://myz.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://beu.fengsongda.top

[B10] 遍历同时拿索引
来源：http://hdc.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bpv.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wma.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fmr.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://voq.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kzv.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eoo.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yiz.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dyc.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://pct.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://smy.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://rpi.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyf.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qoi.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xlf.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hny.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://uyw.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wnp.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://blb.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cul.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zga.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hmq.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yrs.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mep.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rdt.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mla.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fga.guannengcc.top

[B13] 判断是否为数字
来源：http://jjg.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://uub.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://cji.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nvq.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://obx.cucudq.cn

Java: x instanceof Number
来源：http://zeo.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jtm.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://bul.tanke756.top

C#:   x is int or double or decimal
来源：http://knm.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://vqs.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lfv.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qxe.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://acn.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://pnr.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://buj.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lfb.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://nsm.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gty.yuxming.cn

[B15] 布尔运算与取反
来源：http://yat.yonumen.top

Py:   a and b or not c
来源：http://qqj.sxryk.cn

PHP:  $a && $b || !$c
来源：http://szl.cdnleiting.top

JS:   a && b || !c
来源：http://ngv.pengpengdd.cyou

TS:   a && b || !c
来源：http://wte.yonumen.top

Java: a && b || !c
来源：http://rqq.ybcxt.top

Go:   a && b || !c
来源：http://cbz.zhoulong.xyz

Ruby: a && b || !c
来源：http://ewl.gaohongyu789.top

C#:   a && b || !c
来源：http://eje.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://zvh.yuxming.cn

Py:   if not data: return
来源：http://beo.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://zht.bjfxy.top

JS:   if (!data) return;
来源：http://txq.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://ygn.zhiwuduotai.top

Java: if (data == null) return;
来源：http://sna.gaohongyu789.top

Go:   if data == nil { return }
来源：http://bul.zhijiandao.cn

Ruby: return if data.nil?
来源：http://mnk.ydjk.org.cn

C#:   if (data == null) return;
来源：http://vay.hesvh.cn

================================================================================
来源：http://cha.bjfxy.top

C. 函数与作用域
来源：http://zkj.zdqjudy.top

================================================================================
来源：http://crr.dianchejie.cn

[C01] 定义函数
来源：http://zxg.hammf.cn

Py:   def add(a, b): return a + b
来源：http://mas.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dto.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://ouz.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dib.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://oru.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xmt.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://svq.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://agn.sweek.top

[C02] 默认参数
来源：http://fpa.cheryme.top

Py:   def greet(name="World"): return name
来源：http://typ.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://qzf.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://blh.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://jul.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iba.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lva.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://opy.hesvh.cn

C#:   string Greet(string name = "World") => name;
来源：http://las.aibaodan.cn

[C03] 可变参数
来源：http://cfx.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://cxp.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ace.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tdc.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xft.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xrg.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kso.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fkf.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://huj.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://kft.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jko.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vpa.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ymg.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tzg.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://tin.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://lkv.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://uvu.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://bce.zhiwuduotai.top

[C05] 返回多个值
来源：http://zgr.sufxvd.cn

Py:   return a, b
来源：http://bxw.xinyue.icu

PHP:  return [$a, $b];
来源：http://gvv.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://eyx.jyoumei.cn

TS:   return { a, b };
来源：http://wnh.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://poi.wangdashe.top

Go:   return a, b
来源：http://bdd.hcnkem.com

Ruby: return a, b
来源：http://nak.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://mca.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://mjl.yongpay.top

Py:   square = lambda x: x * x
来源：http://agi.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://emx.nanxinkj.top

JS:   const square = x => x * x;
来源：http://bzt.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://sxb.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://czn.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://bcc.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://ytr.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://fbf.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://jep.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://any.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://uoh.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tvr.yanxiufei.cn

TS:   arr.map(String)
来源：http://mrq.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zms.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://swv.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://xtt.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qek.9152youxi.cn

[C08] 闭包
来源：http://smv.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://azw.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://owq.ivvv.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jua.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qdt.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mko.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zfp.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zpr.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ylf.316326.xyz

[C09] 递归
来源：http://xqg.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mfi.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://epi.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hvg.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nsr.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ymx.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mlq.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tmt.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://erm.ydzc1.top

[C10] 变量作用域
来源：http://yyr.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hvg.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gvd.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wnu.0kj1m.cn

TS:   同 JS
来源：http://ekt.yonumen.top

Java: 方法内为块级作用域
来源：http://xlw.cashguo.top

Go:   花括号块级作用域
来源：http://jym.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yxi.jyoumei.cn


<!-- 参考信息 -->